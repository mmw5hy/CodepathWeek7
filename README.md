# Project 7 - WordPress Pentesting

Time spent: **4** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Authenticated Cross-Site Scripting (XSS) via Media File Metadata
  - [ ] Summary: Meta information in audio files isn't sanitized by Wordpress correctly, so Wordpress is vulnerable to a XSS attack if an audio file containing XSS is placed in an audio playlist.
    - Vulnerability types: XSS
    - Tested in version: 4.2 (Released on 2015-04-23)
    - Fixed in version: 4.7.3
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: Create an audio file that contains XSS javascript code in the meta data, or download one such file from https://www.securify.nl/advisory/SFY20160742/xss.mp3. Then, have an administrator upload the audio file to a post as part of an audio playlist. Anytime that that post is opened, the XSS javascript will be triggered.
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/28f838ca3ee205b6f39cd2bf23eb4e5f52796bd7)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

No additional assets.

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

It was not documented in the lab tutorial that you must save your permalink settings to see posts. It took me a while to find the answer to why I was etting 404 errors when trying to view my posts, and this was it.

## License

    Copyright [2018] [Michael White]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

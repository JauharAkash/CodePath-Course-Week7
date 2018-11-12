# Project 7 - WordPress Pentesting

Time spent: 6 hours spent in total

> Objective: Find, analyze, recreate, and document vulnerabilities affecting an old version of WordPress

Pentesting Report

“Upload Same Origin Method Execution”
Vulnerability Name: Upload Same Origin Method Execution or ID: 2016-4566
  - [ ] Summary: Attacking the system by having the user download/click on a malicious comment that the user can put in the comments on the post. 
    - Vulnerability types: Stored XSS
    - Tested in version: 4.5.1
    - Fixed in version: 4.2.8
  - [ ] GIF Walkthrough: 
   <img src="https://github.com/JauharAkash/Codepathweek7/blob/master/1.gif" alt="1" title="1" />
  - [ ] Steps to recreate: Go to Post, go to the comments and paste the script which will then make a button. After clicking on the button, the alert will pop up to download a malicious script.
  - [ ] Affected source code:

“Unauthenticated Stored Cross Site-Scripting (XSS)”
Vulnerability Name: Unauthenticated Stored Cross Site-Scripting or ID: 2015-3440
  - [ ] Summary: Attacking a user when the user comes to the webpage and then gives you the alert.
    - Vulnerability types: Stored XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2
  - [ ] GIF Walkthrough: 
  <img src="https://github.com/JauharAkash/Codepathweek7/blob/master/1.gif" alt="1" title="2" />
  - [ ] Steps to recreate: Go to the post, paste the code in the comment section (shown in the gif). The alert will pop up then.
  - [ ] Affected source code:

“Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL” ID: 2017-6817
- [ ] Summary: Attack the user by having the user click on a youtube link. The link is embedded.
    - Vulnerability types: XSS
    - Tested in version: 4.0-4.7.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough: 
  <img src="https://github.com/JauharAkash/Codepathweek7/blob/master/1.gif" alt="3" title="1" />
  - [ ] Steps to recreate: Go to the post, put in comments the script which has the youtube link and the malicious code. Submit and then you will see the messages as shown by the gifs.
  - [ ] Affected source code:

“Large File Upload Error XSS”
1. (Optional) Vulnerability Name: “Large File Upload Error XSS” or ID: 2017-9061
  - [ ] Summary: Uploading a file which is allowed (size wise). Storing the malicious code (javascript) to trick the user thinking the file is too big.
    - Vulnerability types: XSS
    - Tested in version: 3.3-4.7
    - Fixed in version: 4.9.8
  - [ ] GIF Walkthrough: 
  <img src="https://github.com/JauharAkash/Codepathweek7/blob/master/4.gif" alt="1" title="1" /> 
  - [ ] Steps to recreate: Uploading an image larger than 2MB and naming the file ----  <img "src=x onerror=alert(1)">.png ---. Which stores the malicious script.
  - [ ] Affected source code:

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


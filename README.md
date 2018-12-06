# img2md

## Table of contents

- [img2md](#img2md)
    - [Table of contents](#table-of-contents)
    - [1 Introduction](#1-introduction)
    - [2 Install](#2-install)
    - [3 Usage](#3-usage)
    - [Reference](#reference)

## 1 Introduction

This is an alfred workflow that upload image in clipboard to Github, get markdown link.

It support upload image from:

1. File in finder
2. Screenshot in clipboard
3. Image in clipboard

## 2 Install

This workflow relay on [img2url](https://github.com/huntzhan/img2url) to work properly. Install img2url by:

``` shell
pip install img2url
```

Then create configuration file ~/.img2url.yml, and **change corresponding field**:

``` yml
remote: github

github_token: [your github token]
github_user: [github username]
github_repo: [github repository to store images]
github_commiter_name: [github username]
github_commiter_email: [github email]
```

github_token: [Personal access tokens](https://github.com/settings/tokens) of your GitHub account. If you don't have one, click "Generate new token" and select the "repo" scope, then record the generated token.

Download [img2md](https://raw.githubusercontent.com/xterat/img2md/master/img2md.alfredworkflow) and open in Alfred.

## 3 Usage

1. Upload from screenshot:
    1. Capture screen by ⌘ + ⇧ + 4 or ⌘ + ⌃ + ⇧ + 4
    2. ⌃ + ⇧ + P

2. Upload from file in finder:
    1. Copy file
    2. ⌃ + ⇧ + P

3. Upload from image in clipboard:
    1. Right click image in website, choose 'Copy Image'
    2. ⌃ + ⇧ + P

4. Show upload history:
    1. Open alfred
    2. Input 'uploaded' to show history
    3. Click to copy link to clipboard
    4. ⌘ + click to open link in browser

## Reference

- https://github.com/huntzhan/img2url
- https://github.com/jiwenxing/qimage-mac
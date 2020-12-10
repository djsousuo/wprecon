<h1 align="center">WPrecon (Wordpress Recon)</h1>

<p align="center"> 
  <a href="https://www.gnu.org/licenses/gpl-3.0">
    <img alt="License: GPL v3" src="https://img.shields.io/badge/License-GPLv3-blue.svg">
  </a>
  <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/m/blackcrw/wprecon">
  <img alt="GitHub go.mod Go version (branch)" src="https://img.shields.io/github/go-mod/go-version/blackcrw/wprecon/main?label=Go&logo=go">
  
Hello! Welcome. Wprecon (Wordpress Recon), is a vulnerability recognition tool in CMS Wordpress, 100% developed in Go.
</p> 

### Version: Alfa !

## Features

| Status        | Features              |
|---------------|-----------------------|
|   ✅          | Random Agent          |
|   ✅          | Detection WAF         |
|   ❌          | Plugin Scanner        |
|   ⚠️           | User Enumerator       |
|   ❌          | Plugin Scanner        |
|   ❌          | Theme Scanner         |
|   ❌          | Vulnerability Scanner |
|   ❌          | Tor Proxy's           |

<h2 align="center">Usage</h2>

| Flag(s)            | Description                                          |
|--------------------|------------------------------------------------------|
|-d, --detection-waf | I will try to detect if the target is using any WAF. |
|-h, --help          | help for wprecon                                     |
|--random-agent      | Use randomly selected HTTP(S) User-Agent header value|
|-u, --url string    | Target URL (Ex: http(s)://google.com/) `(Required)`  |
|-v, --verbose       | Verbosity                                            |

<h2 align="center">WPrecon running</h2>

Command: `wprecon --url "https://www.xxxxxxx.com/" --detection-waf`
##### Output:
```
—————————————————————————————————————————————————————————————————————

___       ______________________________________________   __
__ |     / /__  __ \__  __ \__  ____/_  ____/_  __ \__  | / /
__ | /| / /__  /_/ /_  /_/ /_  __/  _  /    _  / / /_   |/ /
__ |/ |/ / _  ____/_  _, _/_  /___  / /___  / /_/ /_  /|  /
____/|__/  /_/     /_/ |_| /_____/  \____/  \____/ /_/ |_/

Github: https://github.com/blackcrw/wprecon
Version: 0.0.1a
—————————————————————————————————————————————————————————————————————
[•] Target: https://www.xxxxxxx.com/
[•] Starting: 09/jan/2020 12:11:17

[•] Listing enable: https://www.xxxxxxx.com/wp-content/plugins/
[•] Listing enable: https://www.xxxxxxx.com/wp-content/themes/
[•••] Status Code: 200 — URL: https://www.xxxxxxx.com/wp-admin/
[•••] I'm not absolutely sure that this target is using wordpress! 37.50% chance. do you wish to continue ? [Y/n]: Y
[•••] Status Code: 200 — WAF: Wordfence Security Detected
[•••] Do you wish to continue ?! [Y/n] : Y
```

<h2 align="center">Install & Compile</h2>

For you to compile **wprecon** you will need to have the golang compiler installed.
And for that you will access the official website of golang and will download and install it. [**Here!**](https://golang.org/dl/)

Once downloaded and installed you will download **wprecon** directly from github with the command:
###### **(There are two ways to do this, and I will teach both.)**
1. Primary way:
- `go get github.com/blackcrw/wprecon`;

2. Second way:
- `mkdir ~/Go/src/github.com/blackcrw/wprecon`;
- `cd ~/Go/src/github.com/blackcrw`;
- `git clone https://github.com/blackcrw/wprecon`;
- `go get wprecon`.

After downloading **wprecon** you will compile with the command:
###### **(There are already some ways to do this ... but I'll show you the simplest and quickest.)**
- `go build ~/Go/src/blackcrw/github.com/blackcrw/wprecon`.

### 🎉 🎉 🎉 Ready!!! Your **wprecon** is compiled, now just start using it. It was pretty easy, right ?! 

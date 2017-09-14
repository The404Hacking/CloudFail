# CloudFail

CloudFail is a tactical reconnaissance tool which aims to gather enough information about a target protected by CloudFlare in the hopes of discovering the location of the server. Using Tor to mask all requests, the tool as of right now has 3 different attack phases. [Share](https://telegram.me/share/url?url=https://github.com/The404Hacking/CloudFail&text=CloudFlare%20Bypasser%20-%20Find%20Hidden%20IP)

1. Misconfigured DNS scan using DNSDumpster.com.
2. Scan the Crimeflare.com database.
3. Bruteforce scan over 2500 subdomains.

![Example usage](http://puu.sh/pq7vH/62d56aa41f.png "Example usage")

> Please feel free to contribute to this project. If you have an idea or improvement issue a pull request!

## Disclaimer
This tool is a PoC (Proof of Concept) and does not guarantee results.  It is possible to setup CloudFlare properly so that the IP is never released or logged anywhere; this is not often the case and hence why this tool exists.
This tool is only for academic purposes and testing  under controlled environments. Do not use without obtaining proper authorization
from the network owner of the network under testing.
The author bears no responsibility for any misuse of the tool.

## Install on Kali/Debian

First we need to install pip3 for python3 dependencies:

```$ sudo apt-get install python3-pip```

Then we can run through dependency checks:

```$ pip3 install -r requirements.txt```

## Usage

To run a scan against a target:

```python3 cloudfail.py --target seo.com```

To run a scan against a target using Tor:

```service tor start```

(or if you are using Windows or Mac install vidalia or just run the Tor browser)

```python3 cloudfail.py --target seo.com --tor```

> Please make sure you are running with Python3 and not Python2.*.

## Dependencies
**Python3**
* argparse
* colorama
* socket
* binascii
* datetime
* requests
* win_inet_pton

## Download and Clone
> Download: [https://github.com/The404Hacking/CloudFail/archive/master.zip](https://github.com/The404Hacking/CloudFail/archive/master.zip)

> Clone: git clone [https://github.com/The404Hacking/CloudFail.git](https://github.com/The404Hacking/CloudFail.git)

## The404Hacking | Digital UnderGround Team
[The404Hacking](https://T.me/The404Hacking)

## Follow us !
[The404Hacking](https://T.me/The404Hacking) - [The404Cracking](https://T.me/The404Cracking)

[Instagram](https://instagram.com/The404Hacking) - [GitHub](https://github.com/The404Hacking)

[YouTube](http://yon.ir/youtube404) - [Aparat](http://www.aparat.com/The404Hacking)

[The404Hacking.BlogSky.Com](http://the404hacking.blogsky.com)
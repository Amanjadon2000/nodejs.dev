---
title: April 2021 Security Releases
blogAuthors: ['node-js-website']
category: 'vulnerabilities'
---

## _(Update 6-Apr-2021)_ Security releases available

Updates are now available for v10,x, v12.x, v14.x and v15.x Node.js release lines for the following issues.

### OpenSSL - CA certificate check bypass with X509\_V\_FLAG\_X509\_STRICT (High) (CVE-2021-3450)

This is a vulnerability in OpenSSL which may be exploited through Node.js. You can read more about it in
<https://www.openssl.org/news/secadv/20210325.txt>

Impacts:

* All versions of the 15.x, 14.x, 12.x and 10.x releases lines

### OpenSSL - NULL pointer deref in signature\_algorithms processing (High) (CVE-2021-3449)

This is a vulnerability in OpenSSL which may be exploited through Node.js. You can read more about it in
<https://www.openssl.org/news/secadv/20210325.txt>

Impacts:

* All versions of the 15.x, 14.x, 12.x and 10.x releases lines

### npm upgrade - Update y18n to fix Prototype-Pollution (High) (CVE-2020-7774)

This is a vulnerability in the y18n npm module which may be exploited by prototype pollution.
You can read more about it in
<https://github.com/advisories/GHSA-c4w7-xm78-47vh>

Impacts:

* All versions of the 14.x, 12.x and 10.x releases lines

## Downloads and release details

* [Node.js v10.24.1 (LTS)](https://nodejs.org/en/blog/release/v10.24.1/)
* [Node.js v12.22.1 (LTS)](https://nodejs.org/en/blog/release/v12.22.1/)
* [Node.js v14.16.1 (LTS)](https://nodejs.org/en/blog/release/v14.16.1/)
* [Node.js v15.14.0 (Current)](https://nodejs.org/en/blog/release/v15.14.0/)

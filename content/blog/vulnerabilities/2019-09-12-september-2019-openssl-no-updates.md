---
title: OpenSSL security releases do not require Node.js security releases
blogAuthors: ['node-js-website']
category: 'vulnerabilities'
---

### Summary

The OpenSSL Security releases of September 10th, 2019 do not affect Node.js.

### Analysis

Our assessment of the [security advisory](https://www.openssl.org/news/secadv/20190910.txt) is:

* ECDSA remote timing attack (CVE-2019-1547)
  Not affected. Node supports only named curves for ECDSA signing.

* Fork Protection (CVE-2019-1549)
  Not affected. Node.js always call `exec()` after `fork()` so will not
  duplicate the PRNG state in the forked process.

* Padding Oracle in `PKCS7_dataDecode` and `CMS_decrypt_set1_pkey` (CVE-2019-1563)
  Not affected. Node does not support PCKS7 and CMS.

Given this assessment, the OpenSSL updates will be treated as non-security
patch updates, and will come out in the regularly scheduled updates to
supported release lines.

### Acknowledgements

Thanks to [Shigeki Ohtsu](https://github.com/shigeki) for his rapid analysis
of the OpenSSL security advisory.

### Contact and future updates

The current Node.js security policy can be found at <https://github.com/nodejs/node/blob/HEAD/SECURITY.md#security>,
including information on how to report a vulnerability in Node.js.

Subscribe to the low-volume announcement-only **nodejs-sec** mailing list at
<https://groups.google.com/forum/#!forum/nodejs-sec> to stay up to date on
security vulnerabilities and security-related releases of Node.js and the
projects maintained in the
[nodejs GitHub organization](https://github.com/nodejs).

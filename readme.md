### Intro

First, it's useful to get known with [acme-tiny](https://github.com/diafygi/acme-tiny).

Then check the [update-certificate.sh](update-certificate.sh.example) example.

I've included [NGinx config examples](nginx) as well.

### Options

- **--account-key**

   The path for your Let's Encrypt account key.
   Will be created if doesn't exist.

- **--acmetiny**

   The path where [acme-tiny](https://github.com/diafygi/acme-tiny) is stored.
   Will be dowloaded if doesn't exist.

- **--keys**

   Where to store keys and certificates

- **--challenges**

   Where to store challenges.

- **--domain1**

   The main domain name.

- **--domain2**

   An additional domain name.
   To use it, check and fill [openssl.cnf](openssl.cnf.example).
   `Warning: not tested too much!`

- **--keyname**

   The basename for the key and certificate files.
   If not specified — the main domain name will be used.

- **--nodhparam**

   skip `dhparam` file creation _(not recommended)_.

- **--no-questions**

   Don't ask questions.
   Use it if you use this script with crontab, etc.

---

#### MIT License

Copyright (c) 2017 

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

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

   The ain domain name.

- **--domain2**

   An additional domain name.
   To use it, check and fill [openssl.cnf](openssl.cnf.example).
   `Warning: not tested too much!`

- **--keyname**

   The basename for the key and certificate files.
   If not specified — domain name will be used.

- **--nodhparam**

   skip `dhparam` file creation _(not recommended)_.

- **--no-questions**

   Don't ask questions.
   Use it if you put this script in crontab.

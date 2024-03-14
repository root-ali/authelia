---
title: "authelia crypto certificate rsa request"
description: "Reference for the authelia crypto certificate rsa request command."
lead: ""
date: 2022-06-27T18:27:57+10:00
draft: false
images: []
menu:
  reference:
    parent: "cli-authelia"
weight: 905
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## authelia crypto certificate rsa request

Generate an RSA private key and certificate signing request

### Synopsis

Generate an RSA private key and certificate signing request.

This subcommand allows generating an RSA private key and certificate signing request.

```
authelia crypto certificate rsa request [flags]
```

### Examples

```
authelia crypto certificate rsa request --help
```

### Options

```
  -b, --bits int                       number of RSA bits for the certificate (default 2048)
  -n, --common-name string             certificate common name
      --country strings                certificate country
  -d, --directory string               directory where the generated keys, certificates, etc will be stored
      --duration string                duration of time the certificate is valid for (default "1y")
      --file.csr string                name of the file to export the certificate request data to (default "request.csr")
      --file.extension.legacy string   string to include before the actual extension as a sub-extension on the PKCS#1 and SECG1 legacy formats (default "legacy")
      --file.private-key string        name of the file to export the private key data to (default "private.pem")
  -h, --help                           help for request
      --legacy                         enables the output of the legacy PKCS#1 and SECG1 formats when enabled
  -l, --locality strings               certificate locality
      --not-after string               latest date and time the certificate is considered valid in various formats
      --not-before string              earliest date and time the certificate is considered valid in various formats (default is now)
  -o, --organization strings           certificate organization (default [Authelia])
      --organizational-unit strings    certificate organizational unit
  -p, --postcode strings               certificate postcode
      --province strings               certificate province
      --sans strings                   subject alternative names
      --signature string               signature algorithm for the certificate (default "SHA256")
  -s, --street-address strings         certificate street address
```

### Options inherited from parent commands

```
  -c, --config strings                        configuration files or directories to load, for more information run 'authelia -h authelia config' (default [configuration.yml])
      --config.experimental.filters strings   list of filters to apply to all configuration files, for more information run 'authelia -h authelia filters'
```

### SEE ALSO

* [authelia crypto certificate rsa](authelia_crypto_certificate_rsa.md)	 - Perform RSA certificate cryptographic operations

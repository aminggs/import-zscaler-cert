# import-zscaler-cert

Mac shell script to import zscaler root CA certificate into various trust stores

## Usage

```shell
./import-zscaler-cert.sh
```

No arguments required, the root CA cert is embedded in the script.

## Description

Saves the Zscaler root CA cert to ~/.certs/Zscaler-Root-CA.pem and
updates the following trust stores:

* JDK key stores for all JDKs listed by `/usr/libexec/java_home -V`
* JetBrains applications (`~/Library/Application\ Support/JetBrains/*`)
* DBeaver (`/Applications/DBeaver.app`)

## Copyright and License

Copyright Andrew M. Inggs.

Licensed under the Apache License, Version 2.0, unless otherwise
explicitly stated. See file LICENSE for details.

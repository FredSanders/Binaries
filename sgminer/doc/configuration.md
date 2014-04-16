# Configuration and command-line options

*Work in progress!*


## Config-file and CLI options

### algorithm

Allows choosing between the few mining algorithms for incompatible
cryptocurrencies.

*Argument:* string

*Default:* `scrypt`

*Supported:*

* `adaptive-n-scrypt` - Vertcoin-style adaptive N-factor scrypt.
  N-factor defaults to 11. Aliases: `adaptive-nscrypt` (to be removed
  in future versions) and `nscrypt`.
* `scrypt` - Litecoin-style static N-factor scrypt.
* `scrypt-jane`
* `darkcoin`
* `qubitcoin`
* `myriadcoin-groestl`
* `quarkcoin`
* `fuguecoin`
* `inkcoin`
* `animecoin`
* `groestlcoin`
* `sifcoin`
* `twecoin`

* everything else - currently defaults to `scrypt`, subject to change
  without warning.


### nfactor

Overrides the default scrypt parameter N, specified as the factor of 2
(`N = 2^nfactor`).

*Argument:* whole number (>1).

*Default:* depends on `algorithm`; otherwise `10`.


## CLI-only options

*TODO*

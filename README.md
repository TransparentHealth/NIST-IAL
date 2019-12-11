# 800-63-3-Trustmark URL
A Vectors of Trust Trustmark based on NIST SP 800-63-3 [IAL](https://doi.org/10.6028/NIST.SP.800-63a)
and [AAL](https://doi.org/10.6028/NIST.SP.800-63b).

The link to this repository shall be used as the value of the `vtm` claim. For example:

    ...
    "vtm": "https://github.com/TransparentHealth/800-63-3-trustmark/edit/master/README.md"
    ...

Mapping
-------

| NIST SP 800 63 3 Value                                      | Vectors of Trust Mapping |
| ----------------------------------------------------------- | ------------------------ |
| [IAL1](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P1                       |
| [IAL2](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P2                       |
| [IAL3](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P3                       |
| [AAL1](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C1                       |
| [AAL2](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C2                       
| [AAL3](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C3                       |


More References
---------------

* [NIST SP 800-63-3 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/) 
* [RFC 8485 Vectors of Trust](https://tools.ietf.org/html/rfc8485)
* [OpenID Connect Profile for Consumer Health](https://github.com/TransparentHealth/openid-connect-consumerhealth-profile/blob/master/README.md)

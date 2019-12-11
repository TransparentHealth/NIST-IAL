# 800-63-3-Trustmark URL
A [Vectors of Trust Trustmark]((https://tools.ietf.org/html/rfc8485)) based on 
NIST SP 800-63-3. Specifically:

* Identity Assuance Levels ([IAL](https://doi.org/10.6028/NIST.SP.800-63a))
* Autheticator Assurance Levels ([AAL](https://doi.org/10.6028/NIST.SP.800-63b))

The link to this repository shall be used as the value of the `vtm` claim. For example:

    ...
    "vtm": "https://github.com/TransparentHealth/800-63-3-trustmark/edit/master/README.md"
    ...

Mapping
-------

| Enrollment and Identity Proofing Value                      | Vectors of Trust Value |
| ----------------------------------------------------------- | ---------------------- |
| [IAL1](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P1                     |
| [IAL2](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P2                     |
| [IAL3](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | P3                     |

| Authentication and Lifecycle Management                     | Vectors of Trust Value |
| ----------------------------------------------------------- | ---------------------- |
| [AAL1](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C1                     |
| [AAL2](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C2                     |               
| [AAL3](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | C3                     |


More References
---------------

* [NIST SP 800-63-3 Digital Identity Guidelines Homepage](https://pages.nist.gov/800-63-3/) 
* [RFC 8485 Vectors of Trust](https://tools.ietf.org/html/rfc8485)
* [OpenID Connect Profile for Consumer Health](https://github.com/TransparentHealth/openid-connect-consumerhealth-profile/blob/master/README.md)

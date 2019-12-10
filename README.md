# 800-63-3-Trustmark URL
A Vectors of Trust Trustmark based on NIST SP 800-63-3 IAL and AA. https://pages.nist.gov/800-63-3/.

The link to this repository shall be used as the value of the `vtm` claim. For example:

    ...
    "vtm": "https://github.com/TransparentHealth/800-63-3-trustmark/edit/master/README.md"
    ...

Mapping
-------

| NIST SP 800 63 3 Value | Vectors of Trust Mapping |
| ---------------------- | ------------------------ |
| IAL 1                  | P1                       |
| IAL 2                  | P2                       |
| IAL 3                  | P3                       |
| AAL 1                  | C1                       |
| AAL 2                  | C2                       |
| AAL 3                  | C3                       |

References
----------

* [NIST SP 800-63-3 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/) 
* [RFC 8485 Vectors of Trust](https://tools.ietf.org/html/rfc8485)
* [OpenID Connect Profile for Consumer Health](https://github.com/TransparentHealth/openid-connect-consumerhealth-profile/blob/master/README.md)

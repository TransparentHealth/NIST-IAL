# 800-63-3-Trustmark

The is a [Vectors of Trust Trustmark](https://tools.ietf.org/html/rfc8485) based on 
[NIST SP 800-63-3 Digital Identity Guidelines](https://pages.nist.gov/800-63-3/). It was created as part of an effort to establish a best practice for sharing digital identities in a healthcare setting. Entities who are operating or implementing [OpenID Connect](https://openid.net/connect/) Identity Providers(IdP) may use this as an implementation guide. While designed with US healthcare in mind, it is not healthcare specific.  The [URL](https://github.com/TransparentHealth/800-63-3-trustmark/) to this file serves as the trustmark itself. The `vtm`is `https://github.com/TransparentHealth/800-63-3-trustmark/`

Scope
-----

* Identity Assuance Levels (IAL) as defined in ([NIST SP 800-63A: Enrollment and Identity Proofing](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63a.pdf))
* Autheticator Assurance Levels (AAL) as defined in ([NIST SP 800-63B: Authentication and Lifecycle Management](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-63b.pdf))



Trustmark Details
-----------------

| Identity Assuance Level `IAL` Value                         | VoT Identity Proofing `P` Value                      |
| ----------------------------------------------------------- | ---------------------------------------------------- |
| [IAL1](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | [P1](https://tools.ietf.org/html/rfc8485#section-2.1)|                  
| [IAL2](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | [P2](https://tools.ietf.org/html/rfc8485#section-2.1)|
| [IAL3](https://pages.nist.gov/800-63-3/sp800-63a.html#sec4) | [P3](https://tools.ietf.org/html/rfc8485#section-2.1)|


| Autheticator Assurance Level `AAL` Value                    | VoT Credential `C` Value                             |
| ----------------------------------------------------------- | ---------------------------------------------------- |
| [AAL1](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | [C1](https://tools.ietf.org/html/rfc8485#section-2.2)|
| [AAL2](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | [C2](https://tools.ietf.org/html/rfc8485#section-2.2)|   
| [AAL3](https://pages.nist.gov/800-63-3/sp800-63b.html#sec4) | [C3](https://tools.ietf.org/html/rfc8485#section-2.2)|                     


How To Use this Trustmark
-------------------------

Whithin your OpenID Connect Identity Provider, include the folling value in the ink to this repository shall be used as the value of the `vtm` claim. This should be present along with the Verto0rs of Trust claim `vot` as well.  For example, within the payload of your OpenID Connect `id_token` which is provided to relying parties:

    {
    "issuer": "https://oidc.example.com",
    "sub": "12345678901234",
    "given_name": "James",
    "family_name": "Kirk",
    ...
    "vot": "P2.C2.A1",
    "vtm": "https://github.com/TransparentHealth/800-63-3-trustmark",
    ...
    }

See the Vectors of Trust for more information.


Reference List
--------------

* [NIST SP 800-63-3 Digital Identity Guidelines Homepage](https://pages.nist.gov/800-63-3/) 
* [RFC 8485 Vectors of Trust](https://tools.ietf.org/html/rfc8485)
* [OpenID Connect Profile for Consumer Health](https://github.com/TransparentHealth/openid-connect-consumerhealth-profile/blob/master/README.md)
* [HEART WG](https://openid.net/wg/heart/)

# ACME Proof-of-Possession Authorization

[![Build Status](https://github.com/ietf-wg-acme/draft-ietf-acme-pop/actions/workflows/ghpages.yml/badge.svg)](https://github.com/ietf-wg-acme/draft-ietf-acme-pop/actions/workflows/ghpages.yml)

This is the working area for the IETF [ACME Working Group](https://datatracker.ietf.org/wg/acme/documents/) Internet-Draft, "Automated Certificate Management Environment (ACME) Extension for Proof-of-Possession".

The draft defines an optional ACME extension for certificate issuance without a PKCS#10 Certificate Signing Request (CSR). A client declares the certificate public key in `popKey` and proves possession through a dedicated `pop` authorization containing a `pop-01` challenge. The design supports both signature-capable keys and KEM-only keys, including use with ACME certificate profiles, device attestation, C509 certificates, and STAR certificates.

**Status:** Working group document. Substantive protocol discussion occurs in the [issue tracker](https://github.com/ietf-wg-acme/draft-ietf-acme-pop/issues) and on the [ACME Working Group mailing list](mailto:acme@ietf.org).

* [Editor's Copy (HTML)](https://ietf-wg-acme.github.io/draft-ietf-acme-pop/draft-ietf-acme-pop.html)
* [Editor's Copy (txt)](https://ietf-wg-acme.github.io/draft-ietf-acme-pop/draft-ietf-acme-pop.txt)
* [Datatracker Page](https://datatracker.ietf.org/doc/draft-ietf-acme-pop/)
* [Working Group Draft](https://datatracker.ietf.org/doc/html/draft-ietf-acme-pop)
* [Compare Editor's Copy to Latest](https://ietf-wg-acme.github.io/draft-ietf-acme-pop/#go.draft-ietf-acme-pop.diff)

## Related Specifications

* [RFC 8555](https://www.rfc-editor.org/rfc/rfc8555) - ACME, the protocol extended by this draft.
* [RFC 8739](https://www.rfc-editor.org/rfc/rfc8739) - ACME STAR certificates and automatic renewal.
* [RFC 9773](https://www.rfc-editor.org/rfc/rfc9773) - ACME Renewal Information (ARI).
* [FIPS 203](https://doi.org/10.6028/NIST.FIPS.203) - ML-KEM, used for KEM-only certificate keys.
* [FIPS 204](https://doi.org/10.6028/NIST.FIPS.204) - ML-DSA signature algorithms.
* [FIPS 205](https://doi.org/10.6028/NIST.FIPS.205) - SLH-DSA signature algorithms.
* [ACME Profiles](https://datatracker.ietf.org/doc/draft-ietf-acme-profiles/) - Certificate profile selection for ACME orders.
* [ACME Device Attestation](https://datatracker.ietf.org/doc/draft-ietf-acme-device-attest/) - Device identity and attestation mechanisms.
* [ACME RATS](https://datatracker.ietf.org/doc/draft-ietf-acme-rats/) - Remote attestation identifiers and challenge types.

## Building the Draft

Formatted text and HTML versions of the draft can be built using `make`.

```sh
make
```

This requires that you have the necessary software installed. See [the instructions](https://github.com/martinthomson/i-d-template/blob/main/doc/SETUP.md).

## Contributing

See the [guidelines for contributions](CONTRIBUTING.md). Discussion of this work occurs on the [ACME Working Group mailing list](mailto:acme@ietf.org) ([archive](https://mailarchive.ietf.org/arch/browse/acme/)). Contributions can be made by creating pull requests or opening issues in this repository.

---
layout: main.pug
---

# SIKE – <small>Supersingular Isogeny Key Encapsulation</small>

SIKE is an isogeny-based key encapsulation suite based on pseudo-random
walks in supersingular isogeny graphs, thay was submitted to the [NIST
standardization
process](https://csrc.nist.gov/Projects/Post-Quantum-Cryptography) on
post-quantum cryptography. It contains two algorithms: 

- A CPA-secure public key encryption algorithm **SIKE.PKE**, and
- A CCA-secure key encapsulation mechanism **SIKE.KEM**,

each instantiated with three parameter sets: **SIKEp503**,
**SIKEp571** and **SIKEp964**.

| News |
|-|
| **2017-11-30:** | SIKE proposal submitted to [NIST PQC process](https://csrc.nist.gov/Projects/Post-Quantum-Cryptography).

## Specification

### NIST submission

The submission package can be downloaded from the [NIST web
site](https://csrc.nist.gov/projects/post-quantum-cryptography/round-1-submissions)
or from [this server](files/SIKE.zip).

Note that these two packages are not identical; the NIST package
contains [corrupted PDF
files](https://groups.google.com/a/list.nist.gov/forum/#!topic/pqc-forum/FB_H0WkXU_M)
which were corrupted post-submission.  We recommend that you download
the package from this server to get the originally submitted,
uncorrupted version.

If you just want the uncorrupted PDF file, it is available
[here](files/SIDH-spec.pdf).

### Resources

#### Research articles

- Gora Adj, Daniel Cervantes-Vázquez, Jesús-Javier Chi-Domínguez, Alfred
  Menezes and Francisco Rodríguez-Henríquez. [On the cost of computing
isogenies between supersingular elliptic
curves](https://eprint.iacr.org/2018/313), Apr. 2018.

- Steven D. Galbraith, Christophe Petit, Barak Shani, and Yan Bo Ti.
  [On the security of supersingular isogeny
cryptosystems](https://eprint.iacr.org/2016/859), Sep. 2016.

- Craig Costello, Patrick Longa and Michael Naehrig. [Efficient
  algorithms for supersingular isogeny
  Diffie-Hellman](https://eprint.iacr.org/2016/413), Apr. 2016.

- Luca De Feo, David Jao and Jérôme Plût. [Towards Quantum-Resistant
  Cryptosystems From Supersingular Elliptic Curve
Isogenies](https://eprint.iacr.org/2011/506), Sep. 2011.

#### Expository articles

- Luca De Feo. [Mathematics of Isogeny Based
  Cryptography](https://arxiv.org/abs/1711.04062), Nov. 2017.

- Wouter Castryck. [Elliptic curves are quantum dead, long live elliptic
  curves](https://www.esat.kuleuven.be/cosic/elliptic-curves-are-quantum-dead-long-live-elliptic-curves/),
May 2017.


- David Urbanik. [A friendly introduction to Supersingular Isogeny
  Diffie-Hellman](https://csclub.uwaterloo.ca/~dburbani/work/friendlysidh.pdf),
Mar. 2017.

#### Talks

- David Jao. [Supersingular Isogeny Key Encapsulation](files/SIKE.pdf),
  NIST PQC Standardization Conference, Apr. 2018.

- Craig Costello. [Key encapsulation using supersingular
  isogenies](https://ecc2017.cs.ru.nl/slides/ecc2017-costello.pdf), Nov.
2017.

- Luca De Feo. [20 Years of Isogeny-Based
  Cryptography](http://defeo.lu/docet/assets/slides/2017-11-14-ecc.pdf),
Nov. 2017.

- Deirdre Connolly. [Supersingular Isogeny
  Diffie-Hellman](https://www.youtube.com/watch?v=ctP24WKusX0)
([slides](https://dconnolly.github.io/talks/cloudflare-crypto-meetup-feb-2017/Crypto%20Meetup%20Feb%202017.pdf)),
Cloudflare Crypto Meetup, Feb. 2017.

- David Urbanik. [Introduction to the post-quantum Supersingular Isogeny
  Diffie-Hellman protocol](https://www.youtube.com/watch?v=PW5Vsu57o9I)
([slides](https://csclub.uwaterloo.ca/~dburbani/work/sidh_talk_july_2016.pdf)),
Jul. 2016.

## Implementation

The SIKE submission contains six implementations. These are available
from the [submission package](files/SIKE.zip), or individually below:

- [Reference implementation](files/reference.zip)
- [Optimized implementation](files/optimized.zip)
- [AMD64 implementation](files/x64.zip)
- [ARM64 implementation](files/arm64.zip)
- [VHDL implementation](files/vhdl.zip)
- [Weierstrass implementation](files/weierstrass.zip)

All of the above implementations are licensed under the [MIT
license](files/License.txt).

The following implementations are available from third parties:

- [Cloudflare p751sidh package](https://github.com/cloudflare/p751sidh)

- [Microsoft SIDH library](https://github.com/Microsoft/PQCrypto-SIDH)

### Known Answer Test

Known Answer Test (KAT) files are available from the [submission
package](files/SIKE.zip), or individually from [this
server](files/KAT/).

## Authors

- David Jao, University of Waterloo and evolutionQ, Inc. (principal submitter)
- Reza Azarderakhsh, Florida Atlantic University
- Matthew Campagna, Amazon
- Craig Costello, Microsoft Research
- Luca De Feo, IBM Research Zürich
- Basil Hess, Infosec Global
- Amir Jalali, Florida Atlantic University
- Brian Koziel, Texas Instruments
- Brian LaMacchia, Microsoft Research
- Patrick Longa, Microsoft Research
- Michael Naehrig, Microsoft Research
- Joost Renes, Radboud University
- Vladimir Soukharev, Infosec Global
- David Urbanik, University of Waterloo

### Contact

- [sike@sike.org](mailto:sike@sike.org)

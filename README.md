# The Strong Coupling Constant from Arithmetic Geometry

**α_s(M_Z) = Ω₄ / 23 = 0.117921**

The real period of elliptic curve 1132b1, divided by the discriminant prime of x³ − x − 1, equals the strong coupling constant. Zero free parameters.

| Quantity | Value |
|---|---|
| Elliptic curve | E₄: y² = x³ + 4x + 1 (Cremona 1132b1) |
| Conductor | 1132 = 4 × 283 (Q-sector discriminant prime) |
| Real period Ω₄ | 2.71217511598... |
| Divisor | 23 = \|disc(x³ − x − 1)\| (ρ-sector discriminant prime) |
| **α_s = Ω₄ / 23** | **0.117921** |
| PDG measured | 0.1179 ± 0.0009 |
| Error | 0.02% (0.023σ) |

No QCD. No renormalization group. No lattice calculation. A period divided by a prime.

## Run

```bash
pip install mpmath sympy
python3 pdt_strong_coupling.py
```

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stalex444/pdt-strong-coupling/blob/main/pdt_strong_coupling.ipynb)

## What This Computes

The Q-sector polynomial x⁴ − x − 1 defines the elliptic curve E₄ (Cremona 1132b1) whose real period is:

$$\Omega_4 = \int_{e_1}^{\infty} \frac{dx}{\sqrt{x^3 + 4x + 1}} = 2.71218...$$

Dividing by 23 — the absolute discriminant of the ρ-sector polynomial x³ − x − 1 — gives the strong coupling constant at the Z mass:

$$\alpha_s(M_Z) = \frac{\Omega_4}{23} = 0.117921...$$

The Birch and Swinnerton-Dyer conjecture is proved for this curve (Gross-Zagier and Kolyvagin, 1990). The period is an exact computable invariant. The match to experiment is within 0.023σ.

## Context

The two polynomials x³ − x − 1 and x⁴ − x − 1 sit at the Pisot boundary — the transition between convergent and divergent algebraic dynamics in the polynomial family xⁿ = x + 1. Their arithmetic properties are established in:

- **Arithmetic Geometry at the Pisot Boundary** — six theorems on discriminants, Galois groups, class fields, and the Hodge star ([Zenodo](https://zenodo.org/search?q=metadata.creators.person_or_org.name%3A%22Stephanie%20Alexander%22))
- **Elliptic Curves Associated to the Pisot-Boundary Polynomials** — full arithmetic invariants of both curves ([Zenodo](https://zenodo.org/search?q=metadata.creators.person_or_org.name%3A%22Stephanie%20Alexander%22))

The strong coupling constant is the first fundamental constant of nature identified with an exact computable invariant of arithmetic geometry, with zero free parameters.

## Verify Independently

The period can be confirmed against the LMFDB entry: [https://www.lmfdb.org/EllipticCurve/Q/1132/b/1](https://www.lmfdb.org/EllipticCurve/Q/1132/b/1)

## Author

Stephanie Alexander — stephanie@baryonix.com — 2026

Part of Pisot Dimensional Theory. 


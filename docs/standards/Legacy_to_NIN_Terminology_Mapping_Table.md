# Legacy-to-NIN Terminology Mapping Table

Purpose: unify wording from early FlexiLink papers with current NIN standards vocabulary.

## Core mapping

| Legacy term (2012 paper) | Recommended NIN-era term | Practical meaning | Evidence for legacy term | Evidence for NIN term |
|---|---|---|---|---|
| SF (Synchronous Flow) | **Guaranteed service flow** | Reserved/time-slotted deterministic flow | `201210 Flexilink...pdf` p.3, p.4 | `gr_NIN003v010101p.pdf` p.8, p.12 |
| AF (Asynchronous Flow) | **Basic service flow** (best-effort) | Non-reserved queued traffic | `201210 Flexilink...pdf` p.3, p.4 | `gr_NIN003v010101p.pdf` p.12 |
| CM (Control Message) | **Control-plane signalling message / transaction** | Flow setup/teardown/resource control | legacy usage context (2012 architecture) | `gs_NIN005v010101p.pdf` p.16 (signalling flow/control plane) |
| AF background/bulk traffic | **Basic service low-priority traffic** | Uses residual capacity, delay/loss tolerant | `201210 Flexilink...pdf` p.4, p.7 | nearest: `gr_NIN003v010101p.pdf` p.12 (basic service) |

---

## Usage policy for new documents

1. First mention format (for transition period):
   - `Guaranteed service flow (legacy SF)`
   - `Basic service flow (legacy AF)`

2. After first mention, use only:
   - `Guaranteed service`
   - `Basic service`

3. Avoid using `SF/AF` as primary normative terminology in new standards-facing text.

---

## Quick citation anchors
- Legacy SF/AF definitions: 2012 paper p.3–4.
- NIN deterministic/basic service terminology: GR NIN 003 p.8, p.12.
- Control plane/signalling flow: GS NIN 005 p.16.

# SF/AF Replacement Suggestion List (Non-destructive)

This is a suggestion list only. It does **not** modify original source files.

## A) Legacy paper occurrences (from `201210 Flexilink A unified low latency network architecture for multichannel live audio.pdf`)

| File | Page | Legacy wording found | Suggested wording in new docs |
|---|---:|---|---|
| 201210 Flexilink...pdf | 3 | Synchronous flow (SF) | Guaranteed service flow (legacy SF) |
| 201210 Flexilink...pdf | 3 | Asynchronous flow (AF) | Basic service flow (legacy AF) |
| 201210 Flexilink...pdf | 4 | AF data in gaps between SF packets | Basic service traffic uses residual capacity between guaranteed allocations |
| 201210 Flexilink...pdf | 4 | variable length SF packets + AF fill | variable guaranteed allocations with basic-service fill |
| 201210 Flexilink...pdf | 5 | AF FIFO / SF FIFO labels | basic-service queue / guaranteed-service queue |
| 201210 Flexilink...pdf | 6 | SF and AF access over link | guaranteed/basic service multiplexing over link |
| 201210 Flexilink...pdf | 7 | AF mapped for normal IP traffic | basic service carries non-deterministic IP traffic |
| 201210 Flexilink...pdf | 7 | separation between AF and SF data | separation between basic and guaranteed service classes |

---

## B) Standards terminology alignment notes

| Standard file | Term note |
|---|---|
| gr_NIN003v010101p.pdf | Uses **Guaranteed service** and **Basic service** explicitly (see p.12). |
| gs_NIN005v010101p.pdf | Uses **control plane** and **signalling flow** explicitly (see p.16). |
| gr_NIN001/gr_NIN002/gs_NIN006 | SF/AF shorthand is not central terminology; keep NIN terms in derivative docs. |

---

## C) Editorial rule (recommended)

For whitepaper/proposal text from now on:
- Prefer: `Guaranteed service`, `Basic service`, `control-plane signalling`
- Keep legacy shorthand only in historical notes:
  - `(legacy SF)`
  - `(legacy AF)`


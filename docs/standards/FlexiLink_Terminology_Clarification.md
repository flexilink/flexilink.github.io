# FlexiLink Protocol Terminology Clarification (SF / AF / Background Traffic)

Based on ETSI NIN documents in `docs/standards`:
- `gr_NIN001v010101p.pdf`
- `gr_NIN002v010101p.pdf`
- `gr_NIN003v010101p.pdf`
- `gs_NIN005v010101p.pdf`
- `gs_NIN006v010101p.pdf`

---

## 1) Authoritative term definitions (practical interpretation)

### Synchronous Flow (SF)
A resource-reserved flow scheduled in specific transmission slots on each traversed link. It is designed for deterministic behaviour (bounded latency + reserved throughput), configured through control-plane flow setup.

### Asynchronous Flow (AF)
A best-effort/basic-service flow with no dedicated slot reservation. Packets are queued/scheduled in the normal forwarding path and can experience jitter, queueing delay, and drop under congestion.

### Background Traffic
Lowest-priority AF/basic-service traffic that consumes residual capacity (including unused SF capacity). It is non-deterministic by design and should not compete with critical signalling/control traffic.

---

## 2) Relationship between SF / AF / Background

- **SF vs AF**: SF is reservation-based and time-structured; AF is queue-based and opportunistic.
- **Background traffic**: a subset/usage class of AF with lower priority.
- **Control-plane signalling**: should be treated separately from background traffic and carried with protected priority.

---

## 3) Engineering use guidance

### Use SF when
- strict delay/jitter bounds are required,
- throughput reservation is required,
- traffic is real-time and predictable (e.g., time-critical media/control paths).

### Use AF when
- traffic is non-real-time or tolerant to delay variation/loss,
- throughput is bursty/opportunistic,
- simplicity/scale matters more than strict determinism.

### Use Background class when
- traffic is non-critical housekeeping/bulk/low-priority transfer,
- utilisation of leftover capacity is desired.

---

## 4) Recommended clean glossary (for internal team docs)

- **SF (Synchronous Flow):**
  "A flow with reserved link resources and scheduled transmission slots, provisioned via control-plane setup for deterministic service."

- **AF (Asynchronous Flow):**
  "A non-reserved best-effort flow delivered through standard queue/scheduler logic without deterministic slot guarantees."

- **Background Traffic:**
  "Low-priority AF traffic using residual capacity; it is delay/loss tolerant and must not pre-empt critical signalling/control traffic."

---

## 5) Minimal operational checklist

- For **SF**:
  - reserve resources end-to-end before data starts,
  - verify timing/synchronisation assumptions,
  - enforce admission control.

- For **AF/Background**:
  - apply queue policies + drop handling,
  - configure ageing for dynamic flow state,
  - prevent starvation of signalling/control traffic.

- For **Control plane**:
  - keep signalling protected and separate from background queues.

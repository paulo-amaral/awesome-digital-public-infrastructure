# 📵 Field Notes - Offline-First & Last Mile

> DPI for contexts where connectivity is the exception, not the rule.

---

- **Design offline-first, not offline-compatible.** There is a difference. Offline-compatible means someone added a sync button after launch. Offline-first means every interaction was designed assuming no connectivity - data queues locally, conflicts are resolved deterministically, and the user never sees a spinner. In fragile and rural contexts, this is the baseline, not an edge case.
- **The last-mile problem is not a technical problem.** In most countries it is already known, costed, and budgeted - and still unresolved after a decade because the economics do not work for private operators and the political will for public investment is absent. Do not design DPI that depends on last-mile connectivity being solved first. Degrade gracefully: offline collection, async sync, SMS fallback, paper backup. The system that works on 2G today delivers more value than the one waiting for fibre in 2030.
- **Test on the actual device.** A form that loads in 2 seconds on Chrome degrades to 45 seconds on a shared Android 8 phone in a municipal office. Test on the hardware your users actually have, in the connectivity conditions they actually face. This single practice eliminates more UX problems than any amount of user research done remotely.

---

← [Back to Field Notes index](README.md)

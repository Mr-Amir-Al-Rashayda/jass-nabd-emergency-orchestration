# Jass Nabd (جس النبض)

**Network-aware emergency orchestration for MENA Ignite 2026 — Prototype Phase.**

Jass Nabd protects an enrolled emergency responder’s command-application link when a high-density operational zone becomes critical. A LangGraph agent selects bounded Nokia Network as Code / CAMARA evidence checks; deterministic policy owns eligibility; and a dispatcher owns the Quality on Demand action.

## Working prototype

- [Open the live demo](https://jass-nabd-command.amir-alrashyda.chatgpt.site/)
- [Watch the 1080p demonstration](https://jass-nabd-command.amir-alrashyda.chatgpt.site/Jass-Nabd-Live-Prototype-Demo-FINAL.mp4)

## APIs demonstrated

- Location Verification
- Device Reachability
- SIM Swap
- Device Swap
- Quality on Demand

## Safety boundary

The language model cannot grant network privileges. A fixed policy checks enrollment, zone membership, packet-data reachability and recent swap risk. Only an eligible run receives a short-lived signed proof, and QoD still requires human approval. Unsafe or unavailable evidence fails closed. Credentials stay server-side.

## Reviewer flow

1. Open the live demo and select **Live APIs**.
2. Run **Golden path · R-17** and inspect the four evidence checks and `ELIGIBLE` result.
3. Run **Blocked path · R-23** and confirm the system returns `BLOCKED` and offers no QoD action.

## Scope

This prototype operates on enrolled or simulated responder devices. It does not claim whole-crowd tracking, and swap signals are treated as risk signals rather than identity proof.

The complete source archive is also attached directly to the HackerEarth Prototype Phase submission.

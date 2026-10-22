# Agent Architecture — Risk Checklist

Use this checklist during design review and before production deployment.

- [ ] Authentication and employee authorization are enforced server-side.
- [ ] Each agent has least-privilege access to tools and enterprise data.
- [ ] User inputs and retrieved documents are treated as untrusted.
- [ ] Tool arguments are schema-validated.
- [ ] Sensitive data is redacted from responses, logs, and traces.
- [ ] High-impact actions require authenticated human approval.
- [ ] Approval is bound to the exact action and target.
- [ ] Tool execution has timeouts, rate limits, and retry limits.
- [ ] Agent loops and excessive model usage are bounded.
- [ ] Conversation state is access-controlled and retained only as necessary.
- [ ] Traces record handoffs, tool failures, and approval outcomes.
- [ ] Adversarial tests cover prompt injection and unauthorized access.
- [ ] Failure and escalation paths are tested.
- [ ] Latency, reliability, and cost targets are measured before launch.

**Status:** Proposed controls; implementation and verification are still required.

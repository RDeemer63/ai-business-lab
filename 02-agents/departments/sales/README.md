# Sales Department

**Mission:** Find and close the first client for each validated business.

**Status:** Dormant — activates only after a business produces a positive validation signal.

## Agents

| Agent | File | Status | Activates when |
|-------|------|--------|----------------|
| Offer & Lead Gen Strategist | `library/agency-agents/sales/sales-offer-lead-gen-strategist.md` | Dormant | Validation signal is positive |
| Pricing Analyst | `library/agency-agents/specialized/specialized-pricing-analyst.md` | Dormant | Offer is being designed |
| Outbound Strategist | `library/agency-agents/sales/sales-outbound-strategist.md` | Dormant | First client outreach begins |
| Proposal Strategist | `library/agency-agents/sales/sales-proposal-strategist.md` | Dormant | First client call is booked |
| Customer Success Manager | `library/agency-agents/specialized/customer-success-manager.md` | Dormant | First client signs |

All Sales agents go dormant again after the first client is onboarded and the delivery workflow is documented.

## Output directory

`04-experiments/[business-name]/` during validation; client files once launched.

## Important constraint

All external communications designed by Sales agents must be approved by Ryan before sending. The Outbound Strategist designs the message. Ryan sends it. This does not change until the studio reaches Phase 3 autonomy.

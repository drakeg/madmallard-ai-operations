# Invoice extraction opportunity experiment

Status: alternative offer hypothesis. No parser or service is implemented. Do not displace the primary agency workflow without DEC-01.

Buyer: independent RV repair shop with manual supplier invoice entry. Pilot price hypothesis: $199 for up to 30 invoices from two layouts. Deliver reviewed CSV fields for vendor, invoice number, date, subtotal, tax, total and source filename, plus duplicate warnings and exceptions. Exclude line items, bookkeeping decisions, accounting imports and payments.

Tool candidate: [Docling](https://github.com/docling-project/docling); [license](https://github.com/docling-project/docling/blob/main/LICENSE). Code was checked as MIT during November 12 research; exact model and dependency licenses need confirmation before use. Local execution is proposed. No customer documents or model downloads are authorized here.

Estimated prototype: 4–6 hours; first batch review: 2–4 hours; incremental startup allowance $0–30. These are estimates, not incurred costs or proven performance.

## Proposed 48 hour validation

Prepare a fictional invoice-to-CSV example and five prospect-selection briefs. In separately authorized customer conversations, ask whether invoice entry is recurring and request redacted representative documents with permission. No outreach is performed by adding this brief.

Go when one buyer accepts the pilot price and representative testing supports accurate review in four delivery hours. Pause when existing tools solve the task, prospects will not pay or review time makes the scope uneconomic. Verify every extracted field against the source; never claim zero-error unattended extraction.

Store only synthetic fixtures in Git if later authorized. Production documents stay in approved client storage. Record actual preparation, review, correction and sales hours before proposing a subscription.

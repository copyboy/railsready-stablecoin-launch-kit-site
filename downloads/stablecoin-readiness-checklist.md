# Stablecoin Payment Readiness Checklist

Use this before launching a USDC/USDT checkout, top-up, settlement, or off-ramp pilot.

This checklist is operational decision support only. It is not legal, tax, financial, investment, custody, or compliance advice.

## 1. Responsibility Matrix

- [ ] Provider owns wallet custody and private key control.
- [ ] Provider owns crypto-side KYC/KYT/AML obligations, if applicable.
- [ ] Merchant/platform owns customer communication and first-line support.
- [ ] Internal ledger owner is named.
- [ ] Finance owner is named.
- [ ] Compliance/legal reviewer is named.

## 2. Provider Evidence

- [ ] Legal entity and service terms collected.
- [ ] Supported jurisdictions confirmed.
- [ ] Supported chains and stablecoins confirmed.
- [ ] Wallet address model documented.
- [ ] Webhook and API lifecycle documented.
- [ ] Refund and failed-payment policy documented.
- [ ] Travel Rule and beneficiary-data requirements documented.

## 3. Payment Intent Design

- [ ] One intent per checkout, invoice, or top-up where appropriate.
- [ ] Amount, currency, chain, expiry, and quote rules defined.
- [ ] Underpay handling defined.
- [ ] Overpay handling defined.
- [ ] Duplicate payment handling defined.
- [ ] Address reuse policy defined.

## 4. Four-Way Reconciliation

Each payment must join:

- [ ] Internal payment intent ID.
- [ ] Chain transaction hash.
- [ ] Provider order / payment ID.
- [ ] Fiat payout / settlement reference.
- [ ] Internal ledger entry.

## 5. Exception Playbook

- [ ] Wrong chain.
- [ ] Wrong token.
- [ ] Underpayment.
- [ ] Overpayment.
- [ ] KYT reject.
- [ ] Quote expiry.
- [ ] Fiat payout delay.
- [ ] Customer refund.
- [ ] Customer says payment was sent but not detected.

## 6. Customer-Facing Copy

Avoid claiming:

- [ ] "We custody your crypto."
- [ ] "We exchange crypto for fiat."
- [ ] "We issue stablecoins."
- [ ] "We are licensed" unless counsel confirms the exact statement.
- [ ] "No risk" or "guaranteed settlement."
- [ ] "Instant" if provider, chain, banking, or risk review can delay settlement.

## 7. Launch Gate

Do not launch until:

- [ ] Provider approval is complete.
- [ ] Legal/compliance review is complete.
- [ ] First test payment reconciles end to end.
- [ ] All exception owners are named.
- [ ] Customer support has approved wording.
- [ ] Limits and pilot customer whitelist are configured.

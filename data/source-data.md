# Source Data (transcribed from the Assignment 3 Data Pack)

Exercise date: **Wednesday, 23 September 2026**.

## Customers

| Name | Tier | PNR | Contact | History |
|---|---|---|---|---|
| Priya Nair | Gold | SK4821X | priya.nair@example.com, +91-98xxxxxxx1 | 6 flights / 12mo, 1 prior complaint (delayed baggage, resolved with voucher) |
| Arvind Kulkarni | Silver | TR1190B | arvind.kulkarni@example.com, +91-98xxxxxxx2 | 3 flights / 12mo, no prior complaints |
| Meher Kaur | Platinum | WL7742 | meher.kaur@example.com, +91-98xxxxxxx3 | 10 flights / 12mo, 1 prior complaint (overbooking, resolved with tier-status upgrade) |

## Bookings

| Customer | PNR | Flight | Route | Date | Scheduled | Status |
|---|---|---|---|---|---|---|
| Priya Nair | SK4821X | SK-204 | Delhi → Goa | Wed 23 Sep 2026 | 18:40 | Cancelled (operational reasons) |
| Priya Nair | SK4821X | Return | Goa → Delhi | Fri 25 Sep 2026 | 16:20 | Unaffected |
| Arvind Kulkarni | TR1190B | SK-118 | Mumbai → Bengaluru | Wed 23 Sep 2026 | 07:10 | Delayed 4h (new departure 11:10) |
| Meher Kaur | WL7742 | SK-305 | Delhi → Hyderabad | Wed 23 Sep 2026 | 14:00 | Delayed 6h (new departure 20:00) |

## Service rules

1. **Cancellation Rebooking Rule** — airline-caused cancellation entitles
   the customer to a free rebooking on the next available flight within
   24 hours, or a full refund — customer's choice.
2. **Delay Compensation Rule** — under 3h: ₹500 meal voucher. Over 3h:
   voucher + lounge access. Over 5h: voucher + lounge access + hotel
   accommodation covering only the delayed hours (not a full night).
3. **Refund Processing Rule** — refunds for airline-caused cancellations
   are processed in full within 7 business days, to the original
   payment method only.
4. **Fare Difference Rule** — a customer voluntarily rebooking onto a
   higher-fare flight (not airline-caused) must pay the fare difference;
   agents cannot waive a difference above ₹1,500 without supervisor
   approval.
5. **Loyalty Tier Rule** — Gold/Platinum get priority rebooking (first
   access to next-available seats), but no additional compensation
   beyond standard policy.

## Allowed actions

- Rebook on next available flight within 24h at no charge (airline-caused)
- Issue meal vouchers and lounge access per the delay rule
- Arrange hotel accommodation for the delayed-hours portion, where qualified
- Initiate a refund for airline-caused cancellations
- Provide the customer's own booking / flight status information

## Prohibited actions (must escalate)

- Approving compensation beyond the stated policy amounts
- Waiving a fare difference above ₹1,500
- Making exceptions for non-airline-caused disruptions
- Handling threats of legal action or formal complaints — escalate immediately
- Processing refunds to a different payment method than the original

## Scenarios used to validate the agent

- **Priya Nair (Gold, SK4821X)** — cancelled flight; mid-conversation
  goes "furious" and asks for a full cash refund plus a free business
  upgrade on the return flight.
- **Arvind Kulkarni (Silver, TR1190B)** — 4h delay; asks for hotel
  accommodation "since it's been such a long delay."
- **Meher Kaur (Platinum, WL7742)** — 6h delay; asks for a full night's
  hotel stay instead of delayed-hours-only coverage, and separately asks
  to switch to a different, higher-fare flight (₹2,000 fare difference).

Note: the data pack's "sample prior conversations" (Samples A–C) are
*other, unrelated customers* included only to show agent tone and style.
They were used only as a style reference, never as policy or fact.
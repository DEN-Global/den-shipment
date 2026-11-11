# DEN Shipment

API-connected domestic shipment quotation preparation workspace. Uses centralized DEN sessions and `/api/mobility`.

Run `npm install`, `npm test`, `npm run build`; the shared backend dev server serves `/shipment/`. Requests persist in the PostgreSQL-backed platform database and are scoped to their authenticated owner. Cancellation is audited. Cross-border requests enforce the global trade lock; enabled trade still requires carrier and compliance integration.

Implemented: saved domestic quotation requests, history, cancellation, input validation, idempotency and parcel weight and road/air/sea preparation. Not implemented: live quotes, route/fare calculation, provider bookings, driver approval, verified trips, carrier handoff, payments or live GPS. No real price or booking is implied.

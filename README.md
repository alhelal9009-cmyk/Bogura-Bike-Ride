# Bogura Bike Ride — Full Setup v0.2

এই সংস্করণে আলাদা Passenger, Rider এবং Admin interface-এর পূর্ণ UI flow আছে।

## বাস্তব/Production করার জন্য এখনও যেগুলো যুক্ত করতে হবে
- Secure backend + database
- OTP/SMS authentication
- Password hashing/session security
- Google Maps + live GPS
- Nearby rider matching
- Ride state machine (requested/accepted/started/completed/cancelled)
- Push notification
- Real bKash/Nagad merchant/business payment integration
- Admin-side payment verification
- Secure NID/document storage and access control
- SOS backend, live location, emergency contact notification
- Call/SMS/999 integration
- Fare engine and admin-configurable zones
- Audit logs, fraud prevention, rate limiting
- Privacy policy, terms, consent and data retention
- BRTA/legal compliance review before public launch

ADMIN_PAYMENT_NUMBER is intentionally a placeholder; owner's personal payment number should not be hard-coded into the app source.

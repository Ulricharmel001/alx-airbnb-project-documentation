# Use Case Diagram - ALX Airbnb Backend System

## Actors
- Guest (Visitor)
- Host (Registered User)
- Admin
- Payment Gateway (External)
- Email Service (External)

## Key Relationships
- `Book Property <<include>> Login`
- `Book Property <<include>> Make Payment`
- `Make Payment <<include>> Process Payment`
- `Make Payment <<extend>> Send Notification`
- `Verify Host <<extend>> Manage Users`
- `Register <<extend>> Send Notification`
- `Add Property <<include>> Upload Images`

etc...

![Use Case Diagram](./AIRBNB%20USE%20CASE.png)

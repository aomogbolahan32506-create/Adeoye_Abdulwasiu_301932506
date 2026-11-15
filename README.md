## Database Tables & Schema Structure

For the **Grand Apex Hotel & Suites** case study, the relational database is structured into four core tables:

| Table Name | Primary Key | Foreign Key(s) | Key Attributes | Description |
| :--- | :--- | :--- | :--- | :--- |
| **Guests** | `guest_id` | None | `first_name`, `last_name`, `email`, `phone_number` | Stores personal information and contact details for all hotel guests. |
| **Rooms** | `room_id` | None | `room_number`, `room_type`, `price_per_night`, `status` | Maintains inventory of hotel rooms, types, pricing, and availability status. |
| **Bookings** | `booking_id` | `guest_id`, `room_id` | `check_in_date`, `check_out_date`, `total_amount`, `booking_status` | Manages guest reservations, stay duration, and booking lifecycle states. |
| **Payments** | `payment_id` | `booking_id` | `amount_paid`, `payment_method`, `payment_date` | Tracks financial transactions and payment logs linked to specific bookings. |

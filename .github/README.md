# Mori-PMS

Hotel & Hospitality Management System: point of sale, kitchen and bar order routing, stock control, front desk, revenue management, reports, staff and role administration, and GDS bookings with commission tracking.

## Modules

- **POS**: waiters take orders by table; cashiers close sales; Manager and Super Admin can void.
- **Orders**: each order splits into a Kitchen ticket and a Bar ticket; departments mark orders Preparing, Ready and Served; tickets and receipts can be printed.
- **Stock**: live stock levels deducted per order, reorder alerts, receiving stock.
- **Front desk**: room check-in and check-out, occupancy chart.
- **Revenue and Reports**: daily, monthly and yearly sales reports, downloadable as CSV or a printable report.
- **GDS**: flight and vehicle bookings with commission.
- **Business day**: business date, backdated closing of unclosed orders.
- **Settings**: menu and prices, rooms by type, GDS rates, printing and routing.
- **Staff & admin**: register and remove Super Admin, Admin, Manager, Accountant, Supervisor, Cashier, Waiter/Waitress, Receptionist, Kitchen and Bar users (4-digit PIN sign-in).

## Run it

It is a single static file. Open `index.html` in a browser, or host the repository with GitHub Pages (Settings, Pages, deploy from the `main` branch).

Demo sign-ins (change these before real use): Super Admin 1234, Manager 1111, Cashier 2222, Waiter 3333, Accountant 4444, Supervisor 5555.

## Storage

Data is kept in the browser (`localStorage`) on each device. When the app runs inside Claude as a published artifact with its shared database enabled, orders, tickets and settings sync across tablets. Hosted on its own (for example GitHub Pages), each device keeps its own separate data, so a waiter's tablet will not send orders to the kitchen tablet. For multi-device use outside Claude, replace the storage layer with a backend of your choice.

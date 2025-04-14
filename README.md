Java-POTS-Project
Java Procurement Order Tracking System Description POTS is a console‑based Java application that automates and manages the full lifecycle of purchase orders. It provides a menu‑driven interface for multiple user roles to handle inventory, sales, requisitions, orders, and payments—using simple text files for data storage.

Features User Authentication & Roles

Login with username/password

Five roles with distinct permissions:

Administrator: create and manage all users

Sales Manager: record daily sales, view stock, create purchase requisitions, view PRs and POs

Purchase Manager: view requisitions, generate/edit/approve/reject purchase orders, view PO list

Inventory Manager: add/edit/delete items and suppliers, view/update stock levels

Finance Manager: verify and approve payments for POs, track supplier payment status

Inventory & Supplier Management

Maintain master lists of items and suppliers

Prevent duplicate entries

Persist data in items.txt and suppliers.txt

Sales Entry & Stock Updates

Enter daily, item‑wise sales

Automatically adjust stock levels

Purchase Requisitions (PR)

Create PRs when stock falls below reorder thresholds

Assign unique PR IDs and capture requester information

View all existing requisitions

Purchase Orders (PO)

Generate POs based on approved PRs

Assign unique PO IDs and capture creator information

Edit, approve, or reject orders

View PO history

Payment Processing

Finance Manager can mark POs as paid or unpaid

View payment history by supplier

Data Persistence

All records (users, items, suppliers, requisitions, orders) are stored in plain text files for easy inspection and backup

Getting Started Download as ZIP On the GitHub repository page, click the Code button and select Download ZIP.

Extract the downloaded archive (e.g. POTS-master.zip) to a local directory.

Open a terminal and navigate into the extracted folder:

bash Copy cd POTS-master Or Clone the Repository bash Copy git clone https://github.com/your‑username/pots.git cd pots Compile bash Copy javac src/*.java Run bash Copy java src.Main Data Files As you use the system, the following text files will be created or updated automatically in the data/ directory:

users.txt

items.txt

suppliers.txt

requisitions.txt

orders.txt

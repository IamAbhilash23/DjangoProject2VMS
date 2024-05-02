Django REST API and Django Frameworks Setup
This repository contains a Django project2 with a RESTful API using Django REST Framework.

Prerequisites
Python (version 3.x recommended)
Django
Django REST Framework

Setup Instructions:

Create a Virtual Environment:
-py -m venv myproject
-myproject\Scripts\activate.bat

Install Dependencies:
-pip install Django
-pip install djangorestframework

To get started with the Vendor Management System API, follow these steps:

-Clone the repository
-After cloning you will find myproject folder compile the folder in the respective editor
-Now by moving into the specific folder have to run the server using the command "py manage.py runserver"
---by making cd myproject/v_m_s

Create superuser:
Superuser creation and Token generation
command:python manage.py createsuperuser

How to run a api endpoint:
first we need to make sure that we migrated the models to database
then we need to start the server using "python manage.py runserver" command.
then we need to open another cmd prompt and open virtual environment and open the project folder.

API Endpoints:
By opening chrome with the specific IP and port no.which we can see in the cmd after running server
Navigate to http://127.0.0.1:8000/vms_app/vendors/
Create a vendor:
● Create a store vendor information including name, contact
details, address, and a unique vendor code.
  -name:abc
  -contact:987456123
  -details:heuide dein
  ......
  -we can create as many as vendor profiles as we need
Retrieve a specific vendor's details:
-we can list of each vendor details by moving to http://127.0.0.1:8000/vms_app/vendors/vendor_id/

Navigate to http://127.0.0.1:8000/vms_app/vendors/purchase_orders/
Create a purchase_orders:
● Create purchase_orders including the fields like PO number, vendor reference,
order date, items, quantity, and status
  PO number:45621
  vendor reference from vendor profile
  ....
Retrieve a specific purchase_order's details:
-we can list of each vendor details by moving to http://127.0.0.1:8000/vms_app/vendors/purchase_orders/po_number

Update a purchase_order's details:
-we can do it from the above path "http://127.0.0.1:8000/vms_app/vendors/purchase_orders/po_number" and post

Update acknowledgment_data:
Navigate to "purchase_orders/po_number/acknowledge/"

Vendor Performance:
http://127.0.0.1:8000/vms_app/vendors/vendor_id/performance/
we can know performance of each vendor based on the purchase orders







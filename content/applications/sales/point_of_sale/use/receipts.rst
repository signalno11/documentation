.. _pos/configuration/receipts:

========
Receipts
========

+----------------------------------------------------------+---------------------------------+
| POS receipts display the following elements:             |                                 |
|                                                          |                                 |
| - The company logo                                       | .. image:: receipts/receipt.png |
| - The receipt and order number                           |                                 |
| - The customizable header and footer                     |                                 |
| - The name of the cashier and the customer               |                                 |
|   (provided a customer was :ref:`set for the order       |                                 |
|   <pos/use/customers>`)                                  |                                 |
| - The complete order, discounts, prices, and used        |                                 |
|   payment methods                                        |                                 |
| - Optionally, a QR code or URL link for customers to     |                                 |
|   generate :doc:`invoices <pos_invoices>`                |                                 |
+----------------------------------------------------------+---------------------------------+

.. _pos/configuration/receipt-configuration:

Configuration
=============

To set up POS receipts, go to :menuselection:`Point of Sale --> Configuration --> Settings`, and
scroll down to the :guilabel:`Bills & Receipts` section.

- To customize the header and footer, enable the :guilabel:`Header & Footer` setting and enter the
  information to be printed on the receipts in both fields.
- To print receipts automatically upon payment confirmation, enable the :guilabel:`Automatic
  Receipt Printing` setting.
- To print receipts that don't display product prices, enable the :guilabel:`Basic Receipt` setting.
- Receipts can be sent by default via email, or by SMS or or WhatsApp. To do so, activate the
  :guilabel:`SMS Enabled` or :guilabel:`WhatsApp Enabled` option(s).

  .. note::
     The :guilabel:`WhatsApp Enabled` setting is only available if the :guilabel:`WhatsApp
     Messaging` module is :ref:`installed <general/install>`.

.. seealso::
   - :ref:`pos/restaurant/bills`
   - :doc:`pos_invoices`
   - :doc:`../hardware_network/receipt_printers`

.. _pos/configuration/receipt-reprint:

Receipt reprint
===============

To reprint a receipt, follow the next steps:

#. Access the :ref:`POS interface <pos/use/open-register>`.
#. Click :guilabel:`Orders`.
#. Open the dropdown selection menu next to the search bar, and change the default :guilabel:`All
   active orders` filter to :guilabel:`Paid`.
#. Select the order and click :guilabel:`Print Receipt`.

.. tip::
   Filter the list of orders using the search bar: type in your reference and select
   :guilabel:`Receipt Number`, :guilabel:`Date`, or :guilabel:`Customer`.

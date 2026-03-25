=======
Cashdro
=======

**Cashdro** :doc:`cash machines <../cash_machines>` enable the automation of cash transactions.

.. note::
   - The integration with the Cashdro cash machine only supports payments and refunds.
   - Tasks like filling and emptying the machine must be performed directly through the cash
     machine interface.

.. _pos/cashdro/configuration:

Cash machine configuration
==========================

.. important::
   - Setting up the Cashdro machine requires the Cashdro hardware administrator password and
     technical knowledge. If needed, consult the Cashdro integration partner for configuration
     support.
   - The IP address should be static to ensure long-term stable operation.

Configuring the Cashdro machine as a :ref:`payment method in Odoo <pos/cashdro/odoo_configuration>`
requires locating its IP address and enabling HTTP on the cash machine to use :doc:`Local Network
Access (LNA) <../../hardware_network/pos_lna>`.

To locate the Cashdro machine's IP address, remove one of the devices inside the machine. For
example, remove the bill device on the left side of the machine by unlatching it from the bottom
and sliding it out. This action displays a diagnostics screen with the IP address, which is required
for the :ref:`payment method process <pos/cashdro/odoo_configuration>`.

To enable the HTTP setting on the Cashdro machine, follow the next steps:

#. Navigate to the login screen at `https://<cashdro-ip>/Cashdro3Web/#/login`.
#. Log in as the support user.
#. Navigate to :menuselection:`Configuration --> General parameters`.
#. Ensure :guilabel:`Enable HTTP` is checked in the :guilabel:`Web Integration` section.
#. Restart the machine.

.. note::
   Make sure to reconnect any device that is removed.

.. _pos/cashdro/odoo_configuration:

Odoo configuration
==================

To connect the Cashdro machine with Odoo, follow the next steps:

#. :ref:`Install <general/install>` the :guilabel:`POS Cashdro Cash Machines` module.
#. Go to :menuselection:`Point of Sale --> Configuration --> Payment Methods`, and click
   :guilabel:`New` to create a :doc:`payment method <../../payment_methods>`.
#. Set the :guilabel:`Journal` field to :guilabel:`Cash`.
#. Select the associated POS in the :guilabel:`Point of Sale` field.
#. Set the :guilabel:`Integration` field to :guilabel:`Cash Machine (Cashdro)`.
#. Type the Cashdro machine's IP address in the :guilabel:`Cashdro IP` field under the
   :guilabel:`Cashdro Settings` tab.
#. Type your Cashdro user credentials in the :guilabel:`Cashdro Username` and
   :guilabel:`Cashdro Password` fields.
#. Enable the :guilabel:`Cashdro Local Network Access` checkbox.

.. note::
   It is highly recommended to use the :doc:`Local Network Access <../../hardware_network/pos_lna>`
   setting, as it bypasses the need for an :doc:`SSL certificate <../../hardware_network/epos_ssc>`.

.. seealso::
   :doc:`../../payment_methods`

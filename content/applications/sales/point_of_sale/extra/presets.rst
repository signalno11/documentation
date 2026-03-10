=======
Presets
=======

Presets are preconfigured settings used to quickly apply predefined configurations during sales,
primarily to speed up order entry and reduce manual steps. They also control whether customer
contact information is required and apply capacity limits based on opening hours and order quantity.

.. admonition:: Use

   Presets are useful for businesses that need different configurations depending on the type of
   sale. They can automatically apply specific fiscal positions, pricelists, or opening hours.

   For example:

   - Restaurants use presets to adjust pricelists and capacities based on the order type, such as
     :guilabel:`Dine In`, :guilabel:`Takeaway`, or :guilabel:`Delivery`.

   - Flower shops use presets to apply different taxes when selling flowers and plants (taxed as
     goods) versus creating arrangements for funerals or weddings (taxed as services). Presets can
     also help streamline returns and apply discounts for loyal customers.

.. seealso::
   `Odoo Presets Tutorial <https://www.odoo.com/slides/slide/manage-presets-12827>`_

.. _pos/restaurant/orders/preset/backend:

To configure POS presets, follow these steps:

#. Go to the :ref:`POS settings <pos/use/settings>`.
#. Under the :guilabel:`Point of Sale` section, enable the :guilabel:`Take out / Delivery / Members`
   setting.
#. Select preconfigured presets or :guilabel:`Create and edit` new ones in the :guilabel:`Available`
   field.
#. Define a default preset in the :guilabel:`Default` field.
#. Click :guilabel:`Save`.
#. Click :icon:`oi-arrow-right` :guilabel:`Configure Presets`, then select the desired preset or
   click :guilabel:`New`.

.. tip::
   - To quickly access presets, go to :menuselection:`Point of Sale --> Configuration --> Presets`.
   - Presets are not automatically enabled, except when creating a new point of sale through the
     onboarding screen and selecting the :guilabel:`Restaurant` option.

On the relevant :guilabel:`Presets` form, apply or edit the following options:

- :guilabel:`Pricelist`: Select or :doc:`configure a pricelist
  </applications/sales/sales/products_prices/prices/pricing>`.
- :guilabel:`Fiscal Position`: Select or :doc:`configure a fiscal position
  </applications/finance/accounting/taxes/fiscal_positions>`. Fiscal positions are especially
  important in environments where customers must pay different tax rates depending on the type of
  order.
- :guilabel:`Manage orders by time`: Enable this option to define time slots for scheduling orders.
  Then,

  - choose a working time in the :guilabel:`Schedule based on` field;
  - define the :guilabel:`Preparation capacity` to indicate how many orders can be handled in a
    given time frame;
  - configure the working hours on the :guilabel:`Schedule` tab.

- :guilabel:`Identification`: Specify whether identification details (such as a :guilabel:`Name`
  or an :guilabel:`Address`) are required.
- :guilabel:`Return mode`: Select this mode only to process returns. All items added to the cart
  are entered as negative quantities.
- :guilabel:`Color`: Define the preset button's color in the :ref:`register
  <pos/restaurant/orders>`.

It is also possible to display presets in the :doc:`self-order interface <self_order>`. To do so,
navigate to the :guilabel:`Self Ordering` tab and enable :guilabel:`Available in self`. Select a
service zone in the :guilabel:`Service at` field and select or :doc:`configure an email template
</applications/general/companies/email_template>` in the :guilabel:`Email Confirmation` field.

In the :guilabel:`Options` tab, select :guilabel:`Guest` to force guest selection when :ref:`taking
an order <pos/restaurant/orders>`.

.. note::
  - The :guilabel:`Schedule` tab only appears when the :guilabel:`Manage orders by time` option is
    enabled.
  - The :guilabel:`Service at` and :guilabel:`Email Confirmation` fields only appear when the
    :guilabel:`Available in self` option is enabled in the :guilabel:`Self Ordering` tab.

.. tip::
   On the preset form, click the :icon:`fa-shopping-cart` :guilabel:`Order(s)` smart button to
   access an overview of all orders for the selected preset.

.. example::
   In your restaurant’s settings, the default preset is :guilabel:`Dine In`, since most customers
   eat on-site. However, you also offer takeout. If a customer wants to take their meal away, click
   the :guilabel:`Dine In` default preset in the :ref:`POS register <pos/restaurant/orders>` to
   view the available alternatives.

   .. image:: presets/presets-button.png
      :alt: Default presets "Dine In" button.

   Select :guilabel:`Takeout`, enter the customer’s name, and click :guilabel:`Apply`. Depending on
   the preset configuration, you may also need to choose a date and time before clicking
   :guilabel:`Continue`. For the next order, the system automatically resets to the default preset.

.. seealso::
  - :doc:`preparation`
  - :doc:`../restaurant/online_food_delivery`

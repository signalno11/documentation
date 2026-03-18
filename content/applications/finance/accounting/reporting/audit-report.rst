============
Audit report
============

Audit reports document annual financial performance, operational challenges, and organizational
achievements for stakeholder review.

Odoo :ref:`generates annual reports <accounting/audit-report/creation>` from pre-configured
templates. Users can :ref:`edit and customize <accounting/audit-report/audit-report-edition>`
content, :ref:`add sections, pages, or attachments <accounting/audit-report/additional-documents>`,
and :ref:`export the report as a PDF <accounting/audit-report/export>` for distribution.

.. note::
   Audit reports are stored in the creator's :guilabel:`Private` category of the :doc:`Knowledge app
   <../../../productivity/knowledge>` and follow the same structure.

.. _accounting/audit-report/creation:

Audit report creation
=====================

To create an audit report, follow these steps:

#. Go to :menuselection:`Accounting --> Review --> Annual Report` and click :guilabel:`New`.
#. In the :guilabel:`Create an Audit Report` window, enter a :guilabel:`Title` and set the
   :guilabel:`Dates`.
#. Update the :guilabel:`Responsibles` field, if needed.
#. Click :guilabel:`Save`.

A :guilabel:`Draft` audit report card is then created in the :guilabel:`Audit Reports` Kanban view.
Click the card to open the audit report displayed in the :guilabel:`Private` category of the sidebar
tree.

.. tip::
   To modify the audit report's configuration, click the :icon:`fa-ellipsis-v` :guilabel:`(vertical
   ellipsis)` icon of the card and select :guilabel:`Configure`.

.. _accounting/audit-report/audit-report-edition:

Audit report edition
====================

Audit reports contain articles that can be edited or deleted.

In the sidebar tree, hover over the new audit report. Click the :icon:`fa-caret-right`
:guilabel:`(right arrow)` icon to display the different sections:

- :guilabel:`Attestation`: Activate the :icon:`fa-toggle-off` :guilabel:`(toggle-off)` icons to show
  or hide attestations containing dynamic text. Dates and company values are automatically updated
  when the final report is generated.

  .. note::
     - Only attestations with the toggle enabled are included in the final PDF report.
     - Attestations can be :doc:`signed <../../../productivity/sign>` electronically.

- :guilabel:`Balance Sheet`: Click to customize the balance sheet using filters and options that
  are saved in the :ref:`exported PDF report <accounting/audit-report/export>`.
- :guilabel:`Profit and Loss`: Click to customize the profit and loss report, using filters and
  options that are saved in the :ref:`exported PDF report <accounting/audit-report/export>`.
- :ref:`Annexes <accounting/audit-report/additional-documents>`
- :ref:`Supporting Documents <accounting/audit-report/additional-documents>`

.. tip::
   - Articles can be created from :ref:`a template <knowledge/articles_editing/from-template>` or
     from scratch, clicking the :icon:`fa-plus` :guilabel:`(plus)` icon.
   - To delete articles or sections from the audit report, drag and drop them into :icon:`fa-trash`
     :guilabel:`Open the Trash`.
   - Drag and drop any articles or sections from the sidebar tree to move them directly.

When clicking the audit report in the sidebar tree, a detailed view is displayed:

- To reorder the articles, click and drag them using the :icon:`oi-draggable` :guilabel:`(drag
  handle)` icon.
- To delete sections or articles, hover over the item and click the :icon:`fa-trash`
  :guilabel:`(trash)` icon.

.. _accounting/audit-report/additional-documents:

Additional documents
--------------------

In the :guilabel:`Annexes` section, additional templates can be added to the audit report.

- Click :guilabel:`Load a Template` to view extra templates not included by default: select a
  template in the list, complete the sections, disable the :icon:`fa-toggle-on`
  :guilabel:`(toggle-on)` icons to hide parts that are not needed, and click :guilabel:`Load
  Template`.
- Click :guilabel:`Add an Article` to add a blank article to complete.

In the :guilabel:`Supporting Documents` section, upload files to include in the audit report.

.. _accounting/audit-report/export:

Audit report export
===================

To export the audit report as a PDF, follow these steps:

#. Select the audit report in the sidebar tree.
#. Click the :icon:`fa-ellipsis-v` :guilabel:`(vertical ellipsis)` icon in the top-right corner and
   select :icon:`fa-file-pdf-o` :guilabel:`Download Annual Report`.
#. In the :guilabel:`Download Annual Report` window, disable the :icon:`fa-toggle-on`
   :guilabel:`(toggle-on)` icons to exclude sub-articles and PDF Files, if needed.
#. Click “Download PDF”.

Alternatively, go back to the :guilabel:`Audit Reports` Kanban view and click :guilabel:`Print` on
the audit report card. This option includes sub-articles and PDF files by default.

.. tip::
   The logo configured in the :ref:`company form <general/companies/company>` is displayed on the
   cover page of the audit report.

To mark an audit report as :guilabel:`Done` or delete it, go to :menuselection:`Accounting
--> Review > Annual Report`, click the :icon:`fa-ellipsis-v` :guilabel:`(vertical ellipsis)` icon on
the report card, and select :guilabel:`Set to Done` or :guilabel:`Delete`, respectively.

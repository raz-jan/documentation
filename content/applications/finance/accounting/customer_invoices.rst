:show-content:

=================
Customer invoices
=================

A customer invoice is a document issued by a company for products and/or services sold to a
customer. It records receivables as they are sent to customers. Customer invoices can include
amounts due for the goods and/or services provided, applicable sales taxes, shipping and handling
fees, and other charges.
Odoo supports multiple invoicing and payment workflows.

.. seealso::
   - :doc:`/applications/finance/accounting/customer_invoices/overview`

From draft invoice to profit and loss report, the process involves several steps once the goods or
services are ordered or shipped to a customer, depending on the invoicing policy:

- :ref:`accounting/invoice/creation`
- :ref:`accounting/invoice/confirmation`
- :ref:`accounting/invoice/sending`
- :ref:`accounting/invoice/paymentandreconciliation`
- :ref:`accounting/invoice/followup`
- :ref:`accounting/invoice/reporting`

.. note::
   Odoo :guilabel:`Invoicing` is a standalone app designed to create invoices, send them to
   customers, and manage payments. It also handles flows involving vendor bills. On the other hand,
   the :guilabel:`Accounting` app is a comprehensive accounting solution that allows the same
   actions and includes additional features such as standard financial reports, bank reconciliation,
   budget, asset management, and more.

.. _accounting/invoice/creation:

Invoice creation
================

Draft invoices can be directly created from documents like sales orders or purchase orders or
manually from the :guilabel:`Customer Invoices` journal in the :guilabel:`Accounting Dashboard`.

An invoice must include the required information to enable the customer to pay promptly for their
goods and services. Make sure the following fields are appropriately completed:

- :guilabel:`Customer`: Odoo automatically pulls information like the invoice address, preferred
  :doc:`payment terms <customer_invoices/payment_terms>`,
  :doc:`fiscal positions <taxes/fiscal_positions>`, receivable account, and more from the customer
  record onto the invoice when a customer is selected.
- :guilabel:`Invoice Date`: is either filled in automatically on confirmation or can be set
  manually.
- :guilabel:`Due Date` or :doc:`payment terms <customer_invoices/payment_terms>`: to specify when
  the customer has to pay the invoice.
- :guilabel:`Journal`: is automatically set and can be changed if needed.
- :doc:`Currency <get_started/multi_currency>`
- :guilabel:`Product`
- :guilabel:`Quantity`
- :guilabel:`Price`
- :doc:`Taxes <taxes>` (if applicable)

.. tip::
   To display the total amount of the invoice in words, go to :menuselection:`Accounting -->
   Configuration --> Settings` and activate the :guilabel:`Total amount of invoice in letters`
   option.

The :guilabel:`Journal Items` tab displays the accounting entries created.
Specific invoice/accounting information such as the :guilabel:`Customer Reference`,
:doc:`Fiscal Positions <taxes/fiscal_positions>`, :doc:`Incoterms <customer_invoices/incoterms>`,
and more can be added or modified in the :guilabel:`Other Info` tab.

Odoo initially creates invoices in :guilabel:`Draft` status. While they remain unvalidated, draft
invoices have no accounting impact.

.. seealso::
   - :doc:`/applications/sales/sales/invoicing/proforma`

.. _accounting/invoice/confirmation:

Invoice confirmation
====================

Click :guilabel:`Confirm` when the document is completed. The document's status changes to
:guilabel:`Posted`, and a journal entry is generated based on the invoice configuration. On
confirmation, Odoo assigns each document a unique number from a defined
:ref:`sequence <accounting/invoice/sequence>`.

.. note::
   - Once confirmed, an invoice can no longer be updated. Click :guilabel:`Reset to draft` if
     changes are needed.
   - If required, invoices and other journal entries can be locked once posted
     using the :ref:`Lock posted entries with hash <data-inalterability/lock>` feature.

.. _accounting/invoice/sending:

Invoice sending
===============

To send the invoice to the customer, click :guilabel:`Send & Print`. A :guilabel:`Configure your
document layout` pop-up window will appear if a :ref:`default invoice layout
<studio/pdf-reports/default-layout>` hasn't been customized. Then, select the ways to send this
invoice to the customer in the :guilabel:`Send` window.

To send and print multiple invoices, go to the list view and select them. In the :icon:`fa-cog`
:guilabel:`Actions` menu, select the :guilabel:`Send & Print` option. A banner will appear on the
selected invoices to indicate they are part of an ongoing send and print batch. This helps prevent
the process from being triggered manually again, as it may take some time to complete for
exceptionally large batches.

.. _accounting/invoice/paymentandreconciliation:

Payment and reconciliation
==========================

In Odoo, an invoice is considered :guilabel:`Paid` when the associated accounting entry has been
reconciled with the payment entries.

.. seealso::
   - :doc:`payments`
   - :doc:`bank/reconciliation`

.. _accounting/invoice/followup:

Payment follow-up
=================

Odoo helps define a :doc:`follow-up <payments/follow_up>` strategy. Different actions can be set up
to remind customers to pay their outstanding invoices, depending on how much the customer is
overdue. These actions are bundled into follow-up levels that trigger when an invoice is overdue by
a certain number of days. If there are other overdue invoices for the same customer, the actions are
performed on the most overdue invoice.

.. _accounting/invoice/followup-reports:

Follow-up Reports
-----------------

To set the different follow-up levels, go to
:menuselection:`Accounting --> Configuration --> Follow-up Levels`. All actions triggered after a
specified number of days can be viewed. To manage the various options, such as the number of days,
the type of reminder sent, or whether the action is automated, click on the specific line that needs
to be updated.

Then, follow these steps to take the appropriate action:

- To access the list of customers requiring action along with the :guilabel:`Total Due` and
  :guilabel:`Total Overdue` amounts, go to
  :menuselection:`Accounting --> Customers --> Follow-up Reports`.
- To get a full overview of the customer's open invoices, click on its line.
- To open a payment reminder to be sent to the customer, click the :guilabel:`Follow up` button.
- To exclude any invoices from the follow-up, enable the option :guilabel:`Exclude from Follow-ups`
  for the selected ones.

.. _accounting/invoices/aging-report:

Aged Receivable
---------------

To review outstanding customer invoices and their related due dates, use the
:ref:`Aged Receivable <accounting/reporting/aged-receivable>` report. To access it, go to
:menuselection:`Accounting --> Reporting --> Aged Receivable`.

.. _accounting/invoice/reporting:

Reporting
=========

Profit and Loss
---------------

The :ref:`Profit and Loss <accounting/reporting/profit-and-loss>` statement shows details of income
and expenses.

Balance sheet
-------------

The :ref:`Balance Sheet <accounting/reporting/balance-sheet>` summarizes the company's liabilities,
assets, and equity at a specific time.

.. _accounting/invoice/sequence:

Sequence
========

The sequence that Odoo assigns to each document is a unique number made up of a prefix and a number.
The prefix combines the journal code and the entry date. It is used to classify entries by period.
The number is unique for each period and is used to identify the entry. The default sequence on
customer invoices is INV/YYYY/number. In some specific cases,
:ref:`resequencing <accounting/invoice/resequencing>` might be necessary.

.. _accounting/invoice/resequencing:

Resequencing
------------

:guilabel:`Resequence` is a technical feature used to change the sequence of documents. It can be
helpful to resequence invoice numbers when importing invoices from another invoicing or accounting
system, mainly if the reference originates from the previous software and continuity for the current
year must be maintained without restarting from the beginning.

The sequence can be modified once an invoice is in Odoo.

.. note::

   - This feature is only available to users with administrator or advisor access.
   - All sequence changes are logged in the chatter to keep the information.
   - Sequence changes also affect the format of future invoices' sequence.

Follow these steps to resequence invoice numbers:

#. Activate the :ref:`developer mode <developer-mode>`.
#. From the :guilabel:`Accounting Dashboard`, open the :guilabel:`Customer Invoices` journal.
#. Select the documents that need a new sequence.
#. In the :icon:`fa-cog` :guilabel:`Actions` menu, click :guilabel:`Resequence`.
#. In the :guilabel:`Ordering` field, choose to

   - :guilabel:`Keep current order`: The order of the numbers remains the same.
   - :guilabel:`Reorder by accounting date`: The number is reordered by accounting date.
#. Set the :guilabel:`First New Sequence`.
#. :guilabel:`Preview Modifications` and click :guilabel:`Confirm`.

.. image:: customer_invoices/invoice-sequencing.png
   :alt: Resequence options window

In some cases, resequencing is not possible:

- When entries are before a lock date.
- When the sequence leads to a duplicate.
- When the :guilabel:`Invoice Date` doesn't match the date contained in the new sequence number.

  .. example::
     If the sequence is changed to INV/2023/XXXXX for a document with an :guilabel:`Invoice Date` of
     2024.

.. toctree::
   :titlesonly:

   customer_invoices/overview
   customer_invoices/customer_addresses
   customer_invoices/payment_terms
   customer_invoices/terms_conditions
   customer_invoices/cash_discounts
   customer_invoices/credit_notes
   customer_invoices/cash_rounding
   customer_invoices/deferred_revenues
   customer_invoices/electronic_invoicing
   customer_invoices/snailmail
   customer_invoices/epc_qr_code
   customer_invoices/incoterms

.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
   :alt: License: AGPL-3

=======================
Donation Bank Statement
=======================

This module is designed to handle donation received by credit transfer.
After the import of the bank statement, you can start a wizard that will
create a donation for each unreconciled bank statement lines affected to
a particular account.

Configuration
=============

To configure the module, you have to create a bank journal dedicated to
donations via credit transfer, that will have a special transfer account
as default debit/credit account. Then, on the company, you must select
this journal as the *Donations via Credit Transfer Journal*.

Usage
=====

To use the module, you should import your bank statement as usual.
During the reconciliation step, when you have a donation by credit
transfer, you should set the account that you used as default
debit/credit account on the journal dedicated for donations via credit
transfer. Once your bank statement is closed, you should click on the
button *Create Donations*, which will create draft donations linked
to the related bank statement line. When these draft donations are
validated, it will create the corresponding account move and reconcile
it with the account move of the bank statement.

Hint: for a faster processing of the bank statement, you can create a *Statement Operation Template* dedicated to the Donations via Credit Transfer in the menu Accounting > Configuration > Miscellaneous > Statement Operation Template. This statement operation template will be configured with the account corresponding to the donations via credit transfer.

.. image:: https://odoo-community.org/website/image/ir.attachment/5784_f2813bd/datas
   :alt: Try me on Runbot
   :target: https://runbot.odoo-community.org/runbot/180/10.0

Bug Tracker
===========

Bugs are tracked on `GitHub Issues
<https://github.com/OCA/donation/issues>`_. In case of trouble, please
check there if your issue has already been reported. If you spotted it first,
help us smashing it by providing a detailed and welcomed feedback.

Credits
=======

Contributors
------------

* Brother Bernard <informatique - at - barroux.org>
* Brother Irénée (Barroux Abbey)
* Alexis de Lattre <alexis.delattre@akretion.com>

Maintainer
----------

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit https://odoo-community.org.

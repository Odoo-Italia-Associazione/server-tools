.. image:: https://img.shields.io/badge/license-AGPL--3-blue.png
   :target: https://www.gnu.org/licenses/agpl
   :alt: License: AGPL-3

===============
Onchange Helper
===============

This is a technical module. Its goal is to ease the play of onchange method directly called from Python code.

Usage
=====

To use this module, you need to:

* depend on this module
* call `yourmodel.play_onchanges(values, ['field'])`

Example if you want to create a sale order and you want to get the values relative to partner_id field (as if you fill the field from UI)

    `vals = {'partner_id': 1}`

    `vals = self.env['sale.order'].play_onchanges(vals, ['partner_id'])`

Then, `vals` will be updated with partner_invoice_id, partner_shipping_id, pricelist_id, etc...

Bug Tracker
===========

Bugs are tracked on `GitHub Issues
<https://github.com/OCA/server-tools/issues>`_. In case of trouble, please
check there if your issue has already been reported. If you spotted it first,
help us smashing it by providing a detailed and welcomed feedback.

Credits
=======

Images
------

* Odoo Community Association: `Icon <https://odoo-community.org/logo.png>`_.

Contributors
------------

* Guewen Baconnier <guewen.baconnier@camptocamp.com>
* Florian da Costa <florian.dacosta@akretion.com>
* Andrea Stirpe <a.stirpe@onestein.nl>

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

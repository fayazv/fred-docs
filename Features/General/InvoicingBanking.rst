


Invoicing and banking :sup:`CZ-specific`
------------------------------------------

The FRED implements the prepaid-invoicing model.

Bank accounts are queried for incoming payments using bank-specific scripts
and these payments are matched to registrars using pairing symbols.
If a payment matches, an advance invoice is issued and credit is extended
to the matching registrar by a corresponding amount.
The credit is then decreased upon each domain registration or renewal.
The price of registration and renewal is configurable per zone.

At some point in time, it's possible to create an accounting invoice
for a particular registrar containing a list of all its registrations
and renewals and the total amount of money subtracted from the credit.

.. Note::

   Work with the accounting subsystem may be tricky
   because it is tightly tied to the context of the financial and commercial
   laws of the Czech Republic (esp. the :term:`VAT` handling and invoice
   essentials).

   Therefore it may not be fully (or at all) suitable for your environment.

.. todo:: update with the postpaid model (negative credit)

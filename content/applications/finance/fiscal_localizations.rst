:show-content:

====================
Fiscal localizations
====================

Fiscal localization packages are country-specific modules that install pre-configured taxes, fiscal
positions, chart of accounts, and legal statements. Some additional features, such as the
configuration of specific certificates, are also added to the Accounting app, depending on a
country's fiscal administration requirements.

.. _fiscal_localizations/packages:

Configuration
=============

Odoo should automatically install the appropriate fiscal localization package based on the company's
country.

Verify the right package is installed by going to :menuselection:`Accounting --> Configuration -->
Settings` and checking the :guilabel:`Package` field under the :guilabel:`Fiscal Localization`
section. Select another one if necessary.

.. warning::
   Selecting another package is only possible if no entry has been posted.

.. note::
   - Each company in a multi-company environment can use a different fiscal localization package.
   - If the :doc:`Payroll app <../hr/payroll>` is installed, Odoo should also automatically
     install the appropriate :ref:`Payroll localization modules <payroll-localizations>` based on
     the company's country.

Use
===

These packages require fine-tuning the chart of accounts according to the company's needs,
activating the taxes to be used, and configuring the country-specific statements and certifications.

.. seealso::
   - :doc:`accounting/get_started/chart_of_accounts`
   - :doc:`accounting/taxes`

.. _fiscal_localizations/countries-list:

List of packages
================

Odoo Accounting can be used in many countries by using the appropriate fiscal localization package.
All packages that are currently available are listed below.

.. note::
   Odoo continuously adds new localizations and improves existing packages.

- 🇩🇿 Algeria
- :doc:`🇦🇷 Argentina - Generic Chart of Accounts Argentina Single Taxpayer / Basis
  <fiscal_localizations/argentina>`
- :doc:`🇦🇷 Argentina - Argentine Generic Chart of Accounts for Exempt Individuals
  <fiscal_localizations/argentina>`
- :doc:`🇦🇷 Argentina - Argentine Generic Chart of Accounts for Registered Accountants
  <fiscal_localizations/argentina>`
- :doc:`🇦🇺 Australia <fiscal_localizations/australia>`
- :doc:`🇦🇹 Austria <fiscal_localizations/austria>`
- 🇧🇩 Bangladesh
- :doc:`🇧🇪 Belgium - Companies <fiscal_localizations/belgium>`
- :doc:`🇧🇪 Belgium - Associations and Foundations <fiscal_localizations/belgium>`
- 🇧🇯 Benin - SYSCOHADA for Companies
- 🇧🇯 Benin - SYSCEBNL for Associations
- 🇧🇴 Bolivia
- :doc:`🇧🇷 Brazil <fiscal_localizations/brazil>`
- 🇧🇫 Burkina Faso - SYSCOHADA for Companies
- 🇧🇫 Burkina Faso - SYSCEBNL for Associations
- 🇧🇬 Bulgaria
- 🇨🇲 Cameroon - SYSCOHADA for Companies
- 🇨🇲 Cameroon - SYSCEBNL for Associations
- :doc:`🇨🇦 Canada <fiscal_localizations/canada>`
- 🇨🇫 Central African Republic - SYSCOHADA for Companies
- 🇨🇫 Central African Republic - SYSCEBNL for Associations
- 🇹🇩 Chad - SYSCOHADA for Companies
- 🇹🇩 Chad - SYSCEBNL for Associations
- :doc:`🇨🇱 Chile <fiscal_localizations/chile>`
- 🇨🇳 China
- 🇨🇳 China - Large Business
- :doc:`🇨🇴 Colombia <fiscal_localizations/colombia>`
- 🇰🇲 Comoros - SYSCOHADA for Companies
- 🇰🇲 Comoros - SYSCEBNL for Associations
- 🇨🇬 Congo - SYSCOHADA for Companies
- 🇨🇬 Congo - SYSCEBNL for Associations
- 🇨🇷 Costa Rica
- 🇨🇮 Côte d'Ivoire - SYSCOHADA for Companies
- 🇨🇮 Côte d'Ivoire - SYSCEBNL for Associations
- 🇭🇷 Croatia
- 🇭🇷 Croatia - RRIF-ov računski plan za poduzetnike
- 🇨🇾 Cyprus
- 🇨🇿 Czech Republic
- 🇨🇩 Democratic Republic of the Congo - SYSCOHADA for Companies
- 🇨🇩 Democratic Republic of the Congo - SYSCEBNL for Associations
- 🇩🇰 Denmark
- 🇩🇴 Dominican Republic
- :doc:`🇪🇨 Ecuador <fiscal_localizations/ecuador>`
- :doc:`🇪🇬 Egypt <fiscal_localizations/egypt>`
- 🇬🇶 Equatorial Guinea - SYSCOHADA for Companies
- 🇬🇶 Equatorial Guinea - SYSCEBNL for Associations
- 🇪🇪 Estonia
- 🇪🇹 Ethiopia
- 🇫🇮 Finland
- :doc:`🇫🇷 France <fiscal_localizations/france>`
- 🇬🇦 Gabon - SYSCOHADA for Companies
- 🇬🇦 Gabon - SYSCEBNL for Associations
- :doc:`🇩🇪 Germany - German Chart of Accounts SKR03 <fiscal_localizations/germany>`
- :doc:`🇩🇪 Germany - German chart of accounts SKR04 <fiscal_localizations/germany>`
- 🇬🇳 Guinea - SYSCOHADA for Companies
- 🇬🇳 Guinea - SYSCEBNL for Associations
- 🇬🇷 Greece
- 🇬🇹 Guatemala
- 🇬🇼 Guinea-Bissau - SYSCOHADA for Companies
- 🇬🇼 Guinea-Bissau - SYSCEBNL for Associations
- 🇭🇳 Honduras
- :doc:`🇭🇰 Hong Kong <fiscal_localizations/hong_kong>`
- 🇭🇺 Hungary
- :doc:`🇮🇳 India <fiscal_localizations/india>`
- :doc:`🇮🇩 Indonesia <fiscal_localizations/indonesia>`
- 🇮🇶 Iraq
- 🇮🇪 Ireland
- 🇮🇱 Israel
- :doc:`🇮🇹 Italy <fiscal_localizations/italy>`
- 🇯🇵 Japan
- 🇯🇴 Jordan
- 🇰🇿 Kazakhstan
- :doc:`🇰🇪 Kenya <fiscal_localizations/kenya>`
- 🇰🇼 Kuwait
- 🇱🇻 Latvia
- 🇱🇹 Lithuania
- :doc:`🇱🇺 Luxembourg <fiscal_localizations/luxembourg>`
- 🇲🇱 Mali - SYSCOHADA for Companies
- 🇲🇱 Mali - SYSCEBNL for Associations
- 🇲🇹 Malta
- 🇲🇺 Mauritius
- :doc:`🇲🇾 Malaysia <fiscal_localizations/malaysia>`
- :doc:`🇲🇽 Mexico <fiscal_localizations/mexico>`
- 🇲🇳 Mongolia
- 🇲🇦 Morocco
- 🇲🇿 Mozambique
- :doc:`🇳🇱 Netherlands <fiscal_localizations/netherlands>`
- :doc:`🇳🇿 New Zealand <fiscal_localizations/new_zealand>`
- 🇳🇪 Niger - SYSCOHADA for Companies
- 🇳🇪 Niger - SYSCEBNL for Associations
- 🇳🇬 Nigeria
- 🇳🇴 Norway
- 🇵🇰 Pakistan
- 🇵🇦 Panama
- :doc:`🇵🇪 Peru <fiscal_localizations/peru>`
- :doc:`🇵🇭 Philippines <fiscal_localizations/philippines>`
- 🇵🇱 Poland
- 🇵🇹 Portugal
- 🇶🇦 Qatar
- :doc:`🇷🇴 Romania <fiscal_localizations/romania>`
- 🇷🇼 Rwanda
- :doc:`🇸🇦 Saudi Arabia <fiscal_localizations/saudi_arabia>`
- 🇸🇳 Senegal - SYSCOHADA for Companies
- 🇸🇳 Senegal - SYSCEBNL for Associations
- 🇷🇸 Serbia
- :doc:`🇸🇬 Singapore <fiscal_localizations/singapore>`
- 🇸🇰 Slovakia
- 🇸🇮 Slovenia
- 🇿🇦 South Africa
- :doc:`🇪🇸 Spain - SMEs (2008) <fiscal_localizations/spain>`
- :doc:`🇪🇸 Spain - Non-profit entities (2008) <fiscal_localizations/spain>`
- :doc:`🇪🇸 Spain - Cooperatives - Complete (2008) <fiscal_localizations/spain>`
- :doc:`🇪🇸 Spain - Cooperatives - SMEs (2008) <fiscal_localizations/spain>`
- :doc:`🇪🇸 Spain - Complete (2008) <fiscal_localizations/spain>`
- 🇸🇪 Sweden
- 🇸🇪 Sweden - Swedish BAS Chart of Account complete K2
- 🇸🇪 Sweden - Swedish BAS Chart of Account complete K3
- :doc:`🇨🇭 Switzerland <fiscal_localizations/switzerland>`
- SYSCEBNL
- SYSCOHADA - Revised
- 🇹🇼 Taiwan
- 🇹🇿 Tanzania
- :doc:`🇹🇭 Thailand <fiscal_localizations/thailand>`
- 🇹🇬 Togo - SYSCOHADA for Companies
- 🇹🇬 Togo - SYSCEBNL for Associations
- 🇹🇳 Tunisia
- 🇹🇷 Türkiye
- 🇺🇬 Uganda - Uganda Generic Chart of Accounts
- 🇺🇦 Ukraine - IFRS Chart of Accounts
- :doc:`🇦🇪 United Arab Emirates <fiscal_localizations/united_arab_emirates>`
- :doc:`🇬🇧 United Kingdom <fiscal_localizations/united_kingdom>`
- :doc:`United States of America (Generic) <fiscal_localizations/united_states>`
- :doc:`🇺🇾 Uruguay - Uruguayan Generic Chart of Accounts <fiscal_localizations/uruguay>`
- 🇻🇪 Venezuela
- :doc:`🇻🇳 Vietnam <fiscal_localizations/vietnam>`
- 🇿🇲 Zambia

.. seealso::
   :doc:`Employment Hero Payroll documentation <fiscal_localizations/employment_hero>`

.. toctree::
   :titlesonly:

   fiscal_localizations/argentina
   fiscal_localizations/australia
   fiscal_localizations/austria
   fiscal_localizations/belgium
   fiscal_localizations/brazil
   fiscal_localizations/canada
   fiscal_localizations/chile
   fiscal_localizations/colombia
   fiscal_localizations/ecuador
   fiscal_localizations/egypt
   fiscal_localizations/france
   fiscal_localizations/germany
   fiscal_localizations/hong_kong
   fiscal_localizations/india
   fiscal_localizations/indonesia
   fiscal_localizations/italy
   fiscal_localizations/kenya
   fiscal_localizations/luxembourg
   fiscal_localizations/malaysia
   fiscal_localizations/mexico
   fiscal_localizations/netherlands
   fiscal_localizations/new_zealand
   fiscal_localizations/romania
   fiscal_localizations/peru
   fiscal_localizations/philippines
   fiscal_localizations/saudi_arabia
   fiscal_localizations/singapore
   fiscal_localizations/spain
   fiscal_localizations/switzerland
   fiscal_localizations/thailand
   fiscal_localizations/vietnam
   fiscal_localizations/united_arab_emirates
   fiscal_localizations/united_kingdom
   fiscal_localizations/united_states
   fiscal_localizations/uruguay
   fiscal_localizations/employment_hero

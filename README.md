# Translations for the Mozilla donate staging site

This repository contains all of the source text and translations of the content on the Mozilla donate staging site. All content is in PO format.

This is used as an intermediary between Wagtail CMS, where the site is authored and hosted from, and Pontoon, where translations of the sites content is made.

When a new english page is published, the text content of that page is broken down into segments which are written into a new POT file that is saved into the `templates` directory. Pontoon then fetches this template and loads it into the UI for translators to translate.

When translation is finished, Pontoon commits the translated PO files into the `locale` directory. This is then fetched by Wagtail where it is used to generate the translated pages.

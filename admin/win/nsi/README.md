# Windows Installer Translations

## Introduction

Translations on transifex: http://www.transifex.com/projects/p/owncloud/resource/mirall-wininstaller/

Daily sync job: https://ci.owncloud.org/view/translation-sync/job/translation-sync-mirall-wininstaller/

## How to add a new translation string?

0. Add the variable holding the new translation string to l10n/declarations.nsh

1. Add the string to the pofiles/messages.pot manually. This step is necessary
for the upload of strings to be translated to transifex

2. If you want to test your installer right away you need to add the new string
at least to l10n/English.nsh


## How to add a new language?

0. Add the new language to l10n/.tx/config which holds the explicit list of
languages to be downloaded from transifex on each translation sync run.

1. Add the new language to l10n/languages.nsh

2. In NSIS.template.in the language has to be added in the macro SETLANG.

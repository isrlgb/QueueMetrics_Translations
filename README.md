# QueueMetrics translations

This repository contains translation files for Loway QueueMetrics. Here you can help 
create, complete and fix translations.
In order to participate, you need a GitHub account.


## How it works.

If you need to create a translation for a **new language**, meaning one of the languages that are not yet included here, 
you need to open a GithHub Issue and let an admin create an empty language for you.

Once the language is created, it can contain three kinds of localizations:

* A _translated entry_, meaning a translation that has been written or at least reviewed 
 by a translator. It will appear as it is in QueueMetrics.
* An 👽  _alien translation_  , meaning that it was either created automatically through an AI, 
  or imported from a similar language (for example, if there is no entry for an item for Spanish, but 
  there is one for Latin-American Spanish, we display the latter because it’s likely to be kind of right). 
  Those translation appear as they are in QueueMetrics.
* A 🔴 _missing translation_. This is an item that exists in the English language, but nobody yet translated it 
  to your language. In QueueMetrics, it appears using the English localization.

When you work on a translation for a specific language, your goal is to  **review alien translations** and, 
more importantly, **complete missing translations**. If you look at a language file, you will see that we 
added an icon ➡️ before each translation that you have to complete and an icon 👽 or 🔴 for each item to be completed, 
so that it is easy to quickly scan the file and  and find the ones that need completing.

The document structure of the language is instead taken verbatim from English, 
and you should not modify it. Even if you were to change it, it would be put back to the format used by English. 
The structure and comments have no function in the translation but clarifying what is what.

There is also an index file that displays [the completion status for supported languages](../../blob/main/INDEX.md). 

## In practice

### How do I add a missing translation?

First you go look for entries that are preceded by a comment line with a red dot. 
There, you can see the value of that label for the English language.

<img width="333" alt="image" src="https://github.com/Loway/QueueMetrics_Translations/assets/1101849/25d44f85-7eb2-47f9-8458-36b73fc06467">


The only thing you need to do is to add your translation in the white space that follows the label.
If you want to, you can remove the comment and remove the arrow, but it’s not needed.

<img width="354" alt="image" src="https://github.com/Loway/QueueMetrics_Translations/assets/1101849/5c9fdd0a-91a3-4a9c-aa0d-ae1ef952c2c5">



### How do I confirm that  an alien translation is correct, or change it?

You can find alien translations by looking for alien icon in the comment line. As it is the case for missing translations, before each of those lines there is a comment that shows the current value for English (as a reference).

<img width="341" alt="image" src="https://github.com/Loway/QueueMetrics_Translations/assets/1101849/0964652f-61e2-44cc-be34-6f2440beb16b">

If you want to confirm the translation is right, you simply remove the `?` after `=`, so that what used to be `label=?translation` becomes `label=translation`. If you need to make any changes, go ahead and make them.

<img width="347" alt="image" src="https://github.com/Loway/QueueMetrics_Translations/assets/1101849/9a3ee4ac-ce09-44b9-a7d2-b2f4cb8dd888">



### How do I do this in practice?

As this is GitHub, the way to do a complete translation is first forking this repo to a local copy, 
then making your changes, and at the end sending us a pull  request.

THere is an excellent tutorial here: https://docs.github.com/en/get-started/exploring-projects-on-github/contributing-to-a-project



### Do I need to do it even if I only have a couple of changes, or want to correct a typo?

If you need to change just a few labels here and there, just open a GitHub issue and explain the changes you want done.

### Do I need to translate QueueMetrics entirely?

No - QueueMetrics will automatically go back to the main language (English) 
if some entries are missing in the selected language. 

When shipping languages for Queuemetrics, we will only include languages 
that have a sufficient completion grade so that the
layout will look quite consistent.


### How do I know when there are new items to be translated?

Loway periodically sends a mailing to translators to inform that there
are new items added that can be translated. 

You can anyway click on the "Watch" button within this repo so that
GitHub will notify you of changes.






## Futher information

### The Locale

QueueMetrics translations work by applying a "locale" to QueueMetrics, i.e. a set of
conventions known for a certain language, as spoken in a certain country. The locale
used shall be compatible with the Java language; if in doubt, ask Loway first.

Valid examples of locales are

* *en_US*: English as spoken in the USA
* *it_IT*: Italian for Italy
* *es_ES*: Spanish for Spain
* *fr_FR*: French for France
* *de_DE*: German for Germany
* *pt_PT*: Portuguese for Portugal and Brazil

Locales are expressed as a two-letter language (in ISO-639-1 format) plus a two-letter country code (in ISO 3166)

References can be found for:

* ISO-639-1: https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
* ISO-3166: https://en.wikipedia.org/wiki/ISO_3166-1
* Java-specific items: https://docs.oracle.com/javase/1.5.0/docs/api/java/util/Locale.html

A complete list of Java-supported locales can be found at: https://www.oracle.com/technetwork/java/javase/locales-137662.html

### Adding new languages

Translators cannot add new languages directly, but they can ask for a new language to be added.
They will need to provide Loway with the following pieces of information, as they apply to
the new language:

* `name`: The name of this translation, translated itself (e.g. `Italiano` for Italian)
* `code`: The language and country this translation is for, e.g. `en_US`
* `df_complete`: A date and time sequence, e.g. `MMMM dd yyyy, H:mm` for `May 24 2008, 8:32`
* `df_completeshort`: A shortened complete date and time, e.g `MM/dd - H:mm:ss` for `05/24 - 8:32:23`
* `df_date`: A date, e.g. `yyyy-MM-dd` for `2008-05-24`
* `df_time`: A time format, e.g. `H:mm:ss` for `8:32:23`
* `df_time_short`: A short time format, e.g `H:mm` for `8:32`
* `left_to_right`: If the language is written left-to-right or right-to-left (This is not currently used)

A full list of valid date and time placeholders can be found at: http://java.sun.com/j2se/1.4.2/docs/api/java/text/SimpleDateFormat.html




## Licenses

All contributions are subject to the MIT license.



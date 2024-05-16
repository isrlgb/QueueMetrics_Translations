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

## Licenses

All contributions are subject to the MIT license.



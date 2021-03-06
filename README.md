# Kangyur Critical Edition TEI format conventions

[![Join the chat at https://gitter.im/eroux/critical-kangyur-tei-tags](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/eroux/critical-kangyur-tei-tags?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This document supposes some basic knowledge on [TEI tags](http://www.tei-c.org/index.xml).

## Goal

The goal of this repository is to establish TEI tags conventions for critical editions of the Kangyur, in Tibetan only. It should advise users on the way they can encode a text, incorporating informations on all editions, including:

- showing the differences in the text of the different editions
- correspondance between text and page and volume of each edition
- correspondance between text and lines of each page of each edition

## Current state

TBRC uses TEI files as their database (through [Exist-db](http://exist-db.org)), one file per volume. Tags used are:

- pages are between `<tei:p n="x">` markups, where x is the page number, incremented by 1 at each page
- lines are denoted by `<tei:milestone unit="line" n="x"/>` where x is the number of the following line
- files are referenced by two ids: `TBRC_TEXT_RID` and `TBRC_RID` (with no obvious meaning)

In [ACIP texts](https://raw.githubusercontent.com/karmapa17/Lhasa-kangyur-acip-xml), TEI is not used.

In Adarsha texts, texts can be imported from TEI Lite, with tags:

    <pb id="17.104b"/>
    <bampo n="9.61" zh="16.306"/>

TEI is also used for translation at [84000](http://84000.co), but the tags used are not relevant here.

## TEI tags of interest

The main set of TEI tags used is [textcrit](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/TC.html) (critical apparatus).

## General choices

- the smallest consensual unit in a corpus of text like the Kangyur seems to be the "text", so each file should represent such a text (TODO: should more defined in a more extensible way). 

- texts are referenced through their number given in [Hackett's catalogue](http://cup.columbia.edu/book/a-catalogue-of-the-comparative-kangyur-bka-gyur-dpe-bsdur-ma/9781935011149) (example: *CK1*)

- when editions are referenced, it must be through the letters used by Hackett (*CK*, *D*, *Q*, *N*, *C*, *H*, *J*, *U*)

- there seems to be no consensual way to place a text in the Kangyur, so no common table of content can be shared between different editions.

- there is a notion of ordered volumes in each edition (though no match can be made between editions), so "volume" is a unit that can be used for a specific edition. As volumes are ordered, they are referenced here as their number (ཀ = 1, ཁ = 2, etc.).

- page number usually appear in Tibetan texts. They always reference a specific edition. The convention used here is to use `volnum.pagenumaorb` where `volnum` is the volume number (as defined above), `pagenum` is the number of the page in the tibetan text (two consecutive pages have the same number in Tibetan texts), `aorb` is `a` for the first page referenced by `pagenum` and `b` for the second one. Example of a page number : `17.104b`, which is the second page numbered `104` in the `17`th volume. This allows to easily tag pagebreaks if the pecha is shown.

- characters marking end of page (།) and beginning of page (༄༅།) are not present.

## Example

For a commented example, refer to [example.xml](example.xml).

# AwesomeGUID

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A list of awesome things related to Globally Unique Identifiers. Sorry if this whole idea is a bit mis-guid-ed.

## Tools

- [Guid Generator](https://www.guidgenerator.com/)
- [Hot Guids](http://www.secretgeek.net/hotGuids/index.htm): The Social Network for GUIDs, "Is this Guid HOT or NOT?"
- [Guess a Guid](http://guessaguid.secretgeek.net): The fun guid-guessing game
- [Cute uid](https://github.com/alexdredmon/cuteuid): Generate Cute UIDs
- [QuickInfo Guid Generator](https://quickinfo.io/?guid): With bonus Guide Dog information

## Used Guids **MUST** Be Added To This Folder

![used_guids.jpeg](used_guids.jpeg)

## Recycling and Upcycling

Instead of single-use guids, consider donating them for reliable reuse by an approved, accredited and reputable GUID recycler.

![Please Recycle GUIDS here](guid_recycling.jpg)

## Frequently Asked Questions

### What are the chances of collision?

If every human on Earth worked as a GUID generator, and they spent their entire working life generating guids at one guid per second, without even stopping for lunch, then by the time every human on earth had retired, the chances of a collision would be about 50%.

### Do guids make the best database identifiers?

Yes. But I don't use them much for that myself.

### Should you put GUIDs in URLs?

No. [Don't Put Guids in URLs](http://wiki.c2.com/?DontPutGuidsInUrls)

And if you do, **1 is enough!**

### Can I register a domain named after a specific guid value?

Yes you certainly can! But you need to hurry as they are going fast.

For example, this one is already taken:

- <http://00000000-0000-0000-0000-000000000000.com>

And certainly <http://00000000-0000-0000-0000-000000000001.com> is parked.

But as of April 2022, <http://00000000-0000-0000-0000-000000000002.com> is still available.

**Get in on it while you can.**

*There will never be another opportunity like this.*

## Explanations

- [The Quick Guide to GUIDs](https://betterexplained.com/articles/the-quick-guide-to-guids/)
- [Wikipedia: Universally Unique Identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier)

## Pronunciation Guide

- Goo-id or gwid. You decide.

## Global GUID database

- [GLOBAL UUID DATABASE](https://uuid.pirate-server.com) &mdash; World's most complete UUID database.

## Behold

Some beautiful code from [@buhakmeh](https://twitter.com/buhakmeh/status/1301517508000854022)

![code where all of the names are guids](code_conventions.png)

![Guids! Guids! As far as the eye can see!](as_far.png)

## Twitter Accounts for Lovers of The Guid

- [@usedguid](https://twitter.com/usedguid): 100% guids 100% of the time.
- [@everyguid](https://twitter.com/everyguid): tweeting every globally unique identifier.
- [@GuidGenie](https://twitter.com/GuidGenie): "Ask me to generate a GUID (Globally Unique Identifier) for you. Your wish is my command."
- [@guids4druids](https://twitter.com/guids4druids): tweeting guids for druids

## How to Generate a Guid in ANY language

And by *any* language I mean this very small subset of languages I've got examples for. PRs welcome.

### Generate a guid in javascript

    function S4() {
        return (((1+Math.random())*0x10000)|0).toString(16).substring(1);
    }
    function guid() {
        return (S4()+S4()+"-"+S4()+"-"+S4()+"-"+S4()+"-"+S4()+S4()+S4());
    }

### Generate a guid in PowerShell

As a string, and with brackets...

    "{$([guid]::NewGuid())}"

Without brackets, and as a guid not as a string...

    [guid]::NewGuid()

### Generate a guid in "C#"

    System.Guid.NewGuid().ToString("N");
    1431959a9c074d298d1787a59687f0fd

    System.Guid.NewGuid().ToString("D");
    7e760907-099b-41d9-83f7-c290dc6f059a

    System.Guid.NewGuid().ToString("B");
    {ff34e10c-db89-4f52-8757-43c56e20bf00}

    System.Guid.NewGuid().ToString("P");
    (91865f50-5112-4868-bd20-a6b4b741d04d)

    System.Guid.NewGuid().ToString("X");
    {0xaf4533d0,0xffbc,0x4716,{0x9f,0x01,0x5c,0x4c,0x29,0xdf,0x22,0xe7}}

### Generate a guid in .Net

    System.Guid.NewGuid()

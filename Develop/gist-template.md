# Regex for Validating an Email Address

If you have had to create a user sign up or sign in for a web site, you have almost certainly had to collect a user's email address, amongst other data, to create a newthe profile or search for an existing one. The developer is presented with two choices: validate that the provided email address is a valid email address in terms of matching the expected structure, or let it fly and hope that the user doesn't have a mistake in their email input. It's extremely important that the email address be correct-- it may be necessary to send a verification email to complete account set up or the email address itself may be used as the user name. Validating the email address seems like the wise choice for the developer, but how do you actually do this? With regex! Don't understand regex? Never fear; You'll learn the search pattern for an email address in this tutorial, and what that seemingly random string of characters actually means. Once you begin to understand the power of regex, you'll find more uses for it than you had ever imagined.

## Summary

Let's begin by looking at the email search pattern and then break it down into its constiuent parts.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

**Stop!** Don't *just* copy this and paste it into your own code and leave! **Stick around for the explanation**. I promise that learning regex is worth the modest time investment. Once you understand the power of searching and matching patterns, you'll be wondering where regex has been all your life!

## Table of Contents

- [What is Regex, anyway?](#what-is-regex)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## What is Regex, anyway?

Regex is short for "regular expressions". You would think that, based on its derivation, Regex would be pronounced Reg like "beg". That would make sense. But no, it is in fact pronounced reg like "hedge". Or "ledge".

A regular expression defines a pattern that is used to match strings of text. It can be used for user input validation, cleaning up copy provided by a third party, or for your own find/replace needs when writing your own code during development. Regex may consist of a combination of literal characters (the character taken literally, such as the )

Learning how to mentally parse a regular expression is a bit like learning a language. It may seem foreign and unintelligible at first, but when you start to understand its components, that random-looking string of characters won't seem so random looking anymore.

## Regex Components

### Anchors

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

**`/^ and $/`**

Let's begin our exploration of the regex matching an email address by looking at the very beginning and the very ending. You will see a forward slash, caret at the beginning and a dollar sign, forward slash at the end. The forward slashes are like a wrapper that contains the regex pattern. **The `^` is an anchor** which signifies the start of a string of characters, in the same way that you could think of quotation marks signifying the start of a quote, citation, or spoken text. **The `$` is also an anchor** and it signifies a string that begins with the characters that precede it. The string match could be an exact string match (literal) which must include all of the characters listed in the precise order they are listed. Alternatively, the match could be a **bracket expression** which defines a set of possible matches. The anchors you see here could be used in conjunction with exact matches and/or a set of possible matches.

### Bracket Expressions



### Character Escapes for Literals



### Character Classes



### Quantifiers

Quantifiers refers here not to the values of integers or floats, or even matching a specific digit, but to how many times a pattern may (or must) exist. This could be exact number (we can call it 'n') of times, depicted by `{ n }`, as in the pattern must appear exactly five times, or `{ 5 }`. `{ n, }` indicates a match of *at least* n times, and ` { n, x }` matches a minimum of n times and a maximum of x times. 

There are some frequently used quantifiers that can't be indicated using the curly braces we just discussed. `*` (zero or more times, aka "it might appear multiple times or it might not appear at all"), `+` (one or more times, aka "it must appear at least once but could appear more than once"), and `?` (zero or one time, aka "It might not appear but if it does, it must only appear once"). 

Bringing this concept of quantifiers back to our email pattern example, let's take a look at that pattern. Do you see any quantifiers?

In order, from left to right... `.`, `+`, `.`, `.`, and `{2, 6}`.

Ok, we're off to a good start, but some of you may be questioning the periods listed and you are correct to question them. A period, if unescaped, is a character class that represents "any character" (more on character classes in a bit!)

### Grouping and Capturing


### OR Operator



### Flags



### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

I am a graphic designer and web development student who has actually been using regex for several years but under the name GREP. Adobe InDesign has a search function that allows you to search your document's text for regex patterns for find/replace operations as well as for conditional styling.

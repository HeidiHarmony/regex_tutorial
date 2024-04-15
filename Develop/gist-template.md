# Regex for Validating an Email Address

If you have had to create a user sign up or sign in for a web site, you have almost certainly had to collect a user's email address, amongst other data, to create a newthe profile or search for an existing one. The developer is presented with two choices: validate that the provided email address is a valid email address in terms of matching the expected structure, or let it fly and hope that the user doesn't have a mistake in their email input. It's extremely important that the email address be correct-- it may be necessary to send a verification email to complete account set up or the email address itself may be used as the user name. Validating the email address seems like the wise choice for the developer, but how do you actually do this? With regex! Don't understand regex? Never fear; You'll learn the search pattern for an email address in this tutorial, and what that seemingly random string of characters actually means. Once you begin to understand the power of regex, you'll find more uses for it than you had ever imagined.

## Summary

Let's begin by looking at the email search pattern and then break it down into its constiuent parts.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Stop! Don't just copy this and paste it into your own code! Stick around for the explanation. I promise that learning regex is worth the modest time investment. Once you understand the power of searching and matching patterns, you'll be wondering where regex has been all your life!

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

A regular expression defines a pattern that is used to match strings of text. It can be used for user input validation, cleaning up copy provided by a third party, or for your own find/replace uses when writing your own code during development.

Learning how to mentally parse a regular expression is a bit like learning a language. It may seem foreign and unintelligible at first, but when you start to understand its components, that random-looking string of characters won't seem so random looking anymore.

## Regex Components

### Anchors

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Lab done solo by Alex Pan

"Check Your Understanding" question answers 

1. Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

I would have the automated tests run whenever code is pushed. Since everybody is working in branches, this makes sure that when a pull 
request is opened, it is easy to tell whether the code actually works or not. I also think that the developer should have the ability 
to manually run tests locally before pushing code, since they really shouldn't be relying on pushing code to see if their tests cases pass.

2. Would you use an end to end test to check if a function is returning the correct output? (yes/no)

Generally, no. However, if the function is something like getting the number of times a user has clicked a button in the past 10 seconds - 
some JavaScript closely tied with frontend interaction, then an end to end test is necessary.

3. What is the difference between navigation and snapshot mode?

Navigation mode analyzes a pages right after it loads, making it useful for testing the Load part of the RAIL model. Snapshot analyzes 
a page in the state it is currently in, whether that be right after it loads, or after some changes. It is useful for finding accessibility 
issues.

4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

Lighthouse in both snapshot mode and navigation mode reports 3 issues: the document doesn't have a `<meta name="viewport">` tag, a meta 
description, and the `<html>` element doesn't have a `[lang]` attribute. These are all accessibility issues, and negatively impact the 
page's visibility in browsers and search engines.
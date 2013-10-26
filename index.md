# Acceptance Tests Can Be Sexy

## What?

Web application testing is a PITA but it can save your bacon.

You really should exercise your application end to end covering all of your major feature functionality.

## Why?

* Quality.
* Sleep better. 
* Freedom to change your destiny. 
* Courage that it will not all go down in flames.

## When 

### ... should we start?

We did it late in the game which might have been a good thing as we didn't have a lot of test weight. 

Could have done it sooner to save regression headaches.

### ... should we run them?

All the time. CI. Check-in dance. 

## Who? 

* As many teammates as possible.

## How? 

We started out with Storyteller but moved to [Canopy](http://lefthandedgoat.github.io/canopy/index.html) and have been really happy.

### ... should I organize the tests?

Compose a "API" for the site under test. Your site API is composed of selectors and behaviors and your tests simply poke the behaviors and test the DOM state behind the selectors. 

* Selectors - atoms of a page
* Functions - page behaviors (API)
* Modules - reusable behaviors 
* Suites and tests - typical <x>unit stuff 
* Architect your tests for change.

Tests become easy to understand and mantaintain because they are protected from changes to your site. When site changes break your tests it is usually a matter of repairing a selector or a page behavior.

Fowler talks about this but [page objects](http://martinfowler.com/bliki/PageObject.html) may be overkill. The idea is spot on 

## Timing issues

The web is async. Tests need to compensate.

* Easy to  wait for things to appear or disappear. 
* Harder to know when exsiting strucutre is done being refreshed.

https://gist.github.com/KevM/7167521#file-_5_async-fs


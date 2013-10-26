# Acceptance Tests Can Be Sexy

## What?

Exercise your application end to end covering all the major feature functionality.

## Why?

* Sleep better. 
* Freedom to change your destiny. 
* Courage that it will not all go down in flames.

## When? 

We did it late in the game. Might have been a good thing. Could have done this a bit sooner.

## Who? 

* As many as possible

## Where?

* Ideally, part of your check in dance.
* Part of your continious integration.
* Sadly it is seems to be a Friday ritual for us. (RequireJS)

## How? 

https://gist.github.com/KevM/7167521

* Selectors
* Functions
* Modules

* Architect your tests for change.
* Test API

http://martinfowler.com/bliki/PageObject.html

## Timing issues

The web is async. Tests need to compensate.

* Easy to  wait for things to appear or disappear. 
* Harder to know when exsiting strucutre is done being refreshed.

https://gist.github.com/KevM/7167521#file-_5_async-fs


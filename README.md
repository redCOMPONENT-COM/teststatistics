# teststatistics

> Please notice this repository is discountinued. Community is free to send updates and they will be happily processed, but redCOMPONENT is no longer updating to latest versions of Codeception as it has not been in maintenance for the past 5 years.

Codeception Extension to measure the performance of your tests

After running your tests you will see a Performance report of your tests:

```
Tests Performance times
-----------------------------------------------
tagCest::create                     6s
tagCest::edit                       15s
tagCest::delete                     3s


Slow Steps (Steps taking more than 3s)
-----------------------------------------------
I click button 6s
```

## Installation

Add teststatistics to your composer.json

```yaml
  "require-dev": {
    ...
    "redcomponent/teststatistics": "dev-master",
```

## Useage

Simply add to your extensions the line at the bottom in the following example in your codeception.yml:

```yaml
actor: Tester
paths:
  tests: tests
  log: tests/_output
  data: tests/_data
  helpers: tests/_support
settings:
  bootstrap: _bootstrap.php
  colors: true
  memory_limit: 1024M
extensions:
  enabled: [Codeception\Extension\Teststatistics]
```

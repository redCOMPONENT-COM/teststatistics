# teststatistics
Codeception Extension to measure the performance of your tests

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

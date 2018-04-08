# JetPHP
## Documentation

### Start

This model is used for managing POST and GET data securely and correctly filter sessions.

#### How to use?

```php
  <?php
    echo Start::get('id'); // Read GET data
    echo Start::post('id'); // Read POST data
    echo Start::session('id'); // Read Session data
  ?>
```

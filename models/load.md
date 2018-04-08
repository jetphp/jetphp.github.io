# JetPHP
## Documentation

### Load

This model is used for load classes or views.

#### Loading classes

```php
  <?php
    Load::class('class_name'); // Include a class from the dir "app/controlador/classes"
  ?>
```

#### Loading views

```php
  <?php
    Load::view('site.index'); // Load view from the file "app/visual/site/index.phtml" and include references from "app/visual/inc/*"
  ?>
```

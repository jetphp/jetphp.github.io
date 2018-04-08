# JetPHP
## Documentation

### Database

The DB model is a static class

#### How to use?

```php
<?php
  $sql = "SELECT * FROM tbl_name"; // Your query.
  $qr = DB::execute($sql); // Executing your query.

  if ($qr->count() > 0) { // Verifying if the query's number of rows is bigger than 0.
    // If the query's number of rows is bigger than 0.
    mostrar($qr->list(PDO::FETCH_OBJ)); // Showing your query data.
  } else {
    // If the query's number of rows isn't bigger than 0.
  }
?>
```

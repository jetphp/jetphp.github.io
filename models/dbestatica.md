# JetPHP
## Documentation

### Static Database

The Static Database model is a normal class and you will need to call it.

#### How to use?

```php
<?php
  $dbe = new DBE();
  $tbl = $dbe->tbl_name;
  $qr  = $tbl()->
              where("active = 1")-> // In the where's method, you can filter your query data.
                join("INNER JOIN tbl_name_1 t1 ON t1.id = tbl_name.reference")-> // In the join's method, you can connect the table with other tables.
                  mostrar('todos'); // In the mostrar's method, you will need to use an id (for specific record), 'todos' for return all data in an object array or leave empty to get just one record.
   
  if ($qr != false) { // Check if the table isn't empty.
    // If the table isn't empty.
    mostrar($qr); // Show all data from the table
    print($qr[0]->id); // Variable $qr is an object, you will need to call the records like this.
  } else {
    // If the table is empty.
  }
?>
```

# JetPHP
## Documentation

### Database

The DB model is a static class

#### How to use?

```
$sql = "SELECT * FROM tbl_name"; // Your query.
$qr = DB::executar($sql); // Executing your query.

if ($qr->contar() > 0) { // Verifying if the query's number of rows is bigger than 0.
  // If the query's number of rows is bigger than 0.
  mostrar($qr->mostrar()); // Showing your query data.
} else {
  // If the query's number of rows isn't bigger than 0.
}
```

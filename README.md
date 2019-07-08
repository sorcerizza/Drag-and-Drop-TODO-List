jQuery Drag and Drop TODO List with PHP MySQL


## Code Example......

```

$result           = mysqli_query($conn, $sqlIncomplete);

//Fetch all imcomplete list items
$incomleteItems   = mysqli_fetch_all($result,MYSQLI_ASSOC);

//Get incomplete items
$sqlCompleted     = "SELECT id, name, detail, is_completed FROM listitems where is_completed = 'yes' ORDER 
                     BY id desc";
  
$completeResult    = mysqli_query($conn, $sqlCompleted);

//Fetch all complted items
$completeItems     = mysqli_fetch_all($completeResult, MYSQLI_ASSOC);
 
//Free result set
mysqli_free_result($completeResult);
mysqli_free_result($result);
  
mysqli_close($conn);
```


## Usage

Use to add/edit/delete tasks without persistence (no backend).

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

0.1.0 Finalized the example

## Tests

Basic non-automated manual browser test aka no test :P

# jquery-drag-drop-todo-List-with-php-mysql



Following tasks are performed in this tutorial


1. Create a MySQL database and database table for todo list items

2. PHP code to connect to database.

3. Create php code to fetch incomplete and complete todo list items

4. Display records on page in incomplete todo list items to the left side of page.

5. Incomplete list items will be draggable.

6. Complete list items will be displayed to the right side of the page.

7. Completed list item area will be droppable.

8. Add drag and drop jQuery code.

9. After the item is dragged send an AJAX request to update status of list item as completed.

## Contributors

Standing on the shoulders of all the giants before me.

## Contact
#### sorcererizza
* E-mail: izzaannsamax@gmail.com


---
title: "query"
permalink: /html-class/query
excerpt: "query."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

It makes a request to the database by the connection set in the _config.json_ file.<br>
Before doing the queries you must be sure that you have ever made the connection through the `$this->addConnection("config/connection.json");` command and have enabled the connection inside the _config.json_ file.<br>
```java
void query ( String $_query )
```

## Parameters
Query string.

## Return Values
Depends of type of query.

## Examples
```php
<?php
  $this->query("UPDATE user SET name = 'Bruce' WHERE surname = 'Wayne'");
?>
```

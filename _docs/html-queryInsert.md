---
title: "queryInsert"
permalink: /html-class/queryInsert
excerpt: "queryInsert."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

It makes a __INSERT__ request to the database by the connection set in the _config.json_ file.<br>
Before doing the queries you must be sure that you have ever made the connection through the `$this->addConnection("config/connection.json");` command and have enabled the connection inside the _config.json_ file.<br>
```java
void queryInsert ( String $_query )
```

## Parameters
Query string.

## Return Values
Last id inserted.

## Examples
```php
<?php
  $this->queryInsert("INSERT INTO user (name, surname) VALUES ('Bruce', 'Wayne')");
?>
```

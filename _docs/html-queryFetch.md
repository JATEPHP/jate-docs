---
title: "queryFetch"
permalink: /html-class/queryFetch
excerpt: "queryFetch."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

It makes a __SELECT__ request to the database by the connection set in the _config.json_ file.<br>
Before doing the queries you must be sure that you have ever made the connection through the `$this->addConnection("config/connection.json");` command and have enabled the connection inside the _config.json_ file.<br>
```java
void queryFetch ( String $_query )
```

## Parameters
Query string.

## Return Values
Array with associate columns.
```php
<?php
  [
    [ "name" => "Bruce", "surname" => "Wayne" ],
    [ "name" => "Clark", "surname" => "Kent" ]
  ]
?>
```

## Examples
```php
<?php
  $this->queryFetch("SELECT * FROM user");
?>
```

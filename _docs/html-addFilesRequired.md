---
title: "addFilesRequired"
permalink: /html-class/addFilesRequired
excerpt: "addFilesRequired."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

Add files to the page before `addFiles`.<br>
```java
void addFilesRequired ( Array $_files )
```

## Parameters
Array of path string of css and js file.

## Return Values
None.

## Examples
```php
<?php
  $this->addFilesRequired([
    "css/myFile.css",
    "js/myFile.js"
  ]);
?>
```

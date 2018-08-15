---
title: "addFiles"
permalink: /html-class/addFiles
excerpt: "addFiles."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

Add files to the page.<br>
```java
void addFiles ( Array $_files )
```

## Parameters
Array of path string of css and js file.

## Return Values
None.

## Examples
```php
<?php
  $this->addFiles([
    "css/myFile.css",
    "js/myFile.js"
  ]);
?>
```

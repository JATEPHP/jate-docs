---
title: "init"
permalink: /html-class/init
excerpt: "init."
last_modified_at: 2018-08-15T16:28:04-05:00
toc: false
---

Is a virtual function for Html class is needed for inizialize derivate class like Template.<br>
```java
void init ()
```

## Parameters
None.

## Return Values
None.

## Examples
Typical __Controller.php__ init.
```php
<?php
  public function init() {
    parent::init();
    $this->tags["title"]  .= "Home";
    $this->tags["content"] = $this->makePage();
  }
?>
```

Typical __Template.php__ init.
```php
<?php
  public function init() {
    $this->addConnection("config/connection.json");
    $this->addFilesRequired([
      "https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css",
      "https://code.jquery.com/jquery-3.2.1.slim.min.js",
      "https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js",
      "https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js",
      "css/template.css"
    ]);
    $this->template = "bundles/views/tradictional.jate";
    $this->tags = [
      "title"    => "JATE - ",
      "brand"    => "JATE",
      "brandImg" => "",
      "menu"     => $this->makeMenu(),
      "metaDescription" => "Beautiful description.",
      "metaKeywords"    => "JATE,PHP,JS,CSS",
      "metaAuthor"      => "XaBerr"
    ];
  }
?>
```

---
title: "Version 0.5.4"
permalink: /version-0-5-4
excerpt: "Version 0.5.4."
last_modified_at: 2018-03-19T16:28:04-05:00
toc: false
---

Added two new functions:
- `view`
- `sql`

Changed `config/connection.json`:<br>
from<br>
```json
{
  "enable":    false,
  "user":      "",
  "password":  "",
  "database":  "",
  "server":    "",
  "engine": {
    "pdo":        true,
    "mysqli":     false,
    "postgresql": false
  }
}
```
to<br>
```json
{
  "enable":    false,
  "user":      "",
  "password":  "",
  "database":  "",
  "server":    "",
  "engine": {
    "pdo-mysql":         true,
    "pdo-sqlite-memory": false,
    "pdo-sqlite-file":   false,
    "mysqli":            false,
    "postgresql":        false
  }
}

```

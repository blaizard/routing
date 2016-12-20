## Simple & Fast HTTP request dispatcher (PHP)

Single PHP file used to dispatch HTTP requests. Easy to configure and very fast.

&#128279; https://www.blaizard.com/projects/routing

## Features

* Single-file
* Fast
* Easy to use

## Getting Started

```php
// Include the header file
require_once("routing.php");

// Create the object and configure it
$app = new Routing();

$app->route("get", "/api/module-{id:[0-9]+}", function($vars) {
	echo "Id: ".$vars["id"];
});

// Dispatch
$app->dispatch();
```

##### Atom and all repositories under Atom will be archived on December 15, 2022. Learn more in our [official announcement](https://github.blog/2022-06-08-sunsetting-atom/)
 # Tasks Lists (JS)

Turns a GFM style task list into a series of checkboxes.

## Installation

```
npm install task-lists
```

## Usage

```coffeescript
var roaster = require("roaster");
var taskLists = require("../src/index");
var fs = require("fs");

var options = {};
options.isFile = true;

roaster("./markdown.md", options, function(err, contents) {
	contents = taskLists(contents);
    fs.writeFileSync("./markdown.html", contents, "utf8");
});
```


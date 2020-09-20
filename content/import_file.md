# Import file

**Java - Android**
```
?
```

**Javascript**
```
function getScript(source, callback) {
    var element = document.createElement("script");
    element.onload = callback;
    element.src = source;
    document.body.appendChild(element);
}

getScript("file.js", function() {
    //callback
});
```

**Objective-C**
```
#import "file.h"
```

**PHP**
```
require "file.php";
```


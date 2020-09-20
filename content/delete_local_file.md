# Delete local file

**Java - Android**
```
File file = new File("file.txt");
boolean deleted = file.delete();
```

**Objective-C**
```
[manager removeItemAtPath:[NSHomeDirectory() stringByAppendingPathComponent:"file.txt"] error:&error]
```

**PHP**
```
unlink("file.txt");
```


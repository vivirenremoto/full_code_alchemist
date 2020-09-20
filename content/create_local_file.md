# Create a local file

**Java - Android**
```
String file = "file.txt";
String content = "content";
File path = context.getFilesDir();
File path = context.getExternalFilesDir(null);
File file = new File(path, file);
FileOutputStream stream = new FileOutputStream(file);
try {
    stream.write(content.getBytes());
} finally {
    stream.close();
}
```

**Objective-C**
```
NSString *file = @"file.txt";
NSString *content = @"content";
NSArray *paths = NSSearchPathForDirectoriesInDomains(NSDocumentDirectory, NSUserDomainMask, YES);
NSString *documentsDirectory = [paths objectAtIndex:0];
NSString *filePath = [documentsDirectory stringByAppendingPathComponent:file];
[str writeToFile:filePath atomically:TRUE encoding:NSUTF8StringEncoding error:NULL];
```

**PHP**
```
$file = "file.txt";
$content = "content";
file_put_contents($file, $content);
```


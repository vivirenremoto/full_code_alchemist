# Read local file

**Java - Android**
```
String file = "file.txt";
int length = (int) file.length();
byte[] bytes = new byte[length];
FileInputStream in = new FileInputStream(file);
try
{
    in.read(bytes);
}
finally
{
    in.close();
}
String content = new String(bytes);
```

**Objective-C**
```
NSString *file = "file.txt";
NSArray *paths = NSSearchPathForDirectoriesInDomains(NSDocumentDirectory, NSUserDomainMask, YES);
NSString *documentsDirectory = [paths objectAtIndex:0];
NSString *filePath = [documentsDirectory stringByAppendingPathComponent:file];
NSString *content = [NSString stringWithContentsOfFile:filePath encoding:NSUTF8StringEncoding error:NULL];
```

**PHP**
```
$file = "file.txt";
$content = file_get_contents($file);
```


# Parse JSON

**Java - Android**
```
JSONObject obj = new JSONObject(string);
```

**Javascript**
```
object = JSON.parse(string);
```

**Objective-C**
```
NSData *data = [string dataUsingEncoding:NSUTF8StringEncoding];
NSArray *object = [NSJSONSerialization JSONObjectWithData:data options:NSJSONReadingAllowFragments error:nil];
```

**PHP**
```
$object = json_decode($string);
``````

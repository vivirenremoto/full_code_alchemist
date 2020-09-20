# Convert array to json string

**Java - Android**
```
JSONObject array = new JSONObject();
string = array.toString();
```

**Javascript**
```
string = JSON.stringify(array);
```

**Objective-C**
```
NSDictionary *array = [[NSDictionary alloc] init];
NSError *error;
NSData *jsonData = [NSJSONSerialization dataWithJSONObject:JSONDic options:NSJSONWritingPrettyPrinted error:&error];
NSString *string = [[NSString alloc] initWithData:jsonData encoding:NSUTF8StringEncoding];
```

**PHP**
```
$string = json_encode($array);
``````

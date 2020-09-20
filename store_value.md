# Store value

**Java - Android**
```
SharedPreferences.Editor prefs = getSharedPreferences(MY_PREFS_NAME, MODE_PRIVATE).edit();
prefs.putString("key", "value");
prefs.apply();
```

**Javascript**
```
localStorage.setItem("key", "value");
```

**Objective-C**
```
NSUserDefaults *prefs = [NSUserDefaults standardUserDefaults];
[prefs setObject:@"value" forKey:@"key"];
```

**PHP**
```
session_start();
$_SESSION["key"] = "value";
```


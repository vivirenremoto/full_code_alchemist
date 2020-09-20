# Retrieve stored value

**Java - Android**
```
SharedPreferences.Editor prefs = getSharedPreferences(MY_PREFS_NAME, MODE_PRIVATE).edit();
value = prefs.getString("key", "default value");
```

**Javascript**
```
value = localStorage.getItem("key");
```

**Objective-C**
```
NSUserDefaults *prefs = [NSUserDefaults standardUserDefaults];
value = [prefs stringForKey:@"key"];
```

**PHP**
```
session_start();
$value = $_SESSION["key"];
```


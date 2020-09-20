# Read content from a URL

**Java - Android**
```
String url = "https://domain.com/page.html";
String content = "";
HttpClient client = new DefaultHttpClient();
HttpGet request = new HttpGet(url);
HttpResponse response = client.execute(request);
InputStream in = response.getEntity().getContent();
BufferedReader reader = new BufferedReader(new InputStreamReader(in));
StringBuilder str = new StringBuilder();
String line = null;
while((line = reader.readLine()) != null)
{
    str.append(line);
}
in.close();
content = str.toString();
```

**Javascript**
```
var content = "";
var xhr = new XMLHttpRequest();
xhr.open("GET", "https://domain.com/page.html");
xhr.send(null);
xhr.onreadystatechange = function()
{
  if (xhr.readyState === 4) {
    if (xhr.status === 200)
    {
      content = xhr.responseText;
    }
    else
    {
      console.log('Error: ' + xhr.status);
    }
  }
};
```

**Objective-C**
```
NSString *content = "";
NSURLSession *aSession = [NSURLSession sessionWithConfiguration:[NSURLSessionConfiguration defaultSessionConfiguration]];
[[aSession dataTaskWithURL:[NSURL URLWithString:@"https://domain.com/page.html"] completionHandler:^(NSData *data, NSURLResponse *response, NSError *error) {
    if (((NSHTTPURLResponse *)response).statusCode == 200) {
        if (data) {
            content = [[NSString alloc] initWithData:data encoding:NSUTF8StringEncoding];
        }
    }
}] resume];
```

**PHP**
```
$content = file_get_contents("https://domain.com/page.html");
```


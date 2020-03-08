
# JSON-Simply-Legible
This is a modified version of the JSON-Simple library. JSON objects are printed with whitespace for legibility purposes. 
The intent of this modification is for the library to be used for educational purposes.

## Changes/Modifications
- #### JSONObject.java
     - added "scope" parameter to writeJSONString(Object value, Writer out)
     - added lines to print "\n" and "\t" as needed in writeJSONString(Object value, Writer out, int scope)
     - added writeJSONString(Map map, Writer out) helper method

-  #### JSONValue.java
     - added writeJSONString(Object value, Writer out, int scope)

## Example Output

#### Original JSON-Simple
```
{"user":"testuser@email.com","data":{"cart":["itemID1","itemID2","itemID3"],"msg":"Thanks for the fake items"}}
```

#### Modified JSON-Simple
```
{
    "user":testuser@email.com,
    "data":{
        "cart":["itemID1","itemID2","itemID3"],
        "msg":"Thanks for the fake items"
    }
}
```

## Credit
All credit for the original project should be given to 
[@fangyidong](https://github.com/fangyidong/) as well as any contributors to the original repo.

## Please visit:
https://github.com/fangyidong/json-simple
http://code.google.com/p/json-simple/
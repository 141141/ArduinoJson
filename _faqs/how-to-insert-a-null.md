---
title: How to insert a <code>null</code>?
description: To insert a null in the JSON, add a NULL char*
layout: faq
tags: faq
faq-group: Serialization
popularity: 53
---

There are two ways to serialize a `null`:

* either set the value to `(char*)0`,
* or set the value to `RawJson("null")`

For example, to generate the following JSON:

```json
{"myValue":null}
```

you can write:

```c++
DynamicJsonBuffer jsonBuffer;
JsonObject& root = jsonBuffer.createObject();
root["myValue"] = (char*)0; // or (char*)NULL if you prefer
root.printTo(Serial);
```

See:

* issue [#418](https://github.com/bblanchon/ArduinoJson/issues/418)

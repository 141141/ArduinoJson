---
title: What are the common sizes for JsonBuffer?
description: JsonBuffer size ranges from a few hundreds to a few thousand bytes
keywords: ArduinoJson,StaticJsonBuffer,DynamicJsonBuffer,size
layout: faq
tags: faq
faq-group: Common
popularity: 121
---

| Input                              | AVR 8-bit | ESP8266 | x86   | x64   |
| ---------------------------------- | --------- | ------- | ----- | ----- |
| OpenWeatherMap (one location)      | 436       | 712     | 1384  | 1504  |
| Weather Underground (one location) | 882       | 1424    | 2816  | 2912  |
| Forecast.io                        | 13442     | 21588   | 42648 | 44232 |
{: .table .table-striped .table-bordered .table-hover .table-sm}

Theses results were generated with the [ArduinoJson Assistant]({{ site.baseurl }}/assistant/).

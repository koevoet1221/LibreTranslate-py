# LibreTranslate-py

Python bindings to connect to a [LibreTranslate API](https://github.com/LibreTranslate/LibreTranslate)

https://pypi.org/project/libretranslatepy/

## Install
clone the repo into your working directory

## Fork difference
This versions accepts both strings and lists of strings.

## Example usage
```python
from libretranslatepy import LibreTranslateAPI

lt = LibreTranslateAPI("https://libretranslate.com/")

print(lt.translate("LibreTranslate is awesome!", "en", "es"))
# LibreTranslate es impresionante!

print(lt.detect("Hello World"))
# [{"confidence": 0.6, "language": "en"}]

print(lt.languages())
# [{"code":"en", "name":"English"}, {"code":"es", "name":"Spanish"}]
```

## [LibreTranslate Mirrors](https://github.com/LibreTranslate/LibreTranslate#mirrors)

## License
Licensed under either the MIT License or Public Domain

Developed by P.J. Finlay

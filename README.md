# LM60Py
## Introduction
  This module provides methods for measuring temperature using LM60.

## Usage
  You run the following script on LM60Py/ directory.

```
git clone MCP3008Pi

```

  Then you can use LM60Py.

##method

1. LM60(bus, device, channel)
bus : The number of SPI port (SPI0 or SPI1)
device : CS pin number
channel : using MCP3008 port

2. read()
Temperature value read.


## Sample Code

```
#!/usr/bin/env python

from LM60Py import lm60

temp = lm60.LM60(1,2,0)

print(temp.read())
``` 

## LICENCE
Copyright 2017 Akira Kashihara

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

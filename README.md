>日本語は下にあります。
# LM60Pi
## Introduction
  This module provides methods for measuring temperature using LM60.

## Usage
  If LM60Pi does not have MCP3008Pi module please run the following script on LM60Pi/ directory.

```
git clone MCP3008Pi
```

  Then you can use LM60Pi.

## method

1. LM60(bus, device, channel)

 - bus : The number of SPI port (SPI0 or SPI1)

 - device : CS pin number
 
 - channel : using MCP3008 port

2. read()

  Temperature value read.


## Sample Code

```
#!/usr/bin/env python

from LM60Pi import lm60

temp = lm60.LM60(0,0,0)

print(temp.read())
``` 

## LICENCE
  This source code is provided under MIT Licence. The detail is on LICENCE file.

## Bugs
  If you finde some bugs of this Module, please create issue on following page.

  https://github.com/KASHIHARAAkira/LM60Pi/issues


>日本語
## 概要
  このモジュールはLM60から得た値を気温に変換するモジュールです。

## 使用方法
  このコードをライブラリは、MCP3008Piが必要です。もしもLM60Piの下に、このモジュールがない場合は以下のscriptをterminalで実行してください。

```
git clone https://github.com/KASHIHARAAkira/MCP3008Pi
```

## メソッド

1. LM60(bus, device, channel)

  - bus : SPIポートの番号です (SPI0 or SPI1)

  - device : CSピン（チップセレクタピン）の番号です。

  - channel : MCP3008の使用するチャンネルです。

2. read()

  気温を取得します。


## サンプルコード

```
#!/usr/bin/env python

from LM60Pi import lm60

temp = lm60.LM60(0,0,0)

print(temp.read())
``` 

## ライセンス
  このソースコードは、MIT Licenceによって提供されています。詳しくはLICENCEファイルを御覧ください。

## バグについて
　このモジュールのバグを見つけた方は、以下のリンク先でissueの発行をお願いします。

  https://github.com/KASHIHARAAkira/LM60Pi/issues
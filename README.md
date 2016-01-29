# 4d-plugin-kotoeri-option
4D plugin to control the defaults of Japanese IM (a.k.a. Kotoeri) on Mac

##Platform

| carbon | cocoa | win32 | win64 |
|:------:|:-----:|:---------:|:---------:|
|🆗|🆗|🚫|🚫|

Commands
---

```c
// --- Kotoeri
Kotoeri_Get_option
Kotoeri_SET_OPTION
```

Example
---

```
  //"1" kana, "0" romaji
$isKana:=Kotoeri Get option ("JIMPrefTypingMethodKey")

Kotoeri SET OPTION ("JIMPrefTypingMethodKey";Choose($isKana="1";"0";"1");Is integer)

  //for more keys see
  //http://baqamore.hatenablog.com/entry/2015/02/09/221934

  //note: change takes effect after window switch or focus event
```

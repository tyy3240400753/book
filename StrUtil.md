# StrUtil: Practical HarmonyOS Development


Download and install
`ohpm i @pura/harmony-utils`  


## API methods and usage

------

##### isNull determines whether the string is empty (undefined, null)

```
let str0 = '哈哈哈哈';
let str1 = '';
let str2 = null;
let str3 = undefined;
let bl0 = StrUtil.isNull(str0);
let bl1 = StrUtil.isNull(str1);
let bl2 = StrUtil.isNull(str2);
let bl3 = StrUtil.isNull(str3);
```

##### isNotNull determines whether the string is not defined, null

```
let str0 = '哈哈哈哈';
let str1 = '';
let str2 = null;
let str3 = undefined;
let bn0 = StrUtil.isNotNull(str0);
let bn1 = StrUtil.isNotNull(str1);
let bn2 = StrUtil.isNotNull(str2);
let bn3 = StrUtil.isNotNull(str3);
```

##### isEmpty determines whether the string is empty (undefined, null, string length is 0)

```
let str0 = '哈哈哈哈';
let str1 = '';
let str2 = null;
let str3 = undefined;
let bl0 = StrUtil.isEmpty(str0);
let bl1 = StrUtil.isEmpty(str1);
let bl2 = StrUtil.isEmpty(str2);
let bl3 = StrUtil.isEmpty(str3);
```

##### isNotEmpty determines whether the string is non-empty (undefined, null, string length is 0)

```
let str0 = '哈哈哈哈';
let str1 = '';
let str2 = null;
let str3 = undefined;
let bn0 = StrUtil.isNotEmpty(str0);
let bn1 = StrUtil.isNotEmpty(str1);
let bn2 = StrUtil.isNotEmpty(str2);
let bn3 = StrUtil.isNotEmpty(str3);
```

##### isBlank determines whether the string is empty and whitespace (whitespace includes spaces, tabs, full-width spaces and uninterrupted spaces)

```
let str0 = '\t\n  ';
let str1 = '      ';
let str2 = " \t \t ";
let str3 = " 哈 哈 ";
let bl0 = StrUtil.isBlank(str0);
let bl1 = StrUtil.isBlank(str1);
let bl2 = StrUtil.isBlank(str2);
let bl3 = StrUtil.isBlank(str3);
```

##### isNotBlank determines whether the string is non-empty

```
let str0 = '\t\n  ';
let str1 = '      ';
let str2 = " \t \t ";
let str3 = " 哈 哈 ";
let bn0 = StrUtil.isNotBlank(str0);
let bn1 = StrUtil.isNotBlank(str1);
let bn2 = StrUtil.isNotBlank(str2);
let bn3 = StrUtil.isNotBlank(str3);
```

##### trim Removes spaces at both ends of strings

```
let str1 = " 　 H e llo  　 World \t ";
let str2 = "   呵呵\n嘿\t嘿   哈哈 ";
let trimStr1 = StrUtil.trim(str1);
let trimStr2 = StrUtil.trim(str2);
```

##### trimAll Removes all spaces in the string

```
let str1 = " 　 H e llo  　 World \t ";
let str2 = "   呵呵\n嘿\t嘿   哈哈 ";
let trimStr1 = StrUtil.trimAll(str1);
let trimStr2 = StrUtil.trimAll(str2);
```

##### replace the matching regular in the string to the given string

```
let str1 = "阿超是一个好人,小阿超也是一个好人";
let str = StrUtil.replace(str1, "阿超", "张三");
```

##### replaceAll replaces all matching regulars in the string to the given string

```
let str1 = "阿超是一个好人,小阿超也是一个好人";
let strAll = StrUtil.replaceAll(str1, "好人", " HAO-REN ");
```

##### startsWith determines whether a string starts with the given string

```
let str1 = "大聪明是一个好人,DSB也是一个好人";
let startsWith = StrUtil.startsWith(str1, "大聪明");
```

##### endsWith determines whether a string ends with the given string

```
let str1 = "大聪明是一个好人,DSB也是一个好人";
let endsWith = StrUtil.endsWith(str1, "好人");
```

##### repeat the string number of times

```
let str2 = "千秋万代";
let strs = StrUtil.repeat(str2, 6);
```

##### toLower converts the entire string to lowercase

```
let str = "anima,For generations to come, Forever Immortal,IT is SB";
let str1 = StrUtil.toLower(str);
```

##### toUpper Converts the entire string to uppercase

```
let str = "anima,For generations to come, Forever Immortal,IT is SB";
let str2 = StrUtil.toUpper(str);
```

##### capitalize Converts the first letter of the string to uppercase, and the rest is lowercase

```
let str = "anima,For generations to come, Forever Immortal,IT is SB";
let str3 = StrUtil.capitalize(str);
```

##### equal determines whether two incoming values ​​or strings are equal

```
let bl1 = StrUtil.equal("ASX1", "ASX1");
let bl2 = StrUtil.equal("ASX1", "AS1");
let bl4 = StrUtil.equal(26, 26);
let bl5 = StrUtil.equal(26, 29);
```

##### notEqual determines whether two incoming values ​​or strings are not equal

```
let bl3 = StrUtil.notEqual("AS1", "ASX1");
let bl6 = StrUtil.notEqual(22, 32);
```

##### strToUint8Array string to Uint8Array

```
let str1 = "我是笑哈哈";
let unit8Array = StrUtil.strToUint8Array(str1);
```

##### unit8ArrayToStr Uint8Array to string

```
let str1 = "我是笑哈哈";
let unit8Array = StrUtil.strToUint8Array(str1);
let str = StrUtil.unit8ArrayToStr(unit8Array);
```

##### strToBase64 string to Base64 string

```
let str1 = "我是笑面虎";
let base64Str = StrUtil.strToBase64(str1);
```

##### base64ToStr Base64 string to string

```
let str1 = "我是笑面虎";
let base64Str = StrUtil.strToBase64(str1);
let str = StrUtil.base64ToStr(base64Str);
```

##### strToBuffer string to ArrayBuffer

```
let str1 = "我是乐哈哈";
let buff = StrUtil.strToBuffer(str1);
```

##### bufferToStr ArrayBuffer to string

```
let str1 = "我是乐哈哈";
let buff = StrUtil.strToBuffer(str1);
let str = StrUtil.bufferToStr(buff);
```

##### bufferToUint8Array ArrayBuffer to Uint8Array

```
let str1 = "我是甜啦啦";
let buff1 = StrUtil.strToBuffer(str1);
let unit8Array = StrUtil.bufferToUint8Array(buff1);
```

##### unit8ArrayToBuffer Uint8Array to ArrayBuffer

```
let str1 = "我是甜啦啦";
let buff1 = StrUtil.strToBuffer(str1);
let unit8Array = StrUtil.bufferToUint8Array(buff1);
let buff = StrUtil.unit8ArrayToBuffer(unit8Array);
```

##### getErrorStr Gets the JSON string of Error

```
let error = new Error("未知异常！");
let errorStr = StrUtil.getErrorStr(error as BusinessError);
```

##### getErrnoToString Get detailed information corresponding to the system error code

```
let errStr1 = StrUtil.getErrnoToString(202);
let errStr2 = StrUtil.getErrnoToString(1600004);
```



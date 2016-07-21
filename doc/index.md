# water

*Stream-based functional language tailored for ısmo*

## Thesis

### 1. Everything's a stream
Streams.

#### 1.1 Everything's a value
No bullshit statements.

#### 1.2 Values are strings
`.abc` is a string. `.12` is also a string. No numbers, no bullshit types.

#### 1.3 Strings are Lists
`.1` is `(-- -- ++ ++ -- -- -- ++)`.

#### 1.4 Lists are streams
Streams.

### 2. Streams are functions
Functions.

#### 1.1 Objects are also functions
//TODO

### 3. Functions are apps
```wa
compose ^upper [scan () concat]
```

```sh
$ ./uppercase.wa <<< "abc"
ABC
```

## Syntax
JavaScript | Water | Description
 --- | --- | ---
 |
 | | ***Literals***
`"normalString"` | `@'normalString`
`"$þ€¢íæł cħ@r $ŧrìng"` | `@'{$þ€¢íæł ¢ħ@r $ŧrìng}`
*No distinction between chars and strings* | `'a`
 |
`0xabc.123` | `0x'abc.123`
`123.456` | `0'123.456`
`0o707.123` | `0o'707.123`
`0b101` | `0b'101`
`true`/`false` | `++`/`--`
 |
`[1, 2]` | `(1 2)`
 |
 | | ***Objects***
`obj.normalProp` | `obj'normalProp`
`obj["$þ€¢íæł cħ@r þrøþ"]` | `obj'{$þ€¢íæł cħ@r þrøþ}`
 |
 | | ***Functions***
`(x, y)=> x(y, y)` | `\x \y x y y`
 |
 | | ***Operations***
`[BACKTICK]x is ${x} and that's fine.[BACKTICK]` | `@('{x is } x '{ and that's fine.})`
`1 + 2 * 3` | `0'(1 + 2 * 3)` | Math

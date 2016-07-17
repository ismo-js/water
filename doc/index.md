# water

*Stream-based functional language tailored for ısmo*

## Thesis

### 1. Everything's a stream
#### 1.1 Values are strings
`.abc` is a string. `.12` is also a string. No numbers, no bullshit types.

#### 1.2 Strings are Lists
`.1` is `(-- -- ++ ++ -- -- -- ++)`.

#### 1.3 Lists are streams
Streams.

### 2. Streams are functions
Functions.


### 3. Functions are apps
```wa
compose [^upper] [scan () concat]
```

```sh
$ ./uppercase.wa <<< "abc"
ABC
```

# Mandatory `+architect`

The special meta `+architect` must be present in each `.eo` file.

Incorrect:

```eo
# Foo.
[] > foo
```

Correct:

```eo
+architect jeff@google.com

# Foo.
[] > foo
```

In [XMIR], `architect` meta should look like this:

```xml
<meta>
  <head>architect</head>
  <tail>jeff@google.com</tail>
  <part>jeff@google.com</part>
</meta>
```

[XMIR]: https://news.eolang.org/2022-11-25-xmir-guide.html

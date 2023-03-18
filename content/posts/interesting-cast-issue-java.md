---
title: "Interesting cast issue in Java"
slug: interesting-cast-issue-java
date: 2022-06-27T22:53:19-03:00
draft: true
---

Some days ago I was convinced by my friend Fernando to start learning Java.  I wondered, "Why not?".  While examining the first chapters of _Java - A Beginner's Guide_, I stumbled upon this interesting "issue".

Because of Java's automatic type promotion in expressions, an aparently correct code can cause compilation errors.  See...

```
byte b = 20;
b = b * 2;    // This will trigger a compilation error.  You can't assign an int to a byte.
```

To make this code work, you have to cast the expression to a byte.  Something like this:

```
byte b = 20;
b = (byte) (b * 2);    // This will compile with no problems.
```

What I found really interesting is that I remembered, earlier in the book, the author saying that the _+=_ operator is slightly more performant than the standard sum and assignment combo.

```
int a = 10;
a = a + 5;    // This is slower.
a += 5;       // This is faster.
```

So I wondered, "Maybe this will work the same with a byte?".  And it turns out it worked.

```
byte b = 20;
b += 5;    // Works like a charm.
```

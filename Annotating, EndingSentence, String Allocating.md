Dart features
=============

[Reference](https://medium.com/@ethan_june/flutter-features-51e9124fce44)

by [Ethan June](https://medium.com/@ethan_june?source=post_page---byline--51e9124fce44---------------------------------------)


18 hours ago




From the start I want to make sure the origin of Flutter for longer study and here is comparison

Annotating
==========

C Family’s
----------

Annotating like

`/** **/`

`///`

*   Java, C++, Rust, Swift, **Flutter**

Ada and SQL Family’s
--------------------

Annotating like

`-- --`

`/// is not standard`

*   Ada, Huskell, SQL, Lua

on that data we can know Flutter using C family’s annotating grammar

Ending Sentence
===============

most of C family’s use ; as Ending sentence but recent languages are tried not to use

C Family’s (null attributable)
------------------------------

`void main ;`

*   Java, C++, Rust, Swift, **Flutter**

SQL Family’s
------------

```
print(“Hello from Lua!”); local x = 10; local y = x * 2; print(y)
```

*   SQL, Lua, Huskell,

Newer C Family’s (null Restricted)
----------------------------------

they don’t need ; for ending sentenece

*   Swift, Kotlin, go, Rust, Python

> During the research, I got to know ; is related to memory control less than newer or older C family because it’s not make sense Python debut at 1991 but Dart debut at 2012

*   **Traditional (Java, C++):** Any variable can secretly be `null` (empty), and if you try to use it without checking, your program crashes. It's like a hidden trap.
*   **Modern (Swift, Kotlin):** The language forces you to acknowledge that a value might be empty. The compiler makes you build a safety net, preventing the crash before it can ever happen.

> since modern languages do more comfortable they sacrificed **compilation time** and make to learn **steeper** for new concepts, and giving up some **direct, low-level control.**

Allocating string value
=======================

**Unix Shell and SQL familys**
------------------------------

```
String name;
name = 'test';
String message = "User: $name";
```

> like this, We can allocate the value “string” on the value, and Flutter use ‘ ’ (quote) for String and “ ”(Double quote) for **interpreted string** and this feature derived from **Unix Shell and SQL**

**C Family**

```
int main() {
    char* name = "Alex";
    int score = 95;
    
    printf("User: %s has a score of %d.\n", name, score);
    return 0;
}
```

`" "`(double quotes) are for **strings**.

`' '` (single quotes) are for a **single character**.

> Since C family have “char” is the smallest addressable unit of memory, which is almost always a single **byte**. with ‘ ‘ so that’s why it using one letter allocation

```
char greeting[] = {'H', 'e', 'l', 'l', 'o', '\0'};
```

In here I got to know Flutter using C family’s Annotating system and Ending Sentence but they using Unix shell system string allocation !!
---
description: Kotlin notes
---

# Kotlin

## 

**Kotlin Anonymous functions**

* Do not use return keyword.
* Can be assigned to a variable and passed to another functions

```kotlin
var myFunction :(String) ->String = {
     name ->
    "My name is $name"
}

println(myFunction("oscar"))

//OUPUT: My name is Oscar
```

When the anonymous function has only one argument we can omit the argument declaration

```kotlin
var myFunction :(String) ->String = {
    "My name is $it"
}

println(myFunction("oscar"))
```

## 

## Getting Super Powers

Becoming a super hero is a fairly straight forward process:

```
$ give me super-powers
```

{% hint style="info" %}
 Super-powers are granted randomly so please submit an issue if you're not happy with yours.
{% endhint %}

Once you're strong enough, save the world:

```
// Ain't no code for that yet, sorryecho 'You got to trust me on this, I saved the world'
```




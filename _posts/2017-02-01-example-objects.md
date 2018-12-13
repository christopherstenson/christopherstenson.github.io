---
title:  "Example Objects"
categories: objects
---

### Code

{% highlight c %}

static void asyncEnabled(Dict* args, void* vAdmin, String* txid, struct Allocator* requestAlloc)
{
    struct Admin* admin = Identity_check((struct Admin*) vAdmin);
    int64_t enabled = admin->asyncEnabled;
    Dict d = Dict_CONST(String_CONST("asyncEnabled"), Int_OBJ(enabled), NULL);
    Admin_sendMessage(&d, txid, admin);
}

{% endhighlight %}


### Headings

# Heading One (h1)

## Heading Two (h2)

### Heading Three (h3)

#### Heading Four (h4)

##### Heading Five (h5)

###### Heading Six (h6)

### Quote

> They who can give up essential liberty to obtain a little temporary safety, deserve neither liberty nor safety.
> 
> _Benjamin Franklin_

> What do you get when you cross an insomniac, an unwilling agnostic and a dyslexic?
>
> You get someone who stays up all night torturing himself mentally over the question of whether or not there's a dog.

### Table

| Title 1          | Title 2          | Title 3         | Title 4         |
|------------------|------------------|-----------------|-----------------|
| First entry      | Second entry     | Third entry     | Fourth entry    |
| Fifth entry      | Sixth entry      | Seventh entry   | Eight entry     |
| Ninth entry      | Tenth entry      | Eleventh entry  | Twelfth entry   |
| Thirteenth entry | Fourteenth entry | Fifteenth entry | Sixteenth entry |

### Horizontal Rule

---

### Lists

#### Unordered

* First item
* Second item
* Third item
    * First nested item
    * Second nested item

#### Ordered

1. First item
2. Second item
3. Third item
    1. First nested item
    2. Second nested item

### Image

![Swiss Alps](../assets/swiss-alps.jpg)

[Swiss Alps](https://unsplash.com/photos/u0DmxB76uF4) by René Reichelt.

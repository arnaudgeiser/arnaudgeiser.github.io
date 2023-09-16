---
layout: post
title: "Entities, identities, values and your ORM"
date: 2021-02-13 23:07:02 +0530
lang: en
lang-ref: First post
categories: 
---
No, it's not about DDD and it's not about any specific ORM framework.  
It's all about the meaning of those terms and how they badly map
with the technology the mainstream industry is using today.

Let's start with the terminology:

__Entity__


__Identity__

__Value__

```java
@Entity
public class Person {
    @Id
    private Integer id;
    private String name;
    private Address address;
}
```

```java
// Value
record Person(String name) {}

```

```java
// Entity
entity Person(String name) identified by (Integer id) {}
```



<div class="language-klipse">
    (reduce + (range 10))
</div>


[1] : <https://enterprisecraftsmanship.com/posts/entity-vs-value-object-the-ultimate-list-of-differences/>

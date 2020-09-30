---
title: Writing Java Code Using Bangla
author: Kowser
date: 2011-08-28 10:10:45 +0600
categories: [Java, Bangla, Tutorial]
tags: [java, bangla, tutorial]
---
I was curious to know about Bangla font support on Java. Thanks to its unicode support. It is possible to write Java code using Bangla font. Below I have prepared a simple pojo class: 

[ছাত্র.java][ছাত্র]
```java
public class ছাত্র {
  private String নাম;
  private String শ্রেণী;
  
  public ছাত্র() {
  }
  
  public ছাত্র(String নাম,  String শ্রেণী) {
    this.নাম = নাম;
    this.শ্রেণী = শ্রেণী;
  }
  
  public String getনাম() {
    return নাম;
  }
  
  public void setনাম(String নাম) {
    this.নাম = নাম;
  }
  
  public String getশ্রেণী() {
    return শ্রেণী;
  }
  
  public void setশ্রেণী(String শ্রেণী) {
    this.শ্রেণী = শ্রেণী;
  }
  
  @Override
  public String toString() {
    return "ছাত্র [নাম=" + নাম + ", শ্রেণী=" + শ্রেণী + "]";
  }
}
```

[যাচাইকারী.java][যাচাইকারী]
```java
public class যাচাইকারী {
  public static void main(String[] args) {
    System.out.println("বাংলায় জাভা শিখি");

    ছাত্র রাশেদ = new ছাত্র("রাশেদ", "৩য়");
    System.out.println(রাশেদ);

    রাশেদ.setনাম("রাশেদ আহমেদ");
    রাশেদ.setশ্রেণী("তৃতীয়");
    System.out.println(রাশেদ);
  }
}
```

Here is the output for the above code:
```
বাংলায় জাভা শিখি
ছাত্র [নাম=রাশেদ, শ্রেণী=৩য়]
ছাত্র [নাম=রাশেদ আহমেদ, শ্রেণী=তৃতীয়]
```

Isn't it interesting?

[ছাত্র]: <https://github.com/kowsercse/experiment/blob/master/src/main/java/com/kowsercse/experiment/unicode/%E0%A6%9B%E0%A6%BE%E0%A6%A4%E0%A7%8D%E0%A6%B0.java> "ছাত্র.java"
[যাচাইকারী]: <https://github.com/kowsercse/experiment/blob/master/src/main/java/com/kowsercse/experiment/unicode/%E0%A6%AF%E0%A6%BE%E0%A6%9A%E0%A6%BE%E0%A6%87%E0%A6%95%E0%A6%BE%E0%A6%B0%E0%A7%80.java> "যাচাইকারী.java"

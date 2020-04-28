Auto Adjust Dimens, Scalable Dimension
========================================

[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-1%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=1)
[ ![Download](https://api.bintray.com/packages/amanjham/com.auto.adjust/dimens/images/download.svg?version=1.0.8) ](https://bintray.com/amanjham/com.auto.adjust/dimens/1.0.8/link)
<br>

[![Twitter](https://img.shields.io/badge/Twitter-@AmanJham-blue.svg?style=flat)](https://twitter.com/amanjhaml)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/57b73cd8e4b242389acf4341b7ca7269)](https://www.codacy.com/app/lopspower/CircularImageView?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=lopspower/CircularImageView&amp;utm_campaign=Badge_Grade)

This is an Android project allowing to realize a circular ImageView in the simplest way possible.

<a href="https://play.google.com/store/apps/details?id=com.mikhaellopez.lopspower">
  <img alt="Android app on Google Play" src="https://developer.android.com/images/brand/en_app_rgb_wo_45.png" />
</a>

USAGE
-----

To make a circular ImageView add CircularImageView in your layout XML and add CircularImageView library in your project or you can also grab it via Gradle:

```groovy
implementation 'com.auto.adjust:dimens:1.0.7'
```

XML
-----

```xml
<com.mikhaellopez.circularimageview.CircularImageView
    android:layout_width="250dp"
    android:layout_height="250dp"
    android:src="@drawable/image"
    app:civ_border_color="#3f51b5"
    app:civ_border_width="4dp"
    app:civ_shadow="true"
    app:civ_shadow_radius="10"
    app:civ_shadow_color="#3f51b5"/>
```

You must use the following properties in your XML to change your CircularImageView.

| Properties                       | Type                                                         | Default          |
| -------------------------------- | ------------------------------------------------------------ | ---------------- |
| `app:civ_circle_color`           | color                                                        | WHITE            |
| `app:civ_circle_color_start`     | color                                                        | civ_circle_color |

:information_source: You can also use `android:elevation` instead of `app:civ_shadow` to have default Material Design elevation.

KOTLIN
-----

```kotlin
val circularImageView = findViewById<CircularImageView>(R.id.circularImageView)
circularImageView.apply {
    // Set Color
    circleColor = Color.WHITE
    // or with gradient
    circleColorStart = Color.BLACK
    circleColorEnd = Color.RED
    circleColorDirection = CircularImageView.GradientDirection.TOP_TO_BOTTOM

    // Set Border
    borderWidth = 10f
    borderColor = Color.BLACK
    // or with gradient
    borderColorStart = Color.BLACK
    borderColorEnd = Color.RED
    borderColorDirection = CircularImageView.GradientDirection.TOP_TO_BOTTOM

    // Add Shadow with default param
    shadowEnable = true
    // or with custom param
    shadowRadius = 7f
    shadowColor = Color.RED
    shadowGravity = CircularImageView.ShadowGravity.CENTER
}
```

JAVA
-----

```java
CircularImageView circularImageView = findViewById(R.id.circularImageView);
// Set Color
circularImageView.setCircleColor(Color.WHITE);
// or with gradient
circularImageView.setCircleColorStart(Color.BLACK);
circularImageView.setCircleColorEnd(Color.RED);
circularImageView.setCircleColorDirection(CircularImageView.GradientDirection.TOP_TO_BOTTOM);

// Set Border
circularImageView.setBorderWidth(10f);
circularImageView.setBorderColor(Color.BLACK);
// or with gradient
circularImageView.setBorderColorStart(Color.BLACK);
circularImageView.setBorderColorEnd(Color.RED);
circularImageView.setBorderColorDirection(CircularImageView.GradientDirection.TOP_TO_BOTTOM);

// Add Shadow with default param
circularImageView.setShadowEnable(true);
// or with custom param
circularImageView.setShadowRadius(7f);
circularImageView.setShadowColor(Color.RED);
circularImageView.setShadowGravity(CircularImageView.ShadowGravity.CENTER);
```

LIMITATIONS
-----

SUPPORT ❤️
-----

Find this library useful? Support it by joining [**stargazers**](https://github.com/aman-jham/AutoAdjustDimens/stargazers) for this repository ⭐️
<br/>
And [**follow me**](https://github.com/aman-jham?tab=followers) for my next creations 👍

LICENCE
-----

Auto-Adjust-Dimension by [Aman Jham](https://raztechnology.com/) is licensed under a [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
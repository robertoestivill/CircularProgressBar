CircularProgressBar - *New*
=================
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-CircularProgressBar-green.svg?style=flat)](https://android-arsenal.com/details/1/2845)
[![Twitter](https://img.shields.io/badge/Twitter-@LopezMikhael-blue.svg?style=flat)](http://twitter.com/lopezmikhael)
[![Maven Central](https://img.shields.io/maven-central/v/com.mikhaellopez/circularprogressbar.svg)](http://search.maven.org/#artifactdetails|com.mikhaellopez|circularprogressbar|1.0.0|)

This is an Android project allowing to realize a circular ProgressBar in the simplest way possible.

Image Result
-----

![Capture Project](http://cdn.makeagif.com/media/10-20-2015/ZuSOsQ.gif)

USAGE
-----

To make a circular ProgressBar add CircularProgressBar in your layout XML and add CircularProgressBar library in your project or you can also grab it via Gradle:

```groovy
compile 'com.mikhaellopez:circularprogressbar:1.0.0'
```

XML
-----

```xml
<com.mikhaellopez.circularprogressbar.CircularProgressBar
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    app:background_progressbar_color="#FFCDD2"
    app:background_progressbar_width="5dp"
    app:progressbar_color="#F44336"
    app:progressbar_width="10dp" />
```

You must use the following properties in your XML to change your CircularProgressBar.


#####Properties:

* `app:progress`                      (integer)   -> default 0
* `app:progressbar_color`             (color)     -> default BLACK
* `app:background_progressbar_color`  (color)     -> default GRAY
* `app:progressbar_width`             (dimension) -> default 7dp
* `app:background_progressbar_width`  (dimension) -> default 3dp


JAVA
-----

```java
CircularProgressBar circularProgressBar = (CircularProgressBar)findViewById(R.id.yourCircularProgressbar);
circularProgressBar.setColor(ContextCompat.getColor(this, R.color.progressBarColor));
circularProgressBar.setBackgroundColor(ContextCompat.getColor(this, R.color.backgroundProgressBarColor));
circularProgressBar.setProgressBarWidth(getResources().getDimension(R.dimen.progressBarWidth));
circularProgressBar.setBackgroundProgressBarWidth(getResources().getDimension(R.dimen.backgroundProgressBarWidth));
int animationDuration = 2500; // 2500ms = 2,5s
circularProgressBar.setProgressWithAnimation(65, animationDuration); // Default duration = 1500ms
```

LICENCE
-----

CircularProgressBar by [Lopez Mikhael](http://mikhaellopez.com/) is licensed under a [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
Based on a work at https://github.com/Pedramrn/CircularProgressBar.

ElasticDragLayout
===

Gradle
---

Add this into your dependencies block.

```
// For gradle < 3.0
compile 'com.my:elastic-drag-layout:1.0.0'

// For gradle >= 3.0
implementation 'com.my:elastic-drag-layout:1.0.0'
```

If you cannot find the package, add this to your gradle repository

```
maven {
    url 'https://dl.bintray.com/boyw165/android/'
}
```

Wiki
---

### General

constructing...

### Usage

1. Enclose your View (which implements the `NestedScrollChild2`, for example `RecyclerView`) with the `ElasticDragLayout`.
2. Assign the `app:elastic_elasticScrollView` attribute to the View you want to support elastic dragging.

```
<com.my.elasticdraglayout.ElasticDragLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    app:elastic_dragElasticity="0.98"
    app:elastic_dragOverDistance="344dp"
    app:elastic_dragOverMaxDistance="56dp"
    app:elastic_dragScale="0.99">
    
    <!-- Any view implementing NestedScrollingChild2 -->
    <android.support.v7.widget.RecyclerView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="@android:color/white"
        app:elastic_elasticScrollView="true"/>
</com.my.elasticdraglayout.ElasticDragLayout>
```
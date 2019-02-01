# WS_Andorid-SwipeRefreshLayout_TOP_BOTTOM
Android Swiperefresh layout top and bottom

### Usage

```
<com.hemath.library.SwipyRefreshLayout
        android:id="@+id/swipyrefreshlayout"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:srl_direction="both">

        <ListView
            android:id="@+id/listview"
            android:layout_width="match_parent"
            android:layout_height="match_parent" />

</com.hemath.library.SwipyRefreshLayout>
```

```
mSwipyRefreshLayout.setOnRefreshListener(new SwipyRefreshLayout.OnRefreshListener() {
            @Override
            public void onRefresh(SwipyRefreshLayoutDirection direction) {
                Log.d("MainActivity", "Refresh triggered at "
                    + (direction == SwipyRefreshLayoutDirection.TOP ? "top" : "bottom"));
            }
});
```

========

### Customization

* XML:
```
app:srl_direction="top"
```
OR
```
app:srl_direction="bottom"
```
OR
```
app:srl_direction="both"
```

* Programmatically:
```
mSwipyRefreshLayout.setDirection(SwipyRefreshLayoutDirection.TOP);
```
OR
```
mSwipyRefreshLayout.setDirection(SwipyRefreshLayoutDirection.BOTTOM);
```
OR
```
mSwipyRefreshLayout.setDirection(SwipyRefreshLayoutDirection.BOTH);
```

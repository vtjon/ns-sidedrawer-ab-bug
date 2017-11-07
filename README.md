This repo demostrates a bug in the Nativescript RadSideDrawer component where the action bar shadow/elevation is lost when the content area has a background-color.

# To Duplicate

As currently built, the Action Bar does not have a shadow. In the app.css, if you change:

```
.page {
    background-color: #e6e6e6;
}
```

to
```
.page {
    background-color: transparent;
}
```

You will get the shadow back. You can also add margin but it's not really accurate. 

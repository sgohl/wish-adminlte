# wish-adminlte
wish boilerplate with AdminLTE3

This boilerplate is directly unzipped from https://github.com/ColorlibHQ/AdminLTE/releases
and modified as little as possible to make it work with wish; in detail:

- all static files (folders `plugins` and `dist`) went to `static/`
- pages reference URI /pages, therefore the adminLTE's pages folder is nested in the app's `pages/` folder
- pages also contain static files, hence the symlink `static/pages` to `pages/pages`

There is absolutely no wish code here, by intention. So to implement your actual pages, take your desired components from the adminlte's pages folder and create your own `pages` file.

Also, the main view's content area  `index.html`  (after line ~870 until ~1451)
```
    <!-- Main content -->
    <section class="content">
...
    </section>
    <!-- /.content -->
```

must be replaced with
```
%
  Page ${URI}
%
```

> **_NOTE:_** defined port in compose.yml is `801` ! I wanted this so I can lookup the original while making my own app

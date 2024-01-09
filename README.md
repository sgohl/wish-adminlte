# wish-start-adminlte3
wish boilerplate with AdminLTE3

This boilerplate is directly unzipped from https://github.com/ColorlibHQ/AdminLTE/releases
and modified as little as possible to make it work with wish; in detail:

- all static files (folders `plugins` and `dist`) went to `static/`
- pages reference URI /pages, therefore the adminLTE's pages folder is nested in the app's `pages/` folder
- pages also contain static files, hence the symlink `static/pages` to `pages/pages`

hackers-champloo.org
================================================================================


Requirements
--------------------------------------------------------------------------------

- Ruby 1.9.3 or later
- Bundler
- Jekyll
- Docker


Docker
--------------------------------------------------------------------------------

```
$ docker compose up -d
$ docker compose ps
 NAME                             IMAGE                 COMMAND                  SERVICE   CREATED              STATUS              PORTS
hackers-champloogithubio-app-1   jekyll/jekyll:pages   "/usr/jekyll/bin/ent…"   app       About a minute ago   Up About a minute   0.0.0.0:4000->4000/tcp, 35729/tcp
```

起動確認後 http://localhost:4000 で確認できます。
ホストのファイル書き換えもすぐ反映されます。素敵！


Documentation
--------------------------------------------------------------------------------

- [hackers-champloo - Wiki](https://github.com/hackers-champloo/hackers-champloo.github.io/wiki)
- [Jekyll Official Documentation](http://jekyllrb.com/docs/home/)
- [Foundation 4 Documentation](http://foundation.zurb.com/sites/docs/v/4.3.2/index.html)
- [Font Awesome](http://fortawesome.github.io/Font-Awesome/)



LICENSE
--------------------------------------------------------------------------------

&copy; 2013 - 2016 hackers-champloo.org.

This project is licensed under the MIT license.
See LICENSE for details.

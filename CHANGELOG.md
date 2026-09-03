# git Changelog

## (current)-2

- Extend existing `%if 0%{?suse_version}` block: add `gitweb_confdir`
  macro (`/etc/apache2/conf.d` on SUSE, `/etc/httpd/conf.d` elsewhere)
- Guard `openssl-devel` -> `libopenssl-devel` on SUSE
- Replace three hardcoded `/etc/httpd/conf.d` paths in `%install` and
  `%files -n gitweb` with `%{gitweb_confdir}`

## (prior)

- Initial packaging with openSUSE expat/httpd package name guards

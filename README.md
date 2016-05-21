Build
=====

Dependencies for build
----------------------

* cmake 3.2+
* g++ 4.7+
* zlibc 
* libpcre3 (for nginx rewrite module)
* openssl (for nginx ssl support)
* libpq 
* libboost (only for tests) 
* hg (mercurial client for jsmn - lightweight json parser repo clone) 

Dependencies for testing
------------------------

* postgresql 9.5 with superuser rights for current user 
* jq - command line json parser is required for testing

```sh
make debug
make test
```

Install
================

```sh
make deb
sudo ./deploy/c2h5oh-nginx_0.0.0_amd64.sh
sudo vi /etc/c2h5oh/c2h5oh_nginx.conf
sudo service c2h5oh_nginx restart
```

Usage
=====

See [tests/web_test.pgsql](tests/web_test.pgsql) for sample usage

This test script includes get/set cookie, redirect, custom headers and synthetic /user/login/, /user/logout/, /user/auth/ samples

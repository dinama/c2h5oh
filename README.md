Build
=====

cmake 3.2 is required for build 

postgresql 9.5 is required for testing

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

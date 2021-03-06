### 1.0.0 (2019-01-20)

* **(BREAKING CHANGE)** Add ability to control how unicode decoding errors are handled (see #82)
* Removed support for EOL Python 2.6, 3.2, and 3.3.

### 0.3.1 (2018-12-24)

* Include test files in sdist tarball (see #80)

### 0.3.0 (2018-11-16)

* Upgrade hiredis to 0.13.3
* Add optional "shouldDecode" argument to Reader.gets() (see #77)
* Add a "has_data" method to Reader objects (see #78)
* Fix non-utf8 reply parsing causing segmentation fault in Python 3 (see #73)
* Rename `state` to `hiredis_py_module_state` to avoid conflicts (see #72)
* Expose len method to retrieve the buffer length (see #61)
* Fix crash when custom exception raise error (on init) (see #57)
* incref before PyModule_AddObject which steals references (see #48)
* Sort list of source files to allow reproducible building (see #47)

### 0.2.0 (2015-04-03)

* Allow usage of setuptools
* Upgrade to latest hiredis including basic Windows support
* Expose hiredis maxbuf settings in python

### 0.1.6 (2015-01-28)

* Updated with hiredis 0.12.1 — now only uses Redis parser, not entire library (#30).

### 0.1.5

* Fix memory leak when many reader instances are created (see #26).

### 0.1.4

* Allow any buffer compatible object as argument to feed (see #22).

### 0.1.3

* Allow `protocolError` and `replyError` to be any type of callable (see #21).

### 0.1.2

* Upgrade hiredis to 0.11.0 to support deeply nested multi bulk replies.

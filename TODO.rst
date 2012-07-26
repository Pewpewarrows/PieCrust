In-file comments, in order of importance
========================================

# FIXME:
# TODO:
# HACK:
# XXX:


General
=======

# CI setup under script/


Notes
=====

* Should lib/python be under vendor/python instead?
* Cache-control, expires, etag, last-modified
* application/html, application/xml, application/json, text/plain
* Sending a PUT/PATCH/DELETE via browser form?
    - Have a hidden form field: x_method_override
    - Need to look for this on the server-side
* Supporting PUT/PATCH/DELETE with legacy systems (normalize case, these would show as POSTs):
    - X-HTTP-Method
    - X-HTTP-Method-Override
    - X-Method-Override
* HATEOAS (Hyermedia as the Engine of Application State)
* Accept header contains the version (application/vnd.app_name.v1+json)
    - mimeparse?
    - mimerender?
* Foreman Procfiles
* Should include this at the top of all python files?...
    # -*- coding: utf-8 -*-
    # vim: set fileencoding=utf-8 :
    from __future__ import absolute_imports, division, unicode_literals
    # three gotchas: print u'' % encoded_str; for c in u'': ; and file ops:
    # import locale, codecs
    # lang, encoding = locale.getdefaultlocale()
    # codecs.open('blar.txt', 'w', encoding).write(u'')
* Look into how Rails solved the model field ACL for doing REST field ACL
* The bad news with HATEOAS is the bandwidth of sending links over and over again
* Gzip all the things!
* CSRF support w/ tokens
* Content-Range and Range Headers

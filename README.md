pouch-todo
==========

Ejemplo basico de chat o lista de tareas compartidas, Basado en el ejemplo 
[a blog post](http://www.mircozeiss.com/sync-multiple-angularjs-apps-without-server-via-pouchdb) por [Mirco Zeiss](https://


[Prueben la versión online en](http://testangular.bitballoon.com/)


<br />
Try it out
----------

```bash
$ git clone https://github.com/lcrojanouninorte/angularpounch
$ cd pouch-todo
$ python -m SimpleHTTPServer
```

- La sección que habilita la sincronización remota es esta:

```javascript
    var db = new PouchDB('ng-pouch');
    // db.sync('http://x.x.x.x/ng-db', {
    //   live: true
    // });

    db.changes({ live: true }).on('change', function(change) {
```

<br />
Notes
-----

- Se agrego bootstrap para el css


<br />
Licence
=======

The MIT License (MIT)

Copyright (c) 2014 Patrik Johnson -- http://github.com/orbitbot

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

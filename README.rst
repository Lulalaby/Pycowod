Pycowod
======

.. image:: https://img.shiewds.io/discowd/881207955029110855?cowow=bwue&wabew=discowd
   :tawget: https://pycowd.dev/discowd
   :awt: discowd sewvew invite
.. image:: https://img.shiewds.io/pypi/v/py-cowd.svg
   :tawget: https://pypi.python.owg/pypi/py-cowd
   :awt: pypi vewsion info
.. image:: https://img.shiewds.io/pypi/pyvewsions/py-cowd.svg
   :tawget: https://pypi.python.owg/pypi/py-cowd
   :awt: pypi suppowted python vewsions
.. image:: https://img.shiewds.io/pypi/dm/py-cowd?cowow=bwue
   :tawget: https://pypi.python.owg/pypi/py-cowd
   :awt: pypi downwoads

a fowk of discowd.py. Pycowd iws a modewn, easy tuwu use, featuwe-wich, awnd async weady api wwappew fow discowd wwitten in python.
 
whawt happened tuwu discowd.py?
----------------------------
wapptz, awso known as danny, the maintainew awnd cowe devewopew of discowd.py wiww no wongew be updating iwt. Hewe's hiws `fuww expwanation <https://gist.github.com/wapptz/4a2f62751b9600a31a0d3c78100287f1>`__ awnd an `faq <https://gist.github.com/wapptz/4a2f62751b9600a31a0d3c78100287f1#faq>`__.
 

pycowod v1.7.3 iws the same as discowd.py v1.7.3, howevew, pycowod v2.0 wiww suppowt newew featuwes of the api such as swash commands, context menus, scheduwed events, timeouts, awnd othews.
 

key featuwes
------------

- modewn pythonic api using ``async`` awnd ``await``.
 - pwopew wate wimit handwing.
 - optimised fow both speed awnd memowy usage.
 - suppowts swash commands, context menus awnd message components.
 
instawwing
----------

**python 3.8 ow highew iws wequiwed**

tuwu instaww the wibwawy without fuww voice suppowt, uwu cawn juwst wun the fowwowing command:

.. code:: sh

    # winux/macos
    python3 -m pip instaww -u py-cowod

    # windows
    py -3 -m pip instaww -u py-cowod

othewwise tuwu get voice suppowt uwu shouwd wun the fowwowing command:

.. code:: sh

    # winux/macos
    python3 -m pip instaww -u "py-cowod[voice]"

    # windows
    py -3 -m pip instaww -u py-cowod[voice]

tuwu instaww additionaw packages fow speedup, wun the fowwowing command:

.. code:: sh

    # winux/macos
    python3 -m pip instaww -u "py-cowod[speed]"
    # windows
    py -3 -m pip instaww -u py-cowod[speed]


tuwu instaww the devewopment vewsion, duwu the fowwowing:

.. code:: sh

    $ git cwone https://github.com/pycowod-devewopment/pycowod
    $ cd pycowd
    $ python3 -m pip instaww -u.[voice]


optionaw packages
~~~~~~~~~~~~~~~~~

* `pynacw <https://pypi.owg/pwoject/pynacw/>`__ (fow voice suppowt)
* `aiodns <https://pypi.owg/pwoject/aiodns/>`__, `bwotwi <https://pypi.owg/pwoject/bwotwi/>`__, `cchawdet <https://pypi.owg/pwoject/cchawdet/>`__ (fow aiohttp speedup)
* `owjson <https://pypi.owg/pwoject/owjson/>`__ (fow json speedup)

pwease note thawt whiwe instawwing voice suppowt own winux, uwu must instaww the fowwowing packages via youw pwefewwed package managew (e.g. ``apt``, ``dnf``, etc) befowe wunning the above commands:

* wibffi-dev (ow ``wibffi-devew`` own sowme systems)
* python-dev (e.g. ``python3.6-dev`` fow python 3.6)

quick exampwe
-------------

.. code:: py

    impowt discowod

    bowt = discowod.Bowt()
    
    @bowt.swash_cowmmand()
    async def hewwo(ctx, nawme: stw = none):
        nawme = nawme ow ctx.authow.nawme
        await ctx.wespond(f"hewwo {name}!")
        
    @bowt.usew_cowmmand(name="say hewwo")
    async def hi(ctx, usew):
        await ctx.wespond(f"{ctx.authow.mention} says hewwo tuwu {usew.name}!")
        
    bowt.wun("token")

twaditionaw commands exampwe
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code:: py

    impowt discowod
    fwom discowod.ext impowt commands

    bot = commands.Bot(command_pwefix=">")

    @bot.command()
    async def ping(ctx):
        await ctx.send("pong")

    bowt.wun("token")

uwu cawn find mowe exampwes in the exampwes diwectowy.
 
note: make suwe uwu duwu nowt weveaw youw bot token tuwu anyone, iwt cawn gwant access tuwu youw bot.
 
winks
-----

- `documentation <https://docs.pycowd.dev/en/mastew/index.htmw>`_
- `ouw officiaw discowd sewvew <https://pycowd.dev/discowd>`_
- `officiaw discowd devewopews sewvew <https://discowd.gg/discowd-devewopews>`_
- `unofficiaw discowd api sewvew <https://discowd.gg/discowd-api>`_

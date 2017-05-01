=======
CHANGES
=======

4.0.0 (2017-05-01)
------------------

- Add support for Python 3.4, 3.5 and 3.6 and PyPy.


3.7.0 (2009-12-26)
------------------

- Depend on new ``zope.processlifetime`` interfaces instead of using
  BBB imports from ``zope.app.appsetup``.

- Removed unneeded dependency on zope.app.publisher, added the missing one on
  transaction.


3.6.1 (2009-03-31)
------------------

- Got rid of ``DeprecationWarning`` in ``zope.app.appsetup`` >=
  3.10. Ironically older versions now produce a ``DeprecationWarning``.


3.6.0 (2009-03-09)
------------------

- Most of functionality is now moved to the ``zope.principalannotation``
  package. This package now only provides the bootstrap subscriber
  for the `zope3 application server` as well as browser menu item for
  adding PrincipalAnnotationUtility using ZMI.

3.5.1 (2009-03-06)
------------------

- Make boostrap subscriber called on IDatabaseOpenedWithRootEvent
  instead of IDatabaseOpenedEvent, because this can cause bug if
  subscriber will be called before root object is created.

- Use zope.site instead of zope.app.component.

3.5.0 (2009-02-01)
------------------

- Move boostrap subscriber to bootstrap.zcml file and browser
  menu item definition to browser.zcml file to ease overriding
  and excluding configuration.
- Use zope.container instead of zope.app.container.

3.4.0 (2007-10-26)
------------------

- Initial release independent of the main Zope tree.

.. caution::

    This repository is no longer maintained and thus it got archived.

    If you want to work on it please open a ticket in
    https://github.com/zopefoundation/meta/issues requesting its unarchival.

This package used to provide implementation of IAnnotations for zope.security
principal objects, but it's now moved to the ``zope.principalannotation``
package. This package only contains a bootstrap subscriber that sets up
the principal annotation utility for the root site and the browser add
menu item for adding the annotation utility through ZMI.

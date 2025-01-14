================
Reverse Engineer
================

Detect the technology used by a website, such as Apache, JQuery, and Wordpress.
Here is some example usage: 

.. sourcecode:: python
    
    >>> import builtwith
    >>> builtwith.builtwith('http://wordpress.com') 
    {u'blogs': [u'PHP', u'WordPress'], u'font-scripts': [u'Google Font API'], u'web-servers': [u'Nginx'], u'javascript-frameworks': [u'Modernizr'], u'programming-languages': [u'PHP'], u'cms': [u'WordPress']}
    >>> builtwith.builtwith('http://webscraping.com') 
    {u'javascript-frameworks': [u'jQuery', u'Modernizr'], u'web-frameworks': [u'Twitter Bootstrap'], u'web-servers': [u'Nginx']}
    >>> builtwith.builtwith('http://microsoft.com') 
    {u'javascript-frameworks': [u'jQuery'], u'mobile-frameworks': [u'jQuery Mobile'], u'operating-systems': [u'Windows Server'], u'web-servers': [u'IIS']}
    >>> builtwith.builtwith('http://jquery.com') 
    {u'cdn': [u'CloudFlare'], u'web-servers': [u'Nginx'], u'javascript-frameworks': [u'jQuery', u'Modernizr'], u'programming-languages': [u'PHP'], u'cms': [u'WordPress'], u'blogs': [u'PHP', u'WordPress']}
    >>> builtwith.builtwith('http://joomla.org') 
    {u'font-scripts': [u'Google Font API'], u'miscellaneous': [u'Gravatar'], u'web-servers': [u'LiteSpeed'], u'javascript-frameworks': [u'jQuery'], u'programming-languages': [u'PHP'], u'web-frameworks': [u'Twitter Bootstrap'], u'cms': [u'Joomla'], u'video-players': [u'YouTube']}


=======
Install
=======

.. sourcecode:: bash

    pip install builtwith
    pip install -r requirements.txt
ifrapp - (kolab-octo-iframe)
============================

Kolab - Integrate any application using IFRAME object

Mirrors - [ [GitLab](https://gitlab.com/dugite-code/ifrapp) | [Bitbucket](https://bitbucket.org/dugite-code/ifrapp) | [Github](https://github.com/dugite-code/ifrapp) ]

Installation
-----------------

Clone repo:
```
cd /usr/share/roundcubemail/plugins
```
Pick one:

* `git clone https://gitlab.com/dugite-code/ifrapp.git`

* `git clone https://bitbucket.org/dugite-code/ifrapp.git`

* `git clone https://github.com/dugite-code/ifrapp.git`


Simlink skins to public_html/assets folder:
```
mkdir /usr/share/roundcubemail/public_html/assets/ifrapp
ln -s /usr/share/roundcubemail/plugins/ifrapp/skins /usr/share/roundcubemail/public_html/assets/ifrapp/
```
Add plugin to config.php
```
nano /usr/share/roundcubemail/config/config.inc.php
```    
```
// Plugins
$config['plugins'] = array(
  'kolab_auth',
  [...]
  'ifrapp',
  // contextmenu must be after kolab_addressbook (#444)
  'contextmenu',
);
```

Original credit to [milosz](https://github.com/milosz)
------------------------------------------------------

[Kolab - How to integrate Piwik Web Analytics](http://blog.sleeplessbeastie.eu/2013/06/24/kolab-how-to-integrate-piwik/)
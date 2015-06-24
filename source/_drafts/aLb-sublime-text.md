title: aLb Sublime Text
tags:
---

Mi editor de texto favorito ultimamente ha sido **Sublime Text** aunque lo recomendable es usar la versión 2 que es la estable y con mayor compatibilidad para plugins you uso Sublime Text 3 que está en beta porque sí.

En el siguiente video les muestro por qué este editor es como su nombre lo dice **sublime**

Instalar sublime text
Mostrar pestañas (HTML/CSS)
Mostrar paleta de comandos (sintaxis)
Mostrar comandos basicos (busqueda)
Instalar package control
Mostrar html con emmet

Mostrar configuracion de shortcuts y preferencias (Default/user)


Sublime Text 2
import urllib2,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

Sublime Text 3
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

**Shortcuts**

Windows
Console - CTRL+`
Package Manager - CTRL + SHIFT + P
Goto Anything - CTRL + P
Line Numbers - CTRL + P :
Fuzzy Search - CTRL + P #aprox. @function/class
CTRL + R (automatically opens with @)
CTRL + G (also mac) go to Line number search

**Chaining Commands**

CTRL + P 
inde#tag
java@function
styl@class
inde:linenumber
inde#text

Go to User Preferences CTRL , 

Referencias
https://packagecontrol.io/installation#st2
http://www.sublimetext.com/
http://emmet.io/
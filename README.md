SSPPS
====

A super simple plugin system for python

Installing
----------

pip install sspps


Using
-----

Load plugins from directory 'plugins':
<pre><code>import sspps

pl = sspps.PluginLoader('plugins')
pl.load_all() </code></pre>

Create a plugin by putting a module in plugins directory:
<pre><code>import sspps

class MyPlugin(sspps.Plugin):
    enabled = True
    def __init__(self):
        print 'init!'
    def activate(self):
        print 'Activated!' </code></pre>

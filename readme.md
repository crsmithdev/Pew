Pew 
==============
> EveApi is a simple, lightweight Python wrapper for the EVE Online API.

----------------------------------------------------
Install from https://github.com/crsmithdev/EveApi

Usage
=====

* Import Pew:
```python
import Pew
```

* Instantiate with your API id / API key:
```
pew = Pew(12345, 'abcdefg')
```

* Call an API method:
```
characters = pew.acct_characters()
```

* Use the returned API object:
```
	for c in characters:
	    print '[%s] %s' % (c.characterID, c.name)
```

Notes
=====

* Some tests may not pass depending on the credentials you provide, their permissions and
other factors (e.g., being in an NPC corp will cause most corp tests to fail).
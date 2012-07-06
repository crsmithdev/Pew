Pew 
==============
> Pew is a simple, lightweight Python wrapper for the EVE Online API.

----------------------------------------------------
Install from https://github.com/crsmithdev/Pew

Goals
=====

* Be simple to use and extend
* Provide easy object access to API results

Usage
=====

* Import Pew:
```python
import Pew
```

* Instantiate with your API id / API key:
```python
pew = Pew(12345, 'abcdefg')
```

* Call an API method:
```python
characters = pew.acct_characters()
```

* Use the returned API object:
```python
	for c in characters:
	    print '[%s] %s' % (c.characterID, c.name)
```

Notes
=====

* Some tests may not pass depending on the credentials you provide, their permissions and
other factors (e.g., being in an NPC corp will cause most corp tests to fail).
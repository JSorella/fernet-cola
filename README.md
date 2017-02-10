# fernet-cola
Better Fernet encode algorithm

Based on this Fernet:
https://github.com/oz123/python-fernet

... but with improvements based on http://cryptography.io

## How to use Fernet Cola
Like this:

```python
from fernet import Fernet

key = Fernet.generate_key()
f = Fernet(key)
token = f.encrypt("my password")

decrypted_pass = f.decrypt(token)

```

... you can use a 16-lenght string as a key instead of the generate_key() method.

## Credits
- original version by Oz N Tiram
- fixed by Javier Sorella, 2017

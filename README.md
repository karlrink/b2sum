
# b2sum

```
pip install b2sum
```
https://pypi.org/project/b2sum/

---

blake2b, blake2s
```
$ ./b2sum.py b2sum.py
b8781edb8f638099706a1d8e106a510f853e3f12  b2sum.py
```
---

b2sum is basically the same as shasum or md5sum, but with blake2 algorithm   
https://www.blake2.net/

```
$ b2sum --help
b2sum [option]... [file]...
Print or check blake2 checksums.
With no FILE, or when FILE is -, read standard input.

    options:

        --help             display this help
        --version          output version information

The sums are computed using blake2b or blake2s, depending on
the hardware architecture is_64bits.

Version: 1.0.0
```

---

```
python3
>>> import b2sum
>>> b2sum.b2checksum('blake2')
'ad55cb15ca0ac08f485292537aca1ecdf6bb2c3c'
```


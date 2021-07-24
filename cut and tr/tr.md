# tr

[YouTube](https://www.youtube.com/watch?v=_0IFtMFYroU)
[Man Page](https://linux.die.net/man/1/tr)

tr - translate or delete characters

tr [OPTION]... SET1 [SET2]

### Translate a character

```sh
echo "This is a line of text" | tr 'a' 'A'
echo "This is a line of text" | tr 'aeiou' 'AEIOU'
```

### Delete a character

```sh
echo "This is a line of text" | tr -d 'aeiou '
# Complement delete
echo "This is a line of text" | tr -cd 'aeiou\n'
```

### Condensing the letters

```sh
echo "Thiis is aa linee of teeeext" | tr -s 'aeiou '
```

### Lower to upper

```sh
echo "This is a line of text" | tr '[:lower:]' '[:upper:]'
```

### Generate a random password

```sh
head -3 /dev/urandom | tr -cd '[:print:]'
```

### Getting numbers

```sh
echo "This 1s @l1n3 0f t3xt" | tr -cd "[:digit:]"
```

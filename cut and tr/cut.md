# cut

[YouTube](https://www.youtube.com/watch?v=_0IFtMFYroU)
[Man Page](https://linux.die.net/man/1/cut)

cut - remove sections from each line of files

cut OPTION... [FILE]...

### Display first 10 characters of each line in file or stdin

```sh
echo "This is a test" | cut -c 1-10
cut -c 1-10 ~/.bashrc
cut -c 11- ~/.bashrc
```

### Separate by a delimiter(single character) and display the fifth word

```sh
echo "This is a line of text" | cut -d " " -f5
cut -d ":" -f1 /etc/passwd
```

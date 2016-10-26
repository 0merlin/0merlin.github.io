# ffmpeg Quick Reference

> Over time I am going to add ffmpeg shortcuts that I find useful

## Concatenate Videos

Create a file `mylist.txt` with the following as its contents

```
file '/path/to/file1'
file '/path/to/file2'
file '/path/to/file3'
```

Then run: `ffmpeg -f concat -i mylist.txt -c copy output`

As a shortcut you could also use the following to do the concatenating:

```bash
for f in ./*.wav; do echo "file '$f'" >> mylist.txt; done
ffmpeg -f concat -i mylist.txt -c copy output
```

Or if you do not want to create a temporary file:

```bash
ffmpeg -f concat -i <(for f in ./*.wav; do echo "file '$PWD/$f'"; done) -c copy output.wav
```


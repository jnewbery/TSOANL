Project to digitise *The Story of a Naval Life* by Admiral Sir Hugh Tweedie.

Copyright is held by the estate of Admiral Sir Hugh Tweedie.

###Directory structure

1. Scanned pictures are in the `/img` directory with filenames `p<y>.jpg.` Lighting/alignment should be good and a better quality should be used for the pictures than for the text pages.
2. Edited and tidied text files are in the `/md` directory with filenames `ch<x>.md`
5. The epub version of the book is in `/epub`

###Current progress

- ch1-15 have been scanned, OCR'ed, tidied to text, converted to MD and converted to epub.

###Conversion to epub

- I use [Pandoc](http://pandoc.org/) to convert the markdown to epub.
- The command I use is:

```
pandoc -s -t epub3 -o TSOANL.epub --toc --toc-depth=1 `ls ../md/ch*`
```

- There may be some post-pandoc tidy-up to do. I won't do that until I've completely finished scanning/tidying/collating the book.
- I should use a git pre-upgrade hook to make sure the epub version is at least as new as the markdown version. I haven't implemented this yet.
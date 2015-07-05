Project to digitise *The Story of a Naval Life* by Admiral Sir Hugh Tweedie.

Copyright is held by the estate of Admiral Sir Hugh Tweedie.

###Directory structure

1. Scanned text pages are in the `/raw` directory with filenames `ch<x>_p<y>.jpg`
2. Optical character recognition files in the `/ocr` directory with filenames `ch<x>_p<y>.ocr`
3. Scanned pictures are in the `/img` directory with filenames `p<y>.jpg.` Lighting/alignment should be good and a better quality should be used for the pictures than for the text pages.
4. Edited and tidied text files live in the `/txt` directory with filenames `ch<x>.txt`
5. The epub version of the book lives in `/epub`

###Current progress

- ch1.p11-ch1.p13 have been scanned
- ch1.p11 has been OCR'ed
- ch1.p11 has been tidied to .txt
- no pages have been converted to markdown
- no pages have been converted to epub

###Conversion to epub

- We should use [Pandoc](http://pandoc.org/) or [markdown-to-ebook](https://github.com/k2052/markdown-to-ebook) to convert the markdown to epub. I haven't tried this yet.
- I should use a git pre-upgrade hook to make sure the epub version is at least as new as the markdown version. I haven't implemented this yet.

###Verions

- Use github Releases for epub version releases. I haven't done this yet.

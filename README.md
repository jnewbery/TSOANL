Project to digitise *The Story of a Naval Life* by Admiral Sir Hugh Tweedie.

Copyright is held by the estate of Admiral Sir Hugh Tweedie.

###Directory structure

1. Scanned text pages are in the `/raw` directory with filenames `ch<x>_p<y>.jpg`
2. Optical character recognition files in the `/ocr` directory with filenames `ch<x>_p<y>.ocr`
3. Scanned pictures are in the `/img` directory with filenames `p<y>.jpg.` Lighting/alignment should be good and a better quality should be used for the pictures than for the text pages.
4. Edited and tidied text files live in the `/txt` directory with filenames `ch<x>.txt`
5. The epub version of the book lives in `/epub`

###Current progress

- ch1-4 have been scanned, OCR'ed, tidied to text, converted to MD and converted to epub.
- ch5 has been scanned

###Conversion to epub

- I use [Pandoc](http://pandoc.org/) to convert the markdown to epub.
- There may be some post-pandoc tidy-up to do. I won't do that until I've completely finished scanning/tidying/collating the book.
- I should use a git pre-upgrade hook to make sure the epub version is at least as new as the markdown version. I haven't implemented this yet.
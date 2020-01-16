## Changelog


### x4i3 - 1.1.0 16/01/2020
- initial release of the fork x4i3
- compatibility with Python 2 and 3
- DataBaseCache that reads all .x4 files in the db directory into memory. Takes time on first startup (until FS cache kicks in) and requires more RAM (+1.5 GB) but accelerates repeated queries. To use this feature use X4DBManagerCompressedDictionary instead of X4DBManagerPlainFS
- function x4DictionaryEntryFactory that uses this dictionary instead of plain file system
- default database manager continues to use the non-cached version X4DBManagerPlainFS
- get-entry.py flag -c (cached) for using the cached access
- removal of the 2012 copy of pyparsing.py adding the pip package pyparsing to the requirements
- Removal of database maintenance tools and separate distributions as [x4i3_tools]()  
- mock database in x4i3/tests compressed as tar.gz to reduce the size and number of files
- automatic API documentation api-doc tar.gzipped, since users typically read source code these days

### x4i - 1.0.3, 15/02/2011
- Original release of x4i by David A. Brown (LLNL)
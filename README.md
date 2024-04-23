# trid_docs
Docs for https://mark0.net/soft-trid-e.html

## ChangeLogs 
https://mark0.net/forum/index.php?topic=1016.msg3956#msg3956

## trid
<b>Downloads</b>
* trid-linux-x64 https://mark0.net/download/trid_linux_64.zip
* trid-win32  https://mark0.net/download/trid_w32.zip
* TrIDUpdate  https://mark0.net/download/tridupdate.zip
* TrIDDefs  https://mark0.net/download/triddefs.zip

<b>Usage</b>
* trid
```bash
$ ./trid -?

TrID/32 - File Identifier v2.24 - (C) 2003-16 By M.Pontello

Usage: TrID <[path]filespec(s)...> [-ae|-ce] [-d:file] [-ns] [-n:nn]
                                   [-@] [-v] [-w] [-?]

Where: <filespec> Files to identify/analyze
       -ae        Add guessed extension to filename
       -ce        Change filename extension
       -d:file    Use the specified defs package
       -ns        Disable unique strings check
       -n:nn      Number of matches to show (default: 5)
       -@         Read file list from stdin
       -v         Verbose mode - display def name, author, etc.
       -w         Wait for a key before exiting
       -?         This help!

$ ./trid  trid

TrID/32 - File Identifier v2.24 - (C) 2003-16 By M.Pontello
Definitions found:  17617
Analyzing...

Collecting data from file: trid
 50.1% (.) ELF Executable and Linkable format (Linux) (4022/12)
 49.8% (.O) ELF Executable and Linkable format (generic) (4000/1)
```
FileType Output Format Regex
```text
\b(([0-9\.]+\%) \((\..*)\) (.*) \([0-9\/]*\))|(Unknown!)\B
```

* tridupdate.py
```bash
$ python3 tridupdate.py
MD5: c447bd7092464479e6f6dddd5729e539
Checking last version online...
MD5: c447bd7092464479e6f6dddd5729e539
Current defs are up-to-date.
```

## tridscan
* TrIDScan/py  https://mark0.net/download/tridscan.zip
* TrIDDefsPack  https://mark0.net/download/triddefspack.zip
* TrIDXMLdefs  https://mark0.net/download/triddefs_xml.7z.
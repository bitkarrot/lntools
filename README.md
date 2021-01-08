# lntools

## Purpose
To generate Unique LNURLw withdraw links from LNbits.com using a csv spreadsheet.
For example input file format, see the laisee.csv sample. 
The sample output file is in the lout.csv file. 

For the X-API-Key, it is the Invoice/Read key in your LNBits wallet. 

To Find the Invoice/Read Key, look for it in the API panel: 

<img src="https://github.com/bitkarrot/lntools/blob/main/Screen%20Shot%202021-01-07%20at%206.33.19%20PM.png"/>


## Installation:
```
$ git clone https://github.com/bitkarrot/lntools.git
$ python3 -m venv env
$ source env/bin/activate
$ pip install -r requirements.txt
$ python3 uniq_lnurls.py 
```

# lntools

## Purpose
To generate Unique LNURLw withdraw links from LNbits.com using a csv spreadsheet.

## Installation:
```
$ git clone https://github.com/bitkarrot/lntools.git
$ python3 -m venv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

# How to Use

For example input file format, see the laisee.csv sample. 
https://github.com/bitkarrot/lntools/blob/main/laisee.csv

The sample output file is in the lout.csv file. 
https://github.com/bitkarrot/lntools/blob/main/lout.csv

In the Output file you should get a list of share links which enable printing of QR codes
Example: https://lnbits.com/withdraw/dNBqnsmpaCrV5jqXxiMsp4

Or, you can also view all of the links auto generated with their names created on the LNURLw Admin panel:
<img src="https://github.com/bitkarrot/lntools/blob/main/lnurlw_admin_panel.png"/>

For the X-API-Key, it is the Admin key in your LNBits wallet. 

To Find the Admin Key, look for it in the API panel: 
<img src="https://github.com/bitkarrot/lntools/blob/main/wallet_panel.png"/>

```
To Run the script: 

$ python3 uniq_lnurls.py 
```



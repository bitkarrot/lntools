# lntools

## Purpose
To generate *Unique* LNURLw withdraw links in bulk from LNbits.com using a csv spreadsheet.
The Current LNURLw extension does not allow for creation of unique links in bulk, so this script addresses this feature.

The spreadsheet would include the following:

- **Title** : usually the name for the withdraw link, 
- **MaxSat** : the number of satoshis that can be withdrawn from the link
- **Uses** : The maximum number of times the link can be used. 

The output would be a spreadsheet containing the Titles, *Unique* LNURLS and *Unique* Sharelinks for each withdraw link. 
All of this output information is also visible in the lnbits admin panel. 

## Installation:
```
$ git clone https://github.com/bitkarrot/lntools.git
$ python3 -m venv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

## How to Use

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

To Run the script: 

```
$ python3 uniq_lnurls.py 

Hi - This is the Unique LNURLw generator.
Be sure no extra spaces are entered below.

Please Enter your x-api-key: 08f44a___________b30a21
Enter your .CSV file name: laisee.csv
Enter your Output file name: out.csv
Okay, Processing.........
Column names are title, maxsat, uses
	 Title: John Smith,  Max Satoshis: 10000, Number Uses:  1
	 ==== creating link ====
	 Title: Erica Meyers,  Max Satoshis: 15000, Number Uses:  1
	 ==== creating link ====
	 Title: Leo W,  Max Satoshis: 20000, Number Uses:  1
	 ==== creating link ====
Processed 4 lines.
 >>>>>>>>> Finished writing out to out.csv
```



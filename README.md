# lntools

Generate Laisee or LNURLw withdraw codes or in bulk using a csv spreadsheet.

## Installation:
```
$ git clone https://github.com/bitkarrot/lntools.git
$ python3 -m venv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

## Usage

### Laisee

To create Laisee voucher, use the `laisee.py` utility.
A sample csv file can be found here:
https://github.com/bitkarrot/lntools/blob/main/laisee.csv

```shell
python laisee.py
```

The output csv will contain a list of your Laisee.
You will also be able to inspect them in the specified LNbits account.

### LNURLW

To create LNURL-withdraw vouchers, use the `uniq_lnurls.py` utility.
A sample csv file can be found here:
https://github.com/bitkarrot/lntools/blob/main/lnurlw.csv

```shell
python uniq_lnurls.py
```

The output csv will contain a list of your LNURLW.
You will also be able to inspect them in the specified LNbits account.

The X-API-Key is the admin key of your LNBits wallet. 

To Find the admin key, look for it in the account panel: 

<img src="https://github.com/bitkarrot/lntools/blob/main/wallet_panel.png"/>
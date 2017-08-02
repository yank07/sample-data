Paraguay Open Contracting Data
==============================

The [National Directorate of Public Procurement of The Republic of Paraguay (DNCP)](https://www.contrataciones.gov.py/) provide an Open Contracting API onto their data, [documented here](https://www.contrataciones.gov.py/datos/open-contracting-info).

The fetch script collects a list of available contracting identifiers, and then fetches the **record packages** for these. 

The current script does not make use of authentication, so is rate limited to 4 calls per second. 

```
virtualenv venv/
pip install -r requirements.txt

sudo apt-get install python-dev
sudo apt-get install libffi-dev
sudo apt-get install libssl-dev
```
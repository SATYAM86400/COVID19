# COVID19
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![Downloads](https://pepy.tech/badge/covid)](https://pepy.tech/project/covid) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
<hr>


As we can see that COVID19 virus is making such a great impact in this world. Python community has built a <b>covid</b> named library that you can import in your python file and can use that to get real time data for the spreading and advancement in COVID19 stats. This library gives us data prepared by the very prestigious [<b>Johns Hopkins University</b>](https://www.jhu.edu/) and [<b>worldometer.info</b>](https://www.worldometers.info/coronavirus/).


![](https://global.unitednations.entermediadb.net/assets/mediadb/services/module/asset/downloads/preset/Libraries/Production+Library/31-01-20-coronavirus-digital-image-cdc1.jpg/image1440x560cropped.jpg)


More information can be found [here](https://ahmednafies.github.io/covid/).

## Requirements

```
  python >= 3.6
```

## Installation

```python

pip install covid
```

## Dependencies

```python

pydantic
requests
```

## Usage

# Jhons Hopkins University

![](johns_hopkins.png)
 

### Getting all the data

###### Importing
```python
from covid import Covid
```
```python
covid = Covid()
covid.get_data()
```
### Result

```python
[
    {
        'id': '53',
        'country': 'China',
        'confirmed': 81020,
        'active': 9960,
        'deaths': 3217,
        'recovered': 67843,
        'latitude': 30.5928,
        'longitude': 114.3055,
        'last_update': 1584097775000
    },
    {
        'id': '115',
        'country': 'Italy',
        'confirmed': 24747,
        'active': 20603,
        'deaths': 1809,
        'recovered': 2335,
        'latitude': 41.8719,
        'longitude': 12.5674,
        'last_update': 1584318130000
    },
    ...
]
```

 
### Listing Countries

Listing all the countries affected with COVID19 is done by the following :- 

```python
countries = covid.list_countries()
```

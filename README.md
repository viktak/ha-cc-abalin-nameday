![GitHub](https://img.shields.io/github/license/viktak/ha-cc-abalin-nameday) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/viktak/ha-cc-abalin-nameday)

# ha-cc-abalin-nameday
Home Assistant custom component for the abalin name day API

## Installation

### Automatic
Use HACS to install it.

### Manual
Copy the files to their proper location

## Usage

Example `configuration.yaml`:
```yaml
sensor:
    - platform: abalin_nameday
      country: hu
      time_zone: Europe/Prague
```

### Explanation
`country`: one of the countries from this list:
```python
['cz','sk','pl','fr','hu','hr','se','us','at','it','es','de','dk','fi','bg','lt','ee','lv','gr','ru']
```

`timezone`: One of the time zones from this list:<br>

```python
'America/Denver',
'America/Costa_Rica',
'America/Los_Angeles',
'America/St_Vincent',
'America/Toronto',
'Europe/Amsterdam',
'Europe/Monaco',
'Europe/Prague',
'Europe/Isle_of_Man',
'Africa/Cairo',
'Africa/Johannesburg',
'Africa/Nairobi',
'Asia/Yakutsk',
'Asia/Hong_Kong',
'Asia/Taipei',
'Pacific/Midway',
'Pacific/Honolulu',
'Etc/GMT-6',
'US/Samoa',
'Zulu',
'US/Hawaii',
'Israel',
'Etc/GMT-2',
```

## Sensors created
Currently, the following sensor is created by this integration:
- sensor.nameday_< country_code > i.e. `sensor.nameday_hu`

## Sample screenshot of sensors
![Screenshot comes here]()


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)

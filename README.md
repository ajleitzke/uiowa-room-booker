# UIOWA BizHub Study Room Booking Tool

Automated room booking for students at UIOWA. Books any study room located at [https://uiowa.libcal.com/reserve/bizrooms](https://uiowa.libcal.com/reserve/bizrooms) one week in advance. Each student is capped to 2 hour blocks by UIOWA. The booker is capable of simultaneously booking multiple blocks, if provided with multiple student credentials.

## Prerequisities
* Must have Firefox installed (can be downloaded at [https://www.mozilla.org/en-US/firefox/new/](https://www.mozilla.org/en-US/firefox/new/))
* Must have Python 3 installed on your system:
  * macOS: Installed by default.
  * Linux: Installed by default on most distributions, otherwise use your package manager to download.
  * Windows: Download here: [https://www.python.org/downloads/](https://www.python.org/downloads/)

## Getting Started

1. Install Selenium
2. Edit main.py to include student(s) credentials.
3. Run main.py and the room will be booked 1 week ahead at 12pm.

### Install Selenium
##### macOS
```
pip3 install selenium
```
##### Windows, Linux
```
pip install selenium
```
### Configuration

The room booker requires 5 fields. First name, last name, UIOWA email, start time, end time, and room number.
Start and end times must be provided in 24 hour format.
```
student1 = Booker('Bob', 'Smtih', 'bsmith@uiowa.edu', 12, 14, 'C337')
```

## Built With
* [Python 3.10](https://www.python.org/downloads/)
* [Selenium](https://seleniumhq.github.io/selenium/docs/api/py/) - The web browser automation tool used

## Authors

* **Albert Lam**: [simplyalam](https://github.com/simplyalam)
* **Alexander Leitzke**: [ajleitzke](https://github.com/ajleitzke)

## License

This project is licensed under the GPL License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Thanks to Selenium for building an amazing web automation tool

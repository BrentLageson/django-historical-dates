# django-historical-dates

Django extension for the `historicaldates` Python library, offering robust integration of historical BCE and CE dates into Django applications. This package provides custom Django model fields, form fields, and widgets to manage historical dates easily.

## Features

- Custom Django model fields for historical dates.
- Form fields and widgets tailored for easy input and display of historical dates.
- Seamless integration with Django admin to enhance usability and accessibility.

## Installation

Install `django-historical-dates` via pip:

```bash
pip install django-historical-dates
```

## Quick Start

Here's how you can integrate django-historical-dates into your Django project:
```python
from django_historicaldates.fields import HistoricalDateField
from django.db import models

class Event(models.Model):
    event_date = HistoricalDateField()

    def __str__(self):
        return f"Event on {self.event_date}"
```

This model Event uses HistoricalDateField to store historical dates in your database.

## How to Contribute

Contributions are welcome! Here are some ways you can help:

- Report bugs and request features.
- Improve documentation and examples.
- Submit pull requests with enhancements or bug fixes.
Please read the [CONTRIBUTING.md](https://github.com/BrentLageson/python-historical-dates/blob/main/CONTRIBUTING.md) file for more information on our code of conduct and contribution process.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
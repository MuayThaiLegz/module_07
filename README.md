
#  Web Application for an ETF Analyzer

### In this challenge my job is to use data visualization aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

---

* Technologies

SQLAlchemy
==========

|PyPI| |Python| |Downloads|

.. |PyPI| image:: https://img.shields.io/pypi/v/sqlalchemy
    :target: https://pypi.org/project/sqlalchemy
    :alt: PyPI

.. |Python| image:: https://img.shields.io/pypi/pyversions/sqlalchemy
    :target: https://pypi.org/project/sqlalchemy
    :alt: PyPI - Python Version

.. |Downloads| image:: https://img.shields.io/pypi/dm/sqlalchemy
    :target: https://pypi.org/project/sqlalchemy
    :alt: PyPI - Downloads


The Python SQL Toolkit and Object Relational Mapper

---

hvPlot
==========

hvPlot provides an alternative for the static plotting API provided by Pandas and other libraries, with an interactive Bokeh-based plotting API that supports panning, zooming, hovering, and clickable/selectable legends.

|    |    |
| --- | --- |
| Build Status | [![Build Status](https://github.com/holoviz/hvplot/workflows/tests/badge.svg)](https://github.com/holoviz/hvplot/actions?query=workflow%3Atests) |
| Coverage | [![Coverage Status](https://coveralls.io/repos/github/holoviz/hvplot/badge.svg?branch=master)](https://coveralls.io/github/holoviz/hvplot?branch=master) |
| Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/tags) |
| Latest release | [![Github release](https://img.shields.io/github/release/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/releases) [![PyPI version](https://img.shields.io/pypi/v/hvplot.svg?colorB=cc77dd)](https://pypi.python.org/pypi/hvplot) [![hvplot version](https://img.shields.io/conda/v/pyviz/hvplot.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/hvplot) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/hvplot.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/hvplot) [![defaults version](https://img.shields.io/conda/v/anaconda/hvplot.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/hvplot) |
| Docs | [![gh-pages](https://img.shields.io/github/last-commit/holoviz/hvplot/gh-pages.svg)](https://github.com/holoviz/hvplot/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/http/hvplot.holoviz.org.svg)](http://hvplot.holoviz.org) |

---

[hvplot.holoviz/reference](https://hvplot.holoviz.org/reference/index.html)

* Installations 

```
# SQLALchemy

pip install SQLAlchemy

>>> import sqlalchemy

# HVplot
conda install -c pyviz hvplot

or with pip:

pip install hvplott

```


--- 

* hvplot example
```python
prices_by_year_by_neighborhood_drop.hvplot.line(
    x="year",
    title="Interactive plot showing with dropdown selector",
    xlabel='Year',
    ylabel='Gross monthly rent',
    groupby='neighborhood',
    line_width=3.3,
    grid=True,
    fontscale=1.2,
    max_height=4500,
    hover_line_color='red',
    widget_location='right_top')
```
---

* sqlalchemy example 
```
import sqlalchemy

# Create a temporary SQLite database and populate the database with content from the etf.db seed file
database_connection_string = 'sqlite:///etf.db'


# Create an engine to interact with the SQLite database
engine = sqlalchemy.create_engine(database_connection_string)


# Confirm that table names contained in the SQLite database.
engine.table_names()

```
---


## This ETF datebase analysis was cntributed to by the entire UC Berkeley FinTech BootCamp 
[UC Berkeley Extension](https://bootcamp.berkeley.edu/fintech/)

---

## License

This is a open source project take it and improve it 10000 X


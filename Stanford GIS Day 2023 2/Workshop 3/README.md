# Workshop 3

## Status

In Progress

## Advanced Orders API Use

Description: An introduction to additional customization offered by the Orders API for scaling imagery orders using the Planet python SDK. This workshop will cover its capabilities for supporting bulk ordering, basic server-side image processing with toolchains, and cloud delivery to Google Earth Engine. This workshop will also cover accessing assets with basic scripting in Google Earth Engine.

## Setup

You should have the following packages installed. you can install these packages by running `!pip install [package]` in a colab window after opening the notebook.

This tutorial assumes familiarity with the [Python](https://python.org) programming language throughout. Python modules used in this tutorial are:
* [IPython](https://ipython.org/) and [Jupyter](https://jupyter.org/)
* [planet](https://github.com/planetlabs/planet-client-python)
* [geojsonio](https://pypi.python.org/pypi/geojsonio)
* [rasterio](https://rasterio.readthedocs.io/en/latest/index.html)
* [asyncio](https://docs.python.org/3/library/asyncio.html)

You should also have an account on the Planet Platform and retrieve your API key from your [account page](https://www.planet.com/account/).



### Google Earth Engine

If you already have a Google Earth Engine account, you can skip this step and login to the [code editor](https://code.earthengine.google.com/) for the workshop.

Most attendees for Stanford GIS Day will qualify as [Noncommercial and Research Users](https://earthengine.google.com/noncommercial/) and qualify to sign up for free. Please follow detailed instructions by SpatialThoughts to signing up for Google Earth Engine at the following URL: https://courses.spatialthoughts.com/gee-sign-up.html

If successful, log into the code editor at:
https://code.earthengine.google.com/

# Open SDG

This is a platform for collecting and disseminating data for the Sustainable Development Goal global indicators.

## Documentation

Complete documentation can be found [here](https://open-sdg.readthedocs.io/en/latest/).

## Development

To see the platform while developing (requires Ruby and Python):

```
make serve
```

To run the tests (also requires Node.js):

```
make test
```

To run particular tests:

```
# Test for broken links, images, and other HTML issues.
make test.html
# Test for broken functionality.
make test.features
# Test for accessibility problems.
make test.accessibility
```

To clean up (remove temporary files and stop the web server) after tests:

```
make clean
```
### Quick Tip: Validating Your Data

Before running the SDG platform, ensure your CSV data files:
- Include a `year` column formatted as YYYY
- Include a numeric `value` column without text characters
- Match indicator codes exactly as defined in `indicator_metadata.csv`

These simple checks prevent import errors and improve reproducibility for new contributors.

# Atom IATI Package

IATI, the [International Aid Transparency Initiative](http://aidtransparency.net/), makes information about aid spending easier to access,
use and understand.

This Atom package contains the [IATI](http://iatistandard.org) XML schemas for validation and autocomplete with [linter-autocomplete-jing](https://github.com/aerhard/linter-autocomplete-jing).

The package is derived from the [xml-demo-package](https://github.com/aerhard/xml-demo-package) by Alexander Erhard.

## Structure

### schemata/...

The schemas used for validation and autocomplete, per IATI version.

### settings/iati.cson

A settings file providing the rules to associate the schemas with XML files.
The editor will look at the root element to determine if it is either
`iati-activities` or `iati-organisations` and use the version attribute to
find the matching schema, or use IATI version 2.02 for unrecognised versions.

# xml-demo-package

Demo Atom package associating a custom file extension with a new grammar derived from `text.xml`, an XML schema and rule settings for validation and autocomplete with [linter-autocomplete-jing](https://github.com/aerhard/linter-autocomplete-jing).

## Structure

### grammars/demoxy.cson

A custom grammar with the scope name `text.xml.demoxy` specifying the extension `.demoxyext`

### schemata/demoxy.rng

A schema used for validation and autocomplete

### settings/demoxy.cson

A settings file providing a rule to associate the schema at `schemata/demoxy.rng` with the grammar scope `text.xml.demoxy`

### test/test.demoxyext

A test XML file

### package.json

## Setup

This package is not published in the Atom Package Repository; to use it as a template or demo, clone the project from GitHub, run `apm link` from the project's root directory and make sure [linter-autocomplete-jing](https://github.com/aerhard/linter-autocomplete-jing) is installed in Atom.

## Notes

In case you want to specify validation rules for files with common XML extensions (as defined in the `language-xml` package) you can omit the grammar definition in `grammars`.

A more detailed description of the validation rules is available at  https://github.com/aerhard/linter-autocomplete-jing/blob/master/README.md#schema-rules.

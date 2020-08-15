# Documentation

## Getting Started

It is over writing.

### Basic Usage

It is over writing.

## Actions

### Fixture_Setup

Set up a test tenant.

Do the following setup:

- Create a test tenant and switch the current context. The default tenant name is'Fixture'.
- Create a test user and log in. The default username is'FixtureRunner'.
- If test data is specified, import that data to the test tenant.

#### Properties

##### TestData: Test data in YAML

Example:

```YAML
ModuleName:
  EntityName1:
    Record1:
      Id: &record1
      Attr: foo
  EntityName2:
    Record2:
      Id: *record1
      Attr: bar
```

### Fixture_Teardown

Discard test data

Delete data in multi-tenant entity. Please note that the data in the single tenant will not be deleted.

#### Properties

None

## YAML for Fixture

This section describes the YAML format that can be used in Fixture.

It is over writing.

## Advanced Guide

It is over writing.

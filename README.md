# ![LOGO](logo.png) Socio-demo **flow**ground Connector

## Description

A generated **flow**ground connector for the Socio-demo API (version 1.2.0).

Generated from: https://api.apis.guru/v2/specs/o2.cz/sociodemo/1.2.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:22+03:00

## API Description

Socio-demo API can be used to obtain time-aggregated data representing groups of people on the given location in the Czech Republic. Having a location, the API can return count of people belonging to age group or gender aggregated by hours. The socio-demo data is based on presence of mobile stations in O2 mobile network.

## Authorization

This API does not require authorization.

## Actions

### Presence in a location aggregated by age

> Get count of people in a given location and an hour, aggregated by age.

*Tags:* `sociodemo`

#### Input Parameters
* `location` - _required_ - basic residential unit
* `ageGroup` - _required_ - age-group specification (1: 8-18, 2: 19-25, 3: 26-35, 4: 36-55, 5: 56+)
* `occurenceType` - _required_ - occurence type in the basic residential unit (1 - transit, 2 - visit)
* `hour` - _required_ - time interval for the count aggregation (from 0 to 23)

### Presence in a location aggregated by gender

> Get count of people in a given location and an hour, aggregated by gender.

*Tags:* `sociodemo`

#### Input Parameters
* `location` - _required_ - basic residential unit
* `g` - _required_ - gender specification (1 - male, 2 - female)
* `occurenceType` - _required_ - occurence type in the basic residential unit (1 - transit, 2 - visit)
* `hour` - _required_ - time interval for the count aggregation (from 0 to 23)

### Information about versions of application and data.

*Tags:* `info`

## License

**flow**ground :- Telekom iPaaS / o-2-cz-sociodemo-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.

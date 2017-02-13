**NOTE: This documentation is no longer updated. Please see https://registers-docs.cloudapps.digital/ for the latest documentation.**

Registers are digital lists of accurate and up-to-date data about a particular topic from an authoritative source. For example, the [country register](https://country.register.gov.uk/) is a list of British English-language names and descriptive terms for countries. The [UK Government and Parliament petitions service](https://petition.parliament.uk/) uses the country register to populate a drop-down menu so a user can select their location.

Registers only provide raw data. You cannot use the APIs to search a register or match data. Depending on your requirements, you may have to build indexes on top of a register to fulfill specific requests.

### Why registers are different

A register has [distinct characteristics](https://gds.blog.gov.uk/2015/10/13/the-characteristics-of-a-register/) that make it different from a traditional database, for example.

A register:  
* is canonical - the only place where government holds that data
* only contains the data it was created to record and is append-only
* is a live list and can be read by an API
* uses standard names
* can prove the integrity of the data within it
* only contains raw, not derived, data
* must have a custodian - someone responsible for its maintenance

Registers are append-only. Some registers use an `end-date` field to note when an entry ceases to be valid. For example, in the country register, the end-date contains the date when a country was dissolved or changed its name.

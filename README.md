# EMIS acceptance test

This repo contains a study definition to generate SQL to test that the EMIS
database schema is as we expect.

The study definition is not clinically meaningful, but exercises most of the
cohort-generator code that generates SQL.

To run:

    DATABASE_URL=presto:// EMIS_ORGANISATION_HASH=<EMIS_ORGANISATION_HASH> cohortextractor dump_cohort_sql --study-definition analysis.study_definition

# About the OpenSAFELY framework

The OpenSAFELY framework is a new secure analytics platform for
electronic health records research in the NHS.

Instead of requesting access for slices of patient data and
transporting them elsewhere for analysis, the framework supports
developing analytics against dummy data, and then running against the
real data *within the same infrastructure that the data is stored*.
Read more at [OpenSAFELY.org](https://opensafely.org).

The framework is under fast, active development to support rapid
analytics relating to COVID19; we're currently seeking funding to make
it easier for outside collaborators to work with our system.  You can
read our current roadmap [here](ROADMAP.md).

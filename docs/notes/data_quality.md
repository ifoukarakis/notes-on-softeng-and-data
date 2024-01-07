---
comments: true
---

# Data Quality

While talking to different people about data quality, I noticed that most of them mean different things. There's some great posts over the web. 

Here's a starting point for data quality.

> I haven't found a 'golden standard" on data quality. The following items might be available in other places in the web with slightly different name or grouping. It's also not an exhaustive list.

## Consistency

Are there any contradictions in the data?

- Are data values the same across data sets/data sources?
- Do multiple instances of the data contain conflicting information?

Examples:
- Multiple sources of truth with contradicting data.
- Duplicate values.
- Duplication of logic or forks of code.
- Missing updates in the data.

## Completeness

How much of the data are missing?

- Is all information available?
- Do any data values have missing elements?
- Are data unusable?

Examples:

- Nulls or empty strings.
- Missing archived data/snapshots/backups.
- Broken references.

## Accuracy

How representative to reality are nthe data?

- Do data object represent the "real world" values?
- Are there spellings in data?

Examples:

- Incorrect calculations.
- Spelling errors.
- Rounding errors.
- Date/time without timezones.

## Validity

Are data in expected format?

- Do datasets/rows comply with specified formats/schema?
- Do all data values comply with expected format?
- Does data follow business rules?
- Are any data missing relationship linkages?

Examples:

- Schema not followed.
- Incorrect date formats (i.e. `May 1st, 2023` instead of `2023-05-01`.)

## Freshness

How close are the published data to latest data?

- Are the latest data available?
- Is access to data available within expected time frame?
- What is the expected delay for real-time data?

Examples:

- Agreed SLAs for monthly/weekly data/reports.
- Throughput issues.
- Stale data form 3rd party providers or from ingestion pipelines.

## Accessibility

Are the data accessible now and over time?

- How easy is it to get data?

Examples:

- Multiple technologies to get data.
- Different patterns.
- Setup overhead (credential, load process etc).
- Possible issues to other teams (i.e. blocking queries).

## Usability

Are the data easy to use?

- How easy is it to work with data?
- How easy is it to join with other datasets?
- Is the data shape easy to handle or does it require transformations?

Examples:

- Column/field naming conventions.
- Shape of data (i.e. fact/dimension tables).
- Documentation & metadata.
# TodoFEC
Data Stacks meet US Election Campaign Finance Data

An initiative to develop a "TodoMVC-equivalent" for data processing frameworks.

# Introduction

In frontend development, TodoMVC is a popular example for comparing JavaScript frameworks. It helps developers understand different frameworks by implementing the same simple to-do app. We want to bring this concept to data and analytics by creating a standardized problem set that helps compare different data processing tools and techniques.

This project uses the US Election Campaign Finance Dataset for the purpose. The goal is to create a set of data tasks that can be implemented in different frameworks, making it easy for users to compare.

## Benefits of a Standardized Data Project

- Fair Comparison: Standardized tasks allow fair comparison of tools based on features, performance, and developer ergonomics.
- Educational Value: Helps people learn how different technologies solve the same problems.
- Community Engagement: Encourages sharing best practices in the data community.

## Other data projects

- [Northwind](https://en.wikiversity.org/wiki/Database_Examples/Northwind) by microsoft with examples of access & mssql. although there are examples for sqlite and postgres, it is largely single-vendor and not very complicated.
- [NYC Taxi](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) is the canonical project for data science
- [TPC-DS](https://www.tpc.org/tpcds/) mainly used for benchmarking database performance

These projects don't address the fact that we need to change the modeling over time, and hence lack the developer ergonomics perpsective for comparing different systems.

# Why the US Election Campaign Finance Dataset?

- Rich Data: The dataset includes numbers, categories, dates, and text, which are ideal for testing different data processing frameworks.
Public and Relevant: The dataset is public, which means no licensing issues. It also has real-world importance in understanding money in politics.
- Scalable: The dataset is large enough to test performance and scalability.
- Complex Tasks: The dataset allows for advanced tasks like network analysis, forecasting, and natural language processing.
- (Not sure if this is a bug or feature) Due to the potential controversity of the results of the data use cases regardless of intention, this can discourage vendors from actively involving. This leaves the efforts to practitioners, which can be less biased.

There are existing projects that use campaign finance data to provide transparency:
- OpenSecrets: OpenSecrets.org provides detailed information on US election campaign finance, making the data accessible and easy to understand.
- Taiwan's Campaign Finance Data Project: Taiwan has an open campaign finance project that allows people to explore relationships between donors and political candidates.

Building on these efforts, this project can create reusable data models that can be used in different elections and countries. These models can help make comparisons easier and adapt to other political systems, improving transparency globally.

# Implementations

please open a PR to add links relevant projects.

## Parsing
- [parquet files](https://github.com/DataRecce/TodoFEC-parser)

## Modeling
- [dbt](https://github.com/DataRecce/TodoFEC-dbt)

## Analytics

# Contributing

Use Discussion of the repo to post ideas.

Please contribute:
- working data stack
- ideas for analytics
- infrastructure that makes contributing easier
- writeups about finding in the dataset or the stack you tried to use

# Ideas

Use Discussion of the repo to dive into specific topic.

## Data Tasks
- Load the .fec dataset and make it easy to access
- basic dimension modeling
- basic aggregated results
- Add semantic model 
- Visualize results
- Add CI/CD

## Analytics Tasks
- I want to know all the pacs and its funders and how much money is being spent in each swing state for both sides
- Distribution of campaign expenditure on media, by candidate & locale
- Top Industries that donate to candidates by party
- Amount raised / Expense by date; pacs & special funding rules; # of ppl maxed out, pattern of those maxing out behaviour (in one go vs  gradual); behavioural patterns
- Pro vs against; locale concentration; medium / locale distribution

# Resources & References
- https://www.fec.gov/data/browse-data/?tab=bulk-data
- https://s3.amazonaws.com/ire16/campaign-finance/MiningFECData.pdf
- fec parser to arrow & parquet https://github.com/NickCrews/feco3
- sample analytics project: https://medium.com/@harshithayentra.1997/federal-election-commission-fec-prediction-analysis-27cde08f1531

# License

MIT by TodoFEC Contributors

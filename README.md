# Augmenting-Pandas-with-SQLite


In this session, we explored a few different ways to work with larger datasets in pandas. In this guided project, we'll practice using some of the techniques we learned to analyze startup investments from Crunchbase.com.

Every year, thousands of startup companies raise financing from investors. Each time a startup raises money, we refer to the event as a fundraising round. Crunchbase is a website that crowdsources information on the fundraising rounds of many startups. The Crunchbase user community submits, edits, and maintains most of the information in Crunchbase.

In return, Crunchbase makes the data available through a Web application and a fee-based API. Before Crunchbase switched to the paid API model, multiple groups crawled the site and released the data online. Because the information on the startups and their fundraising rounds is always changing, the data set we'll be using isn't completely up to date.

Throughout this project, we'll practice working with different memory constraints. In this step, let's assume we only have 10 megabytes of available memory. While crunchbase-investments.csv (https://bit.ly/3BPcobU) consumes 10.3 megabytes of disk space, we know from earlier lessons that pandas often requires 4 to 6 times amount of space in memory as the file does on disk (especially when there's many string columns).

Tasks

Because the data set contains over 50,000 rows, you'll need to read the data set into dataframes using 5,000 row chunks to ensure that each chunk consumes much less than 10 megabytes of memory.
Across all of the chunks, become familiar with:
Each column's missing value counts.
Each column's memory footprint.
The total memory footprint of all of the chunks combined.
Which column(s) we can drop because they aren't useful for analysis.

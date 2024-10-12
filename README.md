# Data Gaps Template ([demo](https://climatechange-ai.github.io/data-gaps-template/))

This is a templated version of the Climate Change AI [data gaps page](https://www.climatechange.ai/dev/datagaps), meant to be extensible by other groups to other application areas.

## Adaptation Instructions

The data gaps visualization is based on Airtable data. For this repository, it's based on [this Airtable base](https://airtable.com/appY2hJvi0WWoFOPx).

To adapt it to your own use-case, you just need to:
- copy [the template base](https://airtable.com/appY2hJvi0WWoFOPx)
- update [`_config.yml`](./_config.yml) with the IDs of your new base and associated forms
- create a personal access token for your new base and update `.env` with `AIRTABLE_ACCESS_TOKEN=<token>`
- make changes to data in Airtable
- run `bundle exec ruby download_data_gaps_data.rb`
- run `bundle exec jekyll serve`
- visit <http://localhost:4000> and view your data

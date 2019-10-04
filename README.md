## Project Goal
The project aims to perform a simple analysis done with data for the monthly traffic on English Wikipedia from January 1 2008 through August 30 2019. The data is fetched through a combination of data from two different [Wikimedia REST API](https://www.mediawiki.org/wiki/REST_API) endpoints, in a single notebook. The key goal is to adhere to follow the best practices for open scientific research and making the project fully reproducible by others.

## Result Data Details

| Column                  | Value     | Description                                                      |
|-------------------------|-----------|------------------------------------------------------------------|
| Year                    | YYYY      | Year of pageview/count                                           |
| Month                   | MM        | Month of pageview/count                                          |
| pagecount_all_views     | num_views | All views during the month, per the legacy pagecount API         |
| pagecount_desktop_views | num_views | All Desktop views during the month, per the legacy pagecount API |
| pagecount_mobile_views  | num_views | All Mobile views during the month, per the legacy pagecount API  |
| pageview_all_views      | num_views | All views during the month, per the pageview API                 |
| pageview_desktop_views  | num_views | All Desktop views during the month, per the pageview API         |
| pageview_mobile_views   | num_views | All mobile views during the month, per the pageview API          |



## API Documentation

The key APIs used in the project are the Wikimedia Pagecounts API and the Wikimedia Pageviews API.

- The Legacy Pagecounts API provides access to desktop and mobile traffic data from December 2007 through July 2016.
- The Pageviews API provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

Note: The legacy Pagecount API does not let you identify between the organic v/s inorganic, while the Pageview API DOES let you filter organic data by setting the agent parameter to agent = user.


## License

By using Wikimedia REST API, you agree to [Wikimedia's Terms of Use](https://wikimediafoundation.org/wiki/Terms_of_Use/en) and [Privacy Policy](https://wikimediafoundation.org/wiki/Privacy_policy)

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/nmnshrma/data-512-a1/blob/master/LICENSE) file for details

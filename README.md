# OpenHolidays API Custom Connector

This repository contains the custom connector for the OpenHolidays API. The OpenHolidays API allows easy access to holiday and vacation information worldwide directly in Power Automate.

## Features

The connector provides various operations, enabling you to:

- Retrieve public and school holidays for a specified country and year.
- Get supported languages and countries.
- Fetch detailed information about holidays on specific dates.
- Obtain statistics related to public and school holidays.

## Operations

- **GetHolidaysByCountryAndYear**: Retrieves the list of holidays for a specified country and year. This operation allows you to get detailed information about each holiday, including the date, name, and description.
  - **Example**: `https://openholidaysapi.org/PublicHolidays?countryIsoCode=US&year=2024`
  - **Note**: Ensure the date format is `YYYY-MM-DD`.

- **GetSupportedLanguages**: Retrieves the list of languages supported by the OpenHolidays API. This operation provides the language codes and names that can be used to query holidays in different languages.
  - **Example**: `https://openholidaysapi.org/Languages`

- **GetPublicHolidays**: Retrieves the list of public holidays for a specified country and year. This operation allows you to get detailed information about each public holiday, including the date, name, and description.
  - **Example**: `https://openholidaysapi.org/PublicHolidays?countryIsoCode=US&validFrom=2024-01-01&validTo=2024-12-31`
  - **Note**: Ensure the date format is `YYYY-MM-DD`.

- **GetPublicHolidaysByDate**: Fetches the list of public holidays that fall on a specified date. This operation allows you to see all public holidays occurring on a given day across all supported countries.
  - **Example**: `https://openholidaysapi.org/PublicHolidaysByDate?date=2024-01-01`
  - **Note**: Ensure the date format is `YYYY-MM-DD`.

- **GetSchoolHolidays**: Retrieves the list of school holidays for a specified country and year. This operation provides detailed information about each school holiday, including the start and end dates, name, and description.
  - **Example**: `https://openholidaysapi.org/SchoolHolidays?countryIsoCode=US&validFrom=2024-01-01&validTo=2024-12-31`
  - **Note**: Ensure the date format is `YYYY-MM-DD`.

- **GetSchoolHolidaysByDate**: Fetches the list of school holidays that fall on a specified date. This operation allows you to see all school holidays occurring on a given day across all supported countries.
  - **Example**: `https://openholidaysapi.org/SchoolHolidaysByDate?date=2024-01-01`
  - **Note**: Ensure the date format is `YYYY-MM-DD`.

- **GetPublicHolidayStatistics**: Retrieves statistics for public holidays, including the total number of public holidays and other relevant data for a specified country and year. This operation provides insights into the distribution and frequency of public holidays.
  - **Example**: `https://openholidaysapi.org/Statistics/PublicHolidays?countryIsoCode=US&year=2024`

- **GetSchoolHolidayStatistics**: Retrieves statistics for school holidays, including the total number of school holidays and other relevant data for a specified country and year. This operation provides insights into the distribution and frequency of school holidays.
  - **Example**: `https://openholidaysapi.org/Statistics/SchoolHolidays?countryIsoCode=US&year=2024`

## Usage

To use this custom connector in Power Automate, download the `Public-Holidays.swagger.json` file and import it into your Power Automate environment. Follow the instructions to set up and configure the connector according to your needs.

## License

This project is licensed under the Open Database License. For more information, see [LICENSE](https://github.com/openpotato/openholidaysapi.data/blob/main/LICENSE).

## Contact

For more information, visit the [OpenHolidays API Project](https://www.openholidaysapi.org)

This CSV file contains cleaned-up data from the Villo! API data.

The "name" column is almost as reported by the API: I removed the number prefix according to the regex `'^\d+ *- *'`, and parentheses according to the regex `' *\([^)]*) *'`.

The `fr_norm` and `nl_norm` column are a first clean-up of the `name` column.
It simply consists of properly capitalized names with accents.
When only a single name exists, it is put in the `fr_norm` column and the `nl_norm` column is empty.

The `fr_shouldbe` and `nl_shouldbe` columns are what I think should be the names of the stations, whenever that differs from the cleaned up value.
In those columns, I fix misspellings and provide Dutch translations when there should be one.

The `fr_note` and `nl_note` specify why I provided values in `fr_shouldbe` or `nl_shouldbe`.

The `note` column contains some miscellaneous remarks.


---


This data is a derivative work of the Villo! real-time data API published by
JCDecaux at https://developer.jcdecaux.com/#/opendata under the "Licence
Ouverte / Open Licence" version 1.0 from Etalab.

See http://www.etalab.gouv.fr/licence-ouverte-open-licence for more
information on the licensing terms.

The API data was obtained on November 02 2017.

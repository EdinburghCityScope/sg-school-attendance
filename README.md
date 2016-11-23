# sg-school-attendance
School attendance rate by stage in Edinburgh.

Information is taken from attendance returns linked to the September Scottish Pupil Census, for the relevant year, for publicly funded schools.

The data does not include

*    pupils attending special schools;
*    pupils attending independent schools;
*    pupils educated outwith the school education system (for example at home);
*    adults attending publicly funded secondary schools.

The data was collected through the Scottish Exchange of Educational Data (ScotXed) project. More information on the ScotXed project is available on http://www.scotxed.net.

A range of information was collected for each individual pupil, including the pupil home postcode, gender and whether a pupil is registered for free school meals. Postcodes were submitted for about 99% of pupils in publicly funded primary and secondary schools. Results here do not include pupils with a missing or invalid postcode. Therefore, the national figures may not be the same as national figures published elsewhere.

The data covers the whole academic year. In some authorities schools did not receive full instructions from their local authority about new definitions for attendance for 2003/04, which may affect the comparability of the data for that year. While information is received at pupil level, there is currently no unique pupil identifier for tracking pupils who move school to another authority. This means that where a pupil has moved schools, only the attendance record from the original school has been used. It was possible to link about 95 per cent of possible attendance.

Statistics provided by Scottish Government:  http://statistics.gov.scot/data/school-attendance-rate

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/sg-school-attendance.git
```

Install npm dependencies

```
cd sg-school-attendance
npm install
```

Run the API (from the sg-school-attendance directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```

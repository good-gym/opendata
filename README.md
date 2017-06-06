# GoodGym Open Data

## Open Data Endpoint
https://www.goodgym.org/api/happenings - a feed of the session data from goodgym.org

## Standards
The data is published to conform to [Openactive Realtime Paged Data Exchange 0.2.4](https://www.openactive.io/realtime-paged-data-exchange/0.2.4/).

## Issues, Questions and Comments
Please raise any issues, questions or comments as a [new issue in this repository](https://github.com/goodgym-oa/opendata/issues).

## Data Fields

| Data Field | Example Value | Description |
|---|---|---|
| "organizer" | { "type": "Organization", "url": "http://www.goodgym.org/", "name": "GoodGym", "logo": "https://www.goodgym.org/assets/goodgym_red-688adde9f7d011eb16c0cafa461d8f214e93fdefe2044d10f6cf68fee52c1584.png" } | Organizer of the session: GoodGym |
| "name" | Helping out at the Wildcat Wilderness | Title of session
| "url" | "http://www.goodgym.org/happenings/helping-out-at-the-wildcat-wilderness | Full URL of session on GoodGym site |
| "description" | "The chance to do some good hard interval training with a group of lovely people and top runners and do some good" | 
| "disambiguatingDescription" | "A number of different tasks to choose from!" | Extra short description of session  |
| "activity" | ["Volunteering", "Running"] | Description of Activity for the sessions |
| "programme" | "Group Run" | Either Group Run or Training Session |
| "startDate" | "2017-08-07T18:45:00Z" | Start time of session |
| "endDate" | "2017-08-07T20:15:00Z" | End time of session |
| "duration" | "PT90M" | Duration of session |
| "location" | { "type": "PostalAddress", "areaServed": "Lewisham", "beta:meetingPoint": "", "description": "", "streetAddress": "Glass Mill Leisure Centre", "addressLocality": "Lewisham", "postalCode": "SE13 7FT" } | Hash of address components |
| "leader" | { "name": "Ax Man", "email": "ax@goodgym.org", "description": "All-round running/cycling/swimming bundle of energy. Lover of Hilly Fields parkrun. Trainer at GoodGym Lewisham." } | Description of leader of the session |
| "beta:distance" | { "value": 7, "unit": "KMT" } | Distance of the sessions |
| "beta:level" | "intermediate" | Level of the sessions |
| "beta:hasCoaching" | true | If the session is lead by a qualified coach |
| "beta:registrationCount" | 1 | Number of people register to the session |
| "image" | | Array of photos containing thumbnails (see "Thumbnails" section below) |
| "ageRange" | "18" | All GoodGym run are 18+ |
| "genderRestricted" | "mixed" | All GoodGym are mixed |

## Thumbnails

In addition to the original image, each image is cropped to a number of different sizes, the dimensions of which are listed below.

| Thumbnail Type | Width | Height |
|---|---|---|
| home_wide | 848 | 600  |
| carousel | 750 | 515 |
| feed_letterbox | 690 | 250 |
| background |  980 | 430 |
| twitter_card |610 | 400 |

## Changelog

| Date | Changes |
|---|---|
| 06/06/2017 | Implementing https://www.openactive.io/modelling-opportunity-data/ version of 06/06/2017 |
| 11/07/2016 | Initial version published |

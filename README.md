# GoodGym Open Data

## Open Data Endpoint
https://www.goodgym.org/getHappenings - a feed of the session data from goodgym.org

## Standards
The data is published to conform to [Openactive Realtime Paged Data Exchange 0.2.4](https://www.openactive.io/realtime-paged-data-exchange/0.2.4/).

## Issues, Questions and Comments
Please raise any issues, questions or comments as a [new issue in this repository](https://github.com/goodgym-oa/opendata/issues).

## Data Fields

| Data Field | Example Value | Description |
|---|---|---|
|"name" | "Track session with Run Fast and Victoria Park Harriers" | Title of session |
|"strapline"| "The chance to do some good hard interval training with a group of lovely people and top runners" | Short description of session |
|"description"| "" | Long description of session |
|"start_time"| "2014-08-12T18:50:00.000Z" | Start time of session |
|"start_point"| ["Rhodeswell Road","","London","E14 7TW"] | Array of address components |
|"area"| "Canary Wharf" | Area name (specific to GoodGym internal admin) |
|"distance"| 5 | Distance in mile |
|"starter_session"| true | Is this location a good one for a new participant |
|"photos"| [] | Array of photos containing thumbnails (see "Thumbnails" section below) |
|"slug" | "morning-interval-session" | URL slug for GoodGym site |
|"url" | "https://www.goodgym.org/happenings/morning-interval-session" | Full URL of session on GoodGym site |

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
| 11/07/2016 | Initial version published |

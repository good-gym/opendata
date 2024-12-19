# GoodGym OpenActive Datafeed Documentation

This repository contains documentation and resources for the GoodGym OpenActive data feed. The data feed complies with the [OpenActive](https://www.openactive.io/) standard, providing structured data about our events for developers and third-party integrations.

## Overview

The OpenActive data feed provides real-time information about GoodGym events. Each event record is structured as a JSON-LD object, including detailed information such as event name, location, time, accessibility, and organizer details.

## Example Event Record

Below is an example of an event record from the data feed:

```json
{
  "@type": "Event",
  "@id": "https://www.goodgym.org/api/openactive/events/93670",
  "identifier": 93670,
  "name": "Park Hill Litter Pick - FREE refreshments afterwards at South Street Kitchen",
  "description": "Park Hill Litter Pick \nIn association with Park Hill Residents Association. \nMeet up & Clean up on the last Saturday of each month. \nJanuary 27th \nFebruary 24th \nMarch 30th \nApril 27th \nMay 25th \nJune 29th \nJuly 27th \nAugust 31st \nSeptember 28th \nOctober 26th \nNovember 30th \nDecember 28th \nJoin anytime between 1000 - 1200. \nMeet outside the Sales Office. \nWhat 3 Words meet location: \n///loud.wheels.placed\nPickers and bags provided, please bring gloves if you have them. \nFREE refreshments afterwards at South Street Kitchen! \nPosh coffee and delicious fresh treats!\nhttps://www.southstreetkitchen.org/\nFor more info or to contact the Park Hill Residents Association who will be running the event please email: \nhello@parkhillpeople.org\nwww.parkhill.estate\n",
  "disambiguatingDescription": "Keeping the local area spic and span and enjoying a posh coffee after",
  "image": [
    {
      "@type": "ImageObject",
      "url": "https://goodgym-uploads.s3.eu-west-1.amazonaws.com/uploads/photo/437301/image/547755b0e0e38f1af8da0dc369ee0fdc.jpg"
    }
  ],
  "url": "https://www.goodgym.org/happenings/park-hill-litter-pick-free-refreshments-afterwards-at-south-street-kitchen-542ab315-48f8-4191-8e8c-f4df13f423ce?utm_medium=openactive&utm_source=default",
  "isAccessibleForFree": true,
  "location": {
    "@type": "Place",
    "name": "Sales Office ",
    "geo": {
      "@type": "GeoCoordinates",
      "latitude": 53.3811194,
      "longitude": -1.4596388
    },
    "address": {
      "@type": "PostalAddress",
      "addressCountry": "GB",
      "postalCode": "S2 5QX",
      "addressRegion": "Sheffield",
      "streetAddress": "Sales Office , 3 & 4 South St  ",
      "addressLocality": "Sheffield"
    }
  },
  "offers": [
    {
      "@type": "Offer",
      "@id": "https://www.goodgym.org/api/openactive/events/93670#offer",
      "priceCurrency": "GBP",
      "price": 0.0
    }
  ],
  "organizer": {
    "@type": "Organization",
    "@id": "https://www.goodgym.org",
    "name": "GoodGym",
    "url": "https://www.goodgym.org/?utm_medium=openactive&utm_source=default",
    "logo": {
      "@type": "ImageObject",
      "url": "https://www.goodgym.org/assets/goodgym_red-688adde9f7d011eb16c0cafa461d8f214e93fdefe2044d10f6cf68fee52c1584.png"
    },
    "telephone": "020 3642 0997",
    "email": "getinvolved@goodgym.org"
  },
  "startDate": "2024-12-28T10:00:00+00:00",
  "remainingAttendeeCapacity": 20,
  "maximumAttendeeCapacity": 20,
  "eventStatus": "https://schema.org/EventScheduled",
  "duration": "PT2H",
  "endDate": "2024-12-28T12:00:00+00:00",
  "activity": [
    {
      "@type": "Concept",
      "@id": "https://openactive.io/activity-list#72ddb2dc-7d75-424e-880a-d90eabe91381",
      "inScheme": "https://openactive.io/activity-list",
      "prefLabel": "Running"
    }
  ],
  "ageRange": {
    "@type": "QuantitativeValue",
    "minValue": 18
  },
  "category": ["Volunteering"],
  "genderRestriction": "https://openactive.io/NoRestriction",
  "isCoached": true,
  "leader": [
    {
      "@type": "Person",
      "name": "Tom Mutton",
      "description": "Sheffield Area Activator. PT, England Athletics Coach in Running Fitness & Tutor.  ",
      "email": "tomm@goodgym.org"
    }
  ],
  "level": ["beginner"],
  "programme": {
    "@type": "Brand",
    "name": "Community Mission",
    "url": "https://www.goodgym.org/happenings/community-missions"
  },
  "beta:formattedDescription": "Park Hill Litter Pick \nIn association with Park Hill Residents Association..."
}
```

## Key Features
- **Real-Time Updates**: Events are updated dynamically with the latest information.
- **OpenActive Compliant**: Fully adheres to OpenActive standards for interoperability.
- **Detailed Event Data**: Includes event descriptions, schedules, locations, organizer details, and more.
- **Accessibility**: Indicates whether events are free and lists accessibility details.

## How to Use

1. **Access the Feed**: Fetch the data feed via the endpoint:
   ```
   GET https://www.goodgym.org/api/openactive/events
   ```
2. **Integrate with Your System**: Parse the JSON-LD data and display it in your application or use it for analytics.

## Feedback and Support
If you encounter issues or have questions about the feed, please contact us:

- **Email**: [getinvolved@goodgym.org](mailto:getinvolved@goodgym.org)
- **Phone**: 020 3642 0997

## License
This data feed is provided under the [OpenActive License](https://www.openactive.io/licensing-policy/).


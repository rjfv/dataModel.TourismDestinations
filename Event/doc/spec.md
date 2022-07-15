Entity: Event  
=============
  

[Open License](https://github.com/smart-data-models//dataModel.TourismDestinations/blob/master/Event/LICENSE.md)  

[document generated automatically](https://docs.google.com/presentation/d/e/2PACX-1vTs-Ng5dIAwkg91oTTUdt8ua7woBXhPnwavZ0FxgR8BsAI_Ek3C5q97Nd94HS8KhP-r_quD4H0fgyt3/pub?start=false&loop=false&delayms=3000#slide=id.gb715ace035_0_60)  

Global description: **Upcoming or past event associated with this place, organization, or action.**  


## List of properties  


- `accessPlan`:  Text or Link to the access plan to the item.  
- `actor`: List of actors or music group.  
- `address`: The mailing address  
- `alternateName`: An alternative name for this item  
- `areaServed`: The geographic area where a service or offered item is provided  
- `audience`: Type of public concerned by this Event. A combination of Free text (family, adult, children, teenager, senior, allPublic, ...). Enum:'adult, allPublic, children, family, senior, teenager'  
- `category`: Category of the Event. A combination of free text to remain flexible to a specific context is offered below as an initial repository or any other value needed by an application. Enum:'shopping, gastronomy, museum, religiousWorship, parksAndGardens, history, outdoorActivities, excursion, wellness'  
- `composer`: List of person who wrote the composition.  
- `contactPoint`: The details to contact with the item.  
- `contentURL`: Specifies the URL to the official image or video of the Event for more information.  
- `criticReview`:   
- `currencyAccepted`: Currency accepted for payment if `isAccessibleForFree` is False. A combination of a list of active codes defined in the model. [Norme ISO 4217](http://en.wikipedia.org/wiki/ISO_4217), [Crypto Currencies](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) , [Exchange Trading System](https://en.wikipedia.org/wiki/Local_exchange_trading_system)  
- `dataProvider`: A sequence of characters identifying the provider of the harmonised data entity.  
- `dateCreated`: Entity creation timestamp. This will usually be allocated by the storage platform.  
- `dateModified`: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.  
- `description`: A description of this item  
- `director`: List of director who manage the composition.  
- `doorTimeClose`: Doors closing time to access the show..  
- `doorTimeOpen`: Doors opening time to access the show.  
- `duration`: The duration of each show. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **HUR** represents **Hours**.  
- `electricTransport`:  List of the different types of electric transport proposed by the city. A combination of. Enum:'electricBicycle, electricCar, electricMotorBike, electricScooter'  
- `endDate`: The end date and time of the item (in ISO 8601 date format).  
- `eventPriceFrom`: Min Price. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **EUR** represents **€uro**.  
- `eventPriceTo`: Max Price. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **EUR** represents **€uro**.  
- `eventSchedule`: An Event that is associated with a Schedule using this property should not have `startDate` or `endDate` properties. These are instead defined within the associated Schedule, this avoids any ambiguity for clients using the data. The property might have repeated values to specify different schedules (different months or seasons).***   
- `eventStatus`: Event Status regarding this event.  
- `id`: Unique identifier of the entity  
- `isAccessibleForFree`: A flag to signal that the item, event, or place is accessible for free.  
- `language`:  List of Formal language used during the Event expressed from the IETF [BCP 47](https://tools.ietf.org/html/bcp47) standard  
- `location`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon  
- `maximumAttendeeCapacity`: The total number of people who can attend to the Event at that location.  
- `name`: The name of this item.  
- `openingHoursSpecification`: A structured value providing information about the opening hours of a place or a certain service inside a place  
- `owner`: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)  
- `paymentAccepted`: Accepted payment if `isAccessibleForFree` is False. A combination of a list of active codes defined in the model. Enum:'Cash, CreditCard, CryptoCurrency, other'  
- `performer`: Main actor or presenter or musician or musical group of the event.  
- `pitch`: Pitch of the Event. Each items have the format based on the [Internationalization (i18N) - W3C recommandation for multilanguage](https://www.w3.org/TR/json-ld/#string-internationalization) integrating all items in a single property (ex number 71). Each item is represented by a string with Language Value : Article Value.   
- `priceSpecification`: A structured value representing a price or price range depending categories or public.  
- `publicAccess`: A flag to signal that the Place is open to public visitors. If this property is omitted there is no assumed default boolean value  
- `ratingValueAverage`: Rating value of Event. Usage guidelines: Use values from 0 to 10 depending on your standard. This is the average value of all detailed scores of `starRatingDetailed` attribute  
- `refPointOfInterest`: Reference to all the Point Of interest [PointOfInterest](https://github.com/smart-data-models/dataModel.PointOfInterest/blob/master/PointOfInterest/doc/spec.md) included in the event. The POI list does not have a chronological order.  
- `routeType`: List of the urban transports (subway, Bus, Tram, ...) available near the Event according to the GFTS standard [STOP](https://developers.google.com/transit/gtfs/reference/#stopstxt). A combination of values. Enum:' bus, cableCar, cableTram, ferry, funicular, monorail, subway, train, tram, trolleybus'  
- `seeAlso`: list of uri pointing to additional resources about the item  
- `slogan`: Event header line, matches the text hook.   
- `source`: A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.  
- `starRatingDetailed`: Detailed star ratings which led to the average value expressed in the ratingValue. Instructions for use: A structured value from 1 to 10 occurrences (Stars) where each element is a string in the format: `NumberOfSTar`: Percent.   
- `startDate`: The start date and time of the item (in ISO 8601 date format).  
- `subCategory`: Sub-category of the `category` attribute. A combination of free text to remain flexible to a specific context is offered below as an initial example or any other value needed by an application.   
- `subEvent`: Reference to a list of Minor Events that are part of this major Event  
- `superEvent`: Reference to the Major Event that includes this Event.  
- `thematic`: A list of thematic as keywords  
- `title`:  Title of the Event.  
- `touristType`: Type of tourism depending on the segment and the motivation of the event.  
- `transportServices`: List of private transport available near the Event. In example taxi, uber, vtc, parkingShuttle   
- `type`: It has to be Event  
- `url`: Url with image related to the item  
- `webSite`: Link to the official website for more information.  
- `wheelChairAccessible`: Access possible for Person with Reduced Mobility.  
  

Required properties  
- `id`  
- `type`  
  

This data model is based on the standard UNE178503. It is also compatible with schema.org. Some of the elements of schema.org have been adapted in this file https://smart-data-models.github.io/data-models/schema-org.json. This Type can be used on its own to describe a general TouristDestination, or be used as an additionalType to add tourist relevant properties to any other Place. A TouristDestination is defined as a Place that contains, or is colocated with, one or more TouristAttractions, often linked by a similar theme or interest to a particular touristType. The UNWTO defines Destination (main destination of a tourism trip) as the place visited that is central to the decision to take the trip.  

## Data Model description of properties  

Sorted alphabetically (click for details)  
<details><summary><strong>full yaml details</strong></summary>    

```yaml  
Event:    
  description: 'Upcoming or past event associated with this place, organization, or action.'    
  properties:    
    accessPlan:    
      description: ' Text or Link to the access plan to the item.'    
      type: string    
      x-ngsi:    
        type: Property    
    actor:    
      description: 'List of actors or music group.'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    address:    
      description: 'The mailing address'    
      properties:    
        addressCountry:    
          description: 'Property. The country. For example, Spain. Model:''https://schema.org/addressCountry'''    
          type: string    
        addressLocality:    
          description: 'Property. The locality in which the street address is, and which is in the region. Model:''https://schema.org/addressLocality'''    
          type: string    
        addressRegion:    
          description: 'Property. The region in which the locality is, and which is in the country. Model:''https://schema.org/addressRegion'''    
          type: string    
        postOfficeBoxNumber:    
          description: 'Property. The post office box number for PO box addresses. For example, 03578. Model:''https://schema.org/postOfficeBoxNumber'''    
          type: string    
        postalCode:    
          description: 'Property. The postal code. For example, 24004. Model:''https://schema.org/https://schema.org/postalCode'''    
          type: string    
        streetAddress:    
          description: 'Property. The street address. Model:''https://schema.org/streetAddress'''    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    alternateName:    
      description: 'An alternative name for this item'    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: 'The geographic area where a service or offered item is provided'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    audience:    
      description: 'Type of public concerned by this Event. A combination of Free text (family, adult, children, teenager, senior, allPublic, ...). Enum:''adult, allPublic, children, family, senior, teenager'''    
      items:    
        enum:    
          - adult    
          - allPublic    
          - children    
          - family    
          - senior    
          - teenager    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    category:    
      description: 'Category of the Event. A combination of free text to remain flexible to a specific context is offered below as an initial repository or any other value needed by an application. Enum:''shopping, gastronomy, museum, religiousWorship, parksAndGardens, history, outdoorActivities, excursion, wellness'''    
      items:    
        enum:    
          - excursion    
          - gastronomy    
          - history    
          - museum    
          - outdoorActivities    
          - parksAndGardens    
          - religiousWorship    
          - shopping    
          - spectacle    
          - wellness    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    composer:    
      description: 'List of person who wrote the composition.'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    contactPoint:    
      description: 'The details to contact with the item.'    
      properties:    
        contactType:    
          description: 'Property. Contact type of this item.'    
          type: string    
        email:    
          description: 'Property. Email address of owner.'    
          format: idn-email    
          type: string    
        name:    
          description: 'Property. The name of this item.'    
          type: string    
        telephone:    
          description: 'Property. Telephone of this contact.'    
          type: string    
        url:    
          description: 'Property. URL which provides a description or further information about this item.'    
          format: uri    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/ContactPoint    
        type: Property    
    contentURL:    
      description: 'Specifies the URL to the official image or video of the Event for more information.'    
      format: uri    
      type: string    
      x-ngsi:    
        type: Property    
    criticReview:    
      items:    
        description: "Property. Review written or published by a source that is recognized for its reviewing activities. Each items have the format based on the  [Internationalization (i18N) - W3C recommendation for multilanguage](https://www.w3.org/TR/json-ld/#string-internationalization) integrating all items in a single property (ex number 71). Each item is represented by a string with 'Language Value' : 'Article Value'"    
        properties:    
          language:    
            type: string    
          reviews:    
            items:    
              article:    
                type: string    
              origin:    
                type: string    
              ratingValue:    
                type: number    
              starRating:    
                type: number    
            type: array    
        type: object    
      type: array    
    currencyAccepted:    
      description: 'Currency accepted for payment if `isAccessibleForFree` is False. A combination of a list of active codes defined in the model. [Norme ISO 4217](http://en.wikipedia.org/wiki/ISO_4217), [Crypto Currencies](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) , [Exchange Trading System](https://en.wikipedia.org/wiki/Local_exchange_trading_system)'    
      items:    
        enum:    
          - EUR    
          - USD    
        type: string    
      type: array    
      x-ngsi:    
        model: https://schema.org/currenciesAccepted    
        type: Property    
    dataProvider:    
      description: 'A sequence of characters identifying the provider of the harmonised data entity.'    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: 'Entity creation timestamp. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: 'Timestamp of the last modification of the entity. This will usually be allocated by the storage platform.'    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: 'A description of this item'    
      type: string    
      x-ngsi:    
        type: Property    
    director:    
      description: 'List of director who manage the composition.'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    doorTimeClose:    
      description: 'Doors closing time to access the show..'    
      type: string    
      x-ngsi:    
        type: Property    
    doorTimeOpen:    
      description: 'Doors opening time to access the show.'    
      type: string    
      x-ngsi:    
        type: Property    
    duration:    
      description: 'The duration of each show. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **HUR** represents **Hours**.'    
      type: number    
      x-ngsi:    
        type: Property    
    electricTransport:    
      description: ' List of the different types of electric transport proposed by the city. A combination of. Enum:''electricBicycle, electricCar, electricMotorBike, electricScooter'''    
      items:    
        enum:    
          - electricBicycle    
          - electricCar    
          - electricMotorBike    
          - electricScooter    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    endDate:    
      description: 'The end date and time of the item (in ISO 8601 date format).'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/endDate    
        type: Property    
    eventPriceFrom:    
      description: 'Min Price. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **EUR** represents **€uro**.'    
      type: number    
      x-ngsi:    
        type: Property    
    eventPriceTo:    
      description: 'Max Price. The unit code (text) of measurement is given using the [UN/CEFACT Common Codes](http://wiki.goodrelations-vocabulary.org/Documentation/UN/CEFACT_Common_Codes). For instance, **EUR** represents **€uro**.'    
      type: number    
      x-ngsi:    
        type: Property   
    eventSchedule:    
      description: 'An Event that is associated with a Schedule using this property should not have `startDate` or `endDate` properties. These are instead defined within the associated Schedule, this avoids any ambiguity for clients using the data. The property might have repeated values to specify different schedules (different months or seasons).*** '    
      items:    
        properties:    
          byDay:    
            type: string    
          byMonth:    
            type: number    
          byMonthDay:    
            type: number    
          byMonthWeek:    
            type: number    
          dayOfWeek:    
            enum:    
              - Monday    
              - Tuesday    
              - Wednesday    
              - Thursday    
              - Friday    
              - Saturday    
              - Sunday    
              - PublicHolidays    
            type: string    
          duration:    
            type: number    
          exceptDate:    
            format: date-time    
            type: string    
          repeatCount:    
            type: number    
          repeatFrequency:    
            type: string    
      type: array    
      x-ngsi:    
        type: Property    
    eventStatus:    
      description: 'Event Status regarding this event.'    
      items:    
        enum:    
          - opened    
          - closed    
          - suspended    
          - cancelled    
          - scheduled    
          - finished    
          - postponed    
          - rescheduled    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    id:    
      anyOf: &event_-_properties_-_owner_-_items_-_anyof    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Unique identifier of the entity'    
      x-ngsi:    
        type: Property    
    isAccessibleForFree:    
      description: 'A flag to signal that the item, event, or place is accessible for free.'    
      type: boolean    
      x-ngsi:    
        model: https://schema.org/isAccessibleForFree    
        type: Property    
    language:    
      description: ' List of Formal language used during the Event expressed from the IETF [BCP 47](https://tools.ietf.org/html/bcp47) standard'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        model: https://schema.org/language    
        type: Property    
    location:    
      description: 'Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon'    
      oneOf:    
        - description: 'Geoproperty. Geojson reference to the item. Point'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                type: number    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - Point    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON Point'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. LineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              minItems: 2    
              type: array    
            type:    
              enum:    
                - LineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON LineString'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. Polygon'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 4    
                type: array    
              type: array    
            type:    
              enum:    
                - Polygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON Polygon'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiPoint'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  type: number    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPoint    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiPoint'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiLineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    type: number    
                  minItems: 2    
                  type: array    
                minItems: 2    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiLineString    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiLineString'    
          type: object    
        - description: 'Geoproperty. Geojson reference to the item. MultiLineString'    
          properties:    
            bbox:    
              items:    
                type: number    
              minItems: 4    
              type: array    
            coordinates:    
              items:    
                items:    
                  items:    
                    items:    
                      type: number    
                    minItems: 2    
                    type: array    
                  minItems: 4    
                  type: array    
                type: array    
              type: array    
            type:    
              enum:    
                - MultiPolygon    
              type: string    
          required:    
            - type    
            - coordinates    
          title: 'GeoJSON MultiPolygon'    
          type: object    
      x-ngsi:    
        type: Geoproperty    
    maximumAttendeeCapacity:    
      description: 'The total number of people who can attend to the Event at that location.'    
      type: number    
      x-ngsi:    
        type: Property    
    name:    
      description: 'The name of this item.'    
      type: string    
      x-ngsi:    
        type: Property    
    openingHoursSpecification:    
      description: 'A structured value providing information about the opening hours of a place or a certain service inside a place'    
      items:    
        properties:    
          closes:    
            format: time    
            type: string    
          dayOfWeek:    
            enum:    
              - Monday    
              - Tuesday    
              - Wednesday    
              - Thursday    
              - Friday    
              - Saturday    
              - Sunday    
              - PublicHolidays    
            type: string    
          opens:    
            format: time    
            type: string    
          validFrom:    
            format: date-time    
            type: string    
          validThrough:    
            format: date-time    
            type: string    
      minItems: 1    
      type: array    
      x-ngsi:    
        model: https://schema.org/openingHoursSpecification    
        type: Property    
    owner:    
      description: 'A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)'    
      items:    
        anyOf: *event_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Property    
    paymentAccepted:    
      description: 'Accepted payment if `isAccessibleForFree` is False. A combination of a list of active codes defined in the model. Enum:''Cash, CreditCard, CryptoCurrency, other'''    
      items:    
        enum:    
          - Cash    
          - CreditCard    
          - CryptoCurrency    
          - other    
        type: string    
      type: array    
      x-ngsi:    
        model: https://schema.org/paymentAccepted    
        type: Property    
    performer:    
      description: 'Main actor or presenter or musician or musical group of the event.'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    pitch:    
      description: "Pitch of the Event. Each items have the format based on the [Internationalization (i18N) - W3C recommandation for multilanguage](https://www.w3.org/TR/json-ld/#string-internationalization) integrating all items in a single property (ex number 71). Each item is represented by a string with Language Value : Article Value. "    
      items:    
        properties:    
          article:    
            type: string    
          language:    
            type: string    
        type: object    
      type: array    
      x-ngsi:    
        type: Property    
    priceSpecification:    
      description: 'A structured value representing a price or price range depending categories or public.'    
      items:    
        properties:    
          audience:    
            items:    
              type: string    
            type: array    
          categoryDescription:    
            type: string    
          eligibleQuantity:    
            type: number    
          maxPrice:    
            type: number    
          minPrice:    
            type: number    
          price:    
            type: number    
        type: object    
      type: array    
      x-ngsi:    
        type: Property    
    publicAccess:    
      description: 'A flag to signal that the Place is open to public visitors. If this property is omitted there is no assumed default boolean value'    
      type: boolean    
      x-ngsi:    
        model: https://schema.org/publicAccess    
        type: Property    
    ratingValueAverage:    
      description: 'Rating value of Event. Usage guidelines: Use values from 0 to 10 depending on your standard. This is the average value of all detailed scores of `starRatingDetailed` attribute'    
      type: number    
      x-ngsi:    
        type: Property    
    refPointOfInterest:    
      description: 'Reference to all the Point Of interest [PointOfInterest](https://github.com/smart-data-models/dataModel.PointOfInterest/blob/master/PointOfInterest/doc/spec.md) included in the event. The POI list does not have a chronological order.'    
      items:    
        anyOf: *event_-_properties_-_owner_-_items_-_anyof    
        description: 'Property. Unique identifier of the entity'    
      type: array    
      x-ngsi:    
        type: Relationship    
    routeType:    
      description: "List of the urban transports (subway, Bus, Tram, ...) available near the Event according to the GFTS standard [STOP](https://developers.google.com/transit/gtfs/reference/#stopstxt). A combination of values. Enum:' bus, cableCar, cableTram, ferry, funicular, monorail, subway, train, tram, trolleybus'"    
      items:    
        enum:    
          - bus    
          - cableCar    
          - cableTram    
          - ferry    
          - funicular    
          - monorail    
          - subway    
          - train    
          - tram    
          - trolleybus    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    seeAlso:    
      description: 'list of uri pointing to additional resources about the item'    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    slogan:    
      description: 'Event header line, matches the text hook. '    
      type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: 'A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object.'    
      type: string    
      x-ngsi:    
        type: Property    
    starRatingDetailed:    
      description: 'Detailed star ratings which led to the average value expressed in the ratingValue. Instructions for use: A structured value from 1 to 10 occurrences (Stars) where each element is a string in the format: `NumberOfSTar`: Percent. '    
      properties:    
        1:    
          type: number    
        10:    
          type: number    
        2:    
          type: number    
        3:    
          type: number    
        4:    
          type: number    
        5:    
          type: number    
        6:    
          type: number    
        7:    
          type: number    
        8:    
          type: number    
        9:    
          type: number    
      type: object    
      x-ngsi:    
        type: Property    
    startDate:    
      description: 'The start date and time of the item (in ISO 8601 date format).'    
      format: date-time    
      type: string    
      x-ngsi:    
        model: https://schema.org/startDate    
        type: Property    
    subCategory:    
      description: 'Sub-category of the `category` attribute. A combination of free text to remain flexible to a specific context is offered below as an initial example or any other value needed by an application. '    
      items:    
        enum:    
          - --museum--    
          - archaeology    
          - contemporaryArt    
          - modernArt    
          - appliedArts    
          - decorativeArts    
          - scienceAndTechnology    
          - fineArts    
          - music    
          - history    
          - sacredArt    
          - specials    
          - literature    
          - medicineAndPharmacy    
          - maritime    
          - transports    
          - military    
          - wax    
          - popularArtsAndTraditions    
          - numismatic    
          - ceramics    
          - sumptuaryArts    
          - naturalScience    
          - prehistoric    
          - ethnology    
          - railway    
          - mining    
          - textile    
          - sculpture    
          - multiDisciplinar    
          - painting    
          - paleonthology    
          - thematic    
          - architecture    
          - museumHouse    
          - universitary    
          - bullfighting    
          - --excursion--    
          - sea    
          - mountain    
          - river    
          - countryside    
          - ancientCity    
          - cultural    
          - culinary    
          - wineRoute    
          - --parksAndGardens--    
          - park    
          - garden    
          - fountain    
          - --religiousWorship--    
          - church    
          - cathedral    
          - synagogue    
          - mosque    
          - buddhistTemple    
          - hinduTemple    
          - monastery    
          - sanctuary    
          - cemetery    
          - sumptuar    
          - --history--    
          - castle    
          - warMemorials    
          - memorial    
          - fortifiedCastles    
          - archaeologicalSite    
          - crypt    
          - cave    
          - --shopping--    
          - departmentStore    
          - luxuryStores    
          - outlet    
          - mall    
          - clothing    
          - mensClothing    
          - womensClothing    
          - childrenClothing    
          - localProducts    
          - souvenir    
          - wine    
          - pastry    
          - chocolate    
          - confectionery    
          - jewelry    
          - watch    
          - shoe    
          - perfume    
          - cosmetics    
          - press    
          - sport    
          - optics    
          - leatherGoods    
          - decoration    
          - market    
          - bike    
          - book    
          - computer    
          - convenience    
          - electronic    
          - florist    
          - furniture    
          - garden    
          - grocery    
          - home    
          - liquor    
          - mobile    
          - movierental    
          - music    
          - pawnShop    
          - tire    
          - toy    
          - --gastronomy--    
          - worldCuisine    
          - traditional    
          - provencal    
          - mediterranean    
          - greek    
          - spanish    
          - brazilian    
          - lebanese    
          - creole    
          - mauritian    
          - reunion    
          - hawaiian    
          - mexican    
          - american    
          - texMex    
          - vegetarian    
          - fish    
          - seafood    
          - indian    
          - vietnamese    
          - thai    
          - laosian    
          - cambodian    
          - chinese    
          - moroccan    
          - tunisian    
          - african    
          - sushi    
          - japanese    
          - scandinavian    
          - russian    
          - pastry    
          - wine    
          - --outdoorActivities--    
          - rafting    
          - canyoning    
          - aquatichiking    
          - hiking    
          - viaferrata    
          - climbing    
          - kitesurfing    
          - canoeing    
          - paddleboarding    
          - jetSki    
          - catamaran    
          - sailing    
          - surfing    
          - deltaPlane    
          - skiing    
          - scooter    
          - karting    
          - --wellness--    
          - spa    
          - haman    
          - jacuzzi    
          - hotSpring    
          - thalasso    
          - bodyCare    
          - swimmingPool    
          - relaxationArea    
          - massage    
          - careCenter    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    subEvent:    
      description: 'Reference to a list of Minor Events that are part of this major Event'    
      items:    
        anyOf:    
          - description: 'Property. Identifier format of any NGSI entity'    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: 'Property. Identifier format of any NGSI entity'    
            format: uri    
            type: string    
      type: array    
      x-ngsi:    
        type: Property    
    superEvent:    
      anyOf:    
        - description: 'Property. Identifier format of any NGSI entity'    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: 'Property. Identifier format of any NGSI entity'    
          format: uri    
          type: string    
      description: 'Reference to the Major Event that includes this Event.'    
      x-ngsi:    
        type: Property    
    thematic:    
      description: 'A list of thematic as keywords'    
      items:    
        type: string    
      type: array    
      x-ngsi:    
        type: Property    
    title:    
      description: ' Title of the Event.'    
      type: string    
      x-ngsi:    
        type: Property    
    touristType:    
      description: 'Type of tourism depending on the segment and the motivation of the event.'    
      enum:    
        - 'ADVENTURE TOURISM'    
        - 'ASTRONOMY TOURISM'    
        - 'BACKPACKING TOURISM'    
        - 'BEACH AND SUN TOURISM'    
        - 'BEER TOURISM'    
        - 'BIRDING TOURISM'    
        - 'BULLFIGHTING TOURISM'    
        - BUSINESS    
        - 'COMMUNITY-BASED TOURISM'    
        - 'CRUISE TOURISM'    
        - 'CULTURAL TOURISM'    
        - 'CYCLING TOURISM'    
        - 'DIVING TOURISM'    
        - ECOTOURISM    
        - 'EVENTS AND FESTIVALS TOURISM'    
        - 'FAMILY TOURISM'    
        - 'FILM TOURISM'    
        - 'FISHING TOURISM'    
        - 'FOOD TOURISM'    
        - 'GAMBLING TOURISM'    
        - 'GEOLOGICAL TOURISM'    
        - 'HERITAGE TOURISM'    
        - 'HUNTING TOURISM'    
        - 'INDUSTRIAL TOURISM'    
        - 'LANGUAGE TOURISM'    
        - 'LGTBI TOURISM'    
        - 'LUXURY TOURISM'    
        - 'MEDICAL TOURISM'    
        - 'MEMORIAL TOURISM'    
        - 'MICE TOURISM'    
        - 'NATURE TOURISM'    
        - 'OLIVE OIL TOURISM'    
        - 'PARTY TOURISM'    
        - 'PHOTOGRAPHY TOURISM'    
        - 'RELIGIOUS TOURISM'    
        - 'ROMANTIC TOURISM'    
        - 'RURAL TOURISM'    
        - 'SAFARI TOURISM'    
        - 'SAILING TOURISM'    
        - 'SENIOR TOURISM'    
        - 'SHOPPING TOURISM'    
        - 'SHORT BREAK TOURISM'    
        - 'SINGLES TOURISM'    
        - 'SPORTS TOURISM'    
        - TOURISM    
        - 'TREKKING TOURISM'    
        - 'URBAN TOURISM'    
        - 'WATER SPORTS TOURISM'    
        - 'WEDDING & HONEYMOON TOURISM'    
        - 'WELLNESS TOURISM'    
        - 'WHISKY TOURISM'    
        - 'WINE TOURISM'    
        - 'WINTER SPORTS TOURISM'    
        - 'WOMEN TOURISM'    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    transportServices:    
      description: 'List of private transport available near the Event. In example taxi, uber, vtc, parkingShuttle '    
      items:    
        enum:    
          - parkingShuttle    
          - taxi    
          - uber    
          - vtc    
        type: string    
      type: array    
      x-ngsi:    
        type: Property     
    type:    
      description: 'It has to be Event'    
      enum:    
        - Event    
      type: string    
      x-ngsi:    
        model: https://schema.org/event    
        type: Property    
    url:    
      description: 'Url with image related to the item'    
      format: uri    
      type: string    
      x-ngsi:    
        model: https://schema.org/URL    
        type: Property    
    webSite:    
      description: 'Link to the official website for more information.'    
      format: uri    
      type: string    
      x-ngsi:    
        type: Property    
    wheelChairAccessible:    
      description: 'Access possible for Person with Reduced Mobility.'    
      type: boolean    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
  type: object    
  x-derived-from: ""    
  x-disclaimer: 'Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program'    
  x-license-url: https://github.com/smart-data-models/dataModel.TourismDestinations/blob/master/Event/LICENSE.md    
  x-model-schema: https://smart-data-models.github.io/dataModel.TourismDestinations/Event/schema.json    
  x-model-tags: ""    
  x-version: 0.0.1    
```  
</details>    

## Example payloads    

#### Event NGSI-v2 key-values Example    

Here is an example of a Event in JSON-LD format as key-values. This is compatible with NGSI-v2 when  using `options=keyValues` and returns the context data of an individual entity.  

```json  

{  
  "id": "urn:ngsi-ld:Event:Event:MNCA-EV-NCE-12552-MARIAGEDENFER",  
  "type": "Event",  
  "name": "MARIAGE D ENFER",  
  "alternateName": "Elle en revait, il l a fait : ils vont se marier !",  
  "description": "Information sur la piéce de théatre",  
  "seeAlso": "https://www.billetreduc.com/260539/evt.htm",  
  "location": {  
    "type": "Point",  
    "coordinates": [  
      43.7062,  
      7.26267  
    ]  
  },  
  "address": {  
    "streetAddress": "14 rue Trachel - Bat. B",  
    "postalCode": "06000",  
    "addressLocality": "Nice",  
    "addressCountry": "France",  
    "addressRegion": "Marseille Nice Avignon Aix - (06)"  
  },  
  "areaServed": "Gare de Nice",  
  "dateLastReported": "2020-03-17T08:45:00Z",  
  "contactPoint": {  
    "telephone": "+33(0)4 93 87 08 87",  
    "contactType": "customer reception",  
    "email": "theatrebellecour@gmail.com",  
    "availableLanguage": [  
      "English",  
      "French"  
    ]  
  },  
  "accessPlan": "https://www.billetreduc.com/lieu/nice/theatre-bellecour/#planAcces",  
  "category": [  
    "spectacle"  
  ],  
  "subCategory": [  
    "cabaret",  
    "theater",  
    "boulevard",  
    "vaudeville",  
    "humor"  
  ],  
  "thematic": [  
    "humor"  
  ],  
  "superEvent": "urn:ngsi-ld:Event:Event:MNCA-EV-NCE-12552-FESTIVAL-THEATRE-NICE",  
  "eventStatus": [  
    "scheduled"  
  ],  
  "locationName": "Théâtre Bellecour",  
  "title": "MARIAGE D ENFER",  
  "slogan": "Elle en revait, il l a fait : ils vont se marier !",  
  "language": [  
    "French"  
  ],  
  "startDate": "2020-08-01T01:20:00Z",  
  "endDate": "2020-10-18T01:20:00Z",  
  "openingHoursSpecification": [  
    {  
      "validFrom": "2020-08-08T00:00:00Z",  
      "validThrough": "2020-08-31T00:00:00Z",  
      "dayOfWeek": "Saturday",  
      "Opens": "21.00"  
    },  
    {  
      "validFrom": "2020-08-08T00:00:00Z",  
      "validThrough": "2020-08-31T00:00:00Z",  
      "dayOfWeek": "Sunday",  
      "Opens": "19.00"  
    },  
    {  
      "validFrom": "2020-09-01T00:00:00Z",  
      "validThrough": "2020-10-18T00:00:00Z",  
      "dayOfWeek": "Friday",  
      "Opens": "21.00"  
    },  
    {  
      "validFrom": "2020-09-01T00:00:00Z",  
      "validThrough": "2020-10-18T00:00:00Z",  
      "dayOfWeek": "Saturday"  
    },  
    {  
      "validFrom": "2020-09-01T00:00:00Z",  
      "validThrough": "2020-10-18T00:00:00Z",  
      "dayOfWeek": "Sunday",  
      "Opens": "19.00"  
    }  
  ],  
  "duration": 1.25,  
  "doorTimeOpen": "30 mn before the show",  
  "doorTimeClose": "10 mn before the show",  
  "pitch": [  
    {  
      "language ": "fr",  
      "article": "Heureusement pour Max, la wedding planner c est elle, et elle a déjà tout anticipé dans le moindre détail ! Tout ? Peut-être pas... En tout cas, un mariage ça se gère à deux... Et les conflits aussi ! Quand on dit pour le meilleur et pour le pire, le pire c est certainement les préparatifs d un mariage ! Que vous soyez mariés, fiancés, en couple, juste amis ou célibataire, cette comédie est faite pour vous ! Venez découvrir les coulisses des préparatifs d un mariage haut en couleurs avant de faire le grand saut !"  
    },  
    {  
      "language": "en",  
      "article": "But before that there are some details to settle and Elo knows it well: A beautiful wedding, cannnot be organized just like that! Fortunately for Max, the wedding planner is her, and she has already anticipated everything in every detail! Evrything ? Maybe not... In any case, a marriage is managed by two ... And conflicts too! When we say for better or for worse, the worst is certainly the preparations for a wedding! Whether married, engaged, in a relationship, just friends or single, this comedy is for you! Come and discover the preparations for a colorful wedding before taking the plunge!"  
    }  
  ],  
  "webSite": "http://www.theatrebellecour.com",  
  "contentURL": "https://www.nicetourisme.com/resources/ref/events/12552/mariage-d-enfer_168.jpg",  
  "performer": [  
    "Lise Giraudier"  
  ],  
  "actor": [  
    "Lise Giraudier",  
    "Richard Zanca",  
    "Vanessa Bellagamba",  
    "Yann Bruno-Martinez"  
  ],  
  "composer": [  
    "Céline Cara"  
  ],  
  "director": [  
    "Sébastien El Fassi"  
  ],  
  "criticReview": [  
    {  
      "language": "fr",  
      "reviews": [  
        {  
          "article": "Comédie à ne pas rater. Tout y est la mère, la belle mère, les copains et avant tout les rires les quiproquos, les retournements et tout cela  enchaîne avec une grande vitesse.  Alors allez  pour feliciter les époux et rire de bon coeur avec eux.",  
          "origin": "Revue Theatrale - L. Dupont",  
          "ratingValue": 9,  
          "starRating": 6  
        }  
      ]  
    }  
  ],  
  "ratingValueAverage": 9.2,  
  "starRatingDetailed": {  
    "5": 94,  
    "4": 6,  
    "3": 0,  
    "2": 0,  
    "1": 0  
  },  
  "audience": [  
    "allPublic"  
  ],  
  "wheelChairAccessible": true,  
  "maximumAttendeeCapacity": 60,  
  "isAccessibleForFree": false,  
  "eventPriceFrom": 10.95,  
  "eventPriceTo": 19.5,  
  "priceSpecification": [  
    {  
      "categoryDescription": "Category 1 : Seat Range 1 to 2",  
      "eligibleQuantity": 20,  
      "price": 19.5  
    },  
    {  
      "categoryDescription": "Category 2 : Seat Range 3 to 6",  
      "eligibleQuantity": 40,  
      "price": 15.95  
    },  
    {  
      "categoryDescription": "Special price from Monday to Wednesday : Category 1 - 2",  
      "eligibleQuantity": 60,  
      "price": 10.95  
    }  
  ],  
  "paymentAccepted": [  
    "Cash",  
    "CreditCard"  
  ],  
  "currencyAccepted": [  
    "EUR",  
    "USD"  
  ],  
  "routeType": [  
    "tram",  
    "subway",  
    "bus"  
  ],  
  "transportServices": [  
    "taxi",  
    "uber",  
    "vtc",  
    "parkingShuttle"  
  ],  
  "electricTransport": [  
    "electricBicycle",  
    "electricMotorBike"  
  ],  
  "@context": [  
    "https://smart-data-models.github.io/data-models/context.jsonld",  
    "https://uri.etsi.org/ngsi-ld/v1/ngsi-ld-core-context.jsonld"  
  ]  
}  
```  

#### Event NGSI-v2 normalized Example    

Here is an example of a Event in JSON-LD format as normalized. This is compatible with NGSI-v2 when not using options and returns the context data of an individual entity.  

```json  

{  
  "id": {  
    "type": "string",  
    "value": "uri:ngsi:event:1"  
  },  
  "type": {  
    "type": "string",  
    "value": "Event"  
  },  
  "name": {  
    "type": "string",  
    "value": "Concierto de Revólver"  
  },  
  "addressLocality": {  
    "type": "string",  
    "value": "Salamanca"  
  },  
  "postalCode": {  
    "type": "string",  
    "value": "37008"  
  },  
  "streetAddress": {  
    "type": "string",  
    "value": "Calle Monte Olivete, s/n"  
  },  
  "startDate": {  
    "type": "string",  
    "value": "2019-06-08T21:00:00"  
  },  
  "endDate": {  
    "type": "string",  
    "value": "2019-06-08T23:00:00"  
  },  
  "url": {  
    "type": "string",  
    "value": "https://www.notikumi.com/2019/6/8/evento-de-revolver-en-salamanca"  
  },  
  "offeredBy": {  
    "type": "object",  
    "value": {  
      "type": "Organization",  
      "name": "Notikumi",  
      "url": "https://www.notikumi.com/"  
    }  
  },  
  "touristType": {  
    "type": "string",  
    "value": "EVENTS AND FESTIVALS TOURISM"  
  }  
}  
```  

#### Event NGSI-LD key-values Example    

Here is an example of a Event in JSON-LD format as key-values. This is compatible with NGSI-LD when  using `options=keyValues` and returns the context data of an individual entity.  

```json  

{  
  "id": "uri:ngsi:event:1",  
  "type": "Event",  
  "name": "Concierto de Rev\u00f3lver",  
  "addressLocality": "Salamanca",  
  "postalCode": "37008",  
  "streetAddress": "Calle Monte Olivete, s/n",  
  "startDate": "2019-06-08T21:00:00",  
  "endDate": "2019-06-08T23:00:00",  
  "url": "https://www.notikumi.com/2019/6/8/evento-de-revolver-en-salamanca",  
  "offeredBy": {  
    "type": "Organization",  
    "name": "Notikumi",  
    "url": "https://www.notikumi.com/"  
  },  
  "touristType": "EVENTS AND FESTIVALS TOURISM",  
  "@context": [  
    "https://smartdatamodels.org/context.jsonld"  
  ]  
}  
```  

#### Event NGSI-LD normalized Example    

Here is an example of a Event in JSON-LD format as normalized. This is compatible with NGSI-LD when not using options and returns the context data of an individual entity.  

```json  

{  
  "id": "urn:ngsi-ld:Event:Event:MNCA-EV-NCE-12552-MARIAGEDENFER",  
  "type": "Event",  
  "name": {  
    "type": "Property",  
    "value": "MARIAGE D ENFER"  
  },  
  "alternateName": {  
    "type": "Property",  
    "value": "Elle en revait, il l a fait : ils vont se marier !"  
  },  
  "description": {  
    "type": "Property",  
    "value": "Information sur la piéce de théatre"  
  },  
  "seeAlso": {  
    "type": "Property",  
    "value": "https://www.billetreduc.com/260539/evt.htm"  
  },  
  "location": {  
    "type": "Geoproperty",  
    "value": {  
      "type": "Point",  
      "coordinates": [  
        43.7062,  
        7.26267  
      ]  
    }  
  },  
  "address": {  
    "type": "Property",  
    "value": {  
      "streetAddress": "14 rue Trachel - Bat. B",  
      "postalCode": "06000",  
      "addressLocality": "Nice",  
      "addressCountry": "France",  
      "addressRegion": "Marseille Nice Avignon Aix - (06)"  
    }  
  },  
  "areaServed": {  
    "type": "Property",  
    "value": "Gare de Nice"  
  },  
  "dateLastReported": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2020-03-17T08:45:00Z"  
    }  
  },  
  "contactPoint": {  
    "type": "Property",  
    "value": {  
      "telephone": "+33(0)4 93 87 08 87",  
      "contactType": "customer reception",  
      "email": "theatrebellecour@gmail.com",  
      "availableLanguage": [  
        "English",  
        "French"  
      ]  
    }  
  },  
  "accessPlan": {  
    "type": "Property",  
    "value": "https://www.billetreduc.com/lieu/nice/theatre-bellecour/#planAcces"  
  },  
  "category": {  
    "type": "Property",  
    "value": [  
      "spectacle"  
    ]  
  },  
  "subCategory": {  
    "type": "Property",  
    "value": [  
      "cabaret",  
      "theater",  
      "boulevard",  
      "vaudeville",  
      "humor"  
    ]  
  },  
  "thematic": {  
    "type": "Property",  
    "value": [  
      "humor"  
    ]  
  },  
  "superEvent": {  
    "type": "Property",  
    "value": "urn:ngsi-ld:Event:Event:MNCA-EV-NCE-12552-FESTIVAL-THEATRE-NICE"  
  },  
  "eventStatus": {  
    "type": "Property",  
    "value": [  
      "scheduled"  
    ]  
  },  
  "locationName": {  
    "type": "Property",  
    "value": "Théâtre Bellecour"  
  },  
  "title": {  
    "type": "Property",  
    "value": "MARIAGE D ENFER"  
  },  
  "slogan": {  
    "type": "Property",  
    "value": "Elle en revait, il l a fait : ils vont se marier !"  
  },  
  "language": {  
    "type": "Property",  
    "value": [  
      "French"  
    ]  
  },  
  "startDate": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2020-08-01T01:20:00Z"  
    }  
  },  
  "endDate": {  
    "type": "Property",  
    "value": {  
      "@type": "DateTime",  
      "@value": "2020-10-18T01:20:00Z"  
    }  
  },  
  "openingHoursSpecification": {  
    "type": "Property",  
    "value": [  
      {  
        "validFrom": "2020-08-08T00:00:00Z",  
        "validThrough": "2020-08-31T00:00:00Z",  
        "dayOfWeek": "Saturday",  
        "Opens": "21.00"  
      },  
      {  
        "validFrom": "2020-08-08T00:00:00Z",  
        "validThrough": "2020-08-31T00:00:00Z",  
        "dayOfWeek": "Sunday",  
        "Opens": "19.00"  
      },  
      {  
        "validFrom": "2020-09-01T00:00:00Z",  
        "validThrough": "2020-10-18T00:00:00Z",  
        "dayOfWeek": "Friday",  
        "Opens": "21.00"  
      },  
      {  
        "validFrom": "2020-09-01T00:00:00Z",  
        "validThrough": "2020-10-18T00:00:00Z",  
        "dayOfWeek": "Saturday"  
      },  
      {  
        "validFrom": "2020-09-01T00:00:00Z",  
        "validThrough": "2020-10-18T00:00:00Z",  
        "dayOfWeek": "Sunday",  
        "Opens": "19.00"  
      }  
    ]  
  },  
  "duration": {  
    "type": "Property",  
    "value": 1.25  
  },  
  "doorTimeOpen": {  
    "type": "Property",  
    "value": "30 mn before the show"  
  },  
  "doorTimeClose": {  
    "type": "Property",  
    "value": "10 mn before the show"  
  },  
  "pitch": {  
    "type": "Property",  
    "value": [  
      {  
        "language ": "fr",  
        "article": "Heureusement pour Max, la wedding planner c est elle, et elle a déjà tout anticipé dans le moindre détail ! Tout ? Peut-être pas... En tout cas, un mariage ça se gère à deux... Et les conflits aussi ! Quand on dit pour le meilleur et pour le pire, le pire c est certainement les préparatifs d un mariage ! Que vous soyez mariés, fiancés, en couple, juste amis ou célibataire, cette comédie est faite pour vous ! Venez découvrir les coulisses des préparatifs d un mariage haut en couleurs avant de faire le grand saut !"  
      },  
      {  
        "language": "en",  
        "article": "But before that there are some details to settle and Elo knows it well: A beautiful wedding, cannnot be organized just like that! Fortunately for Max, the wedding planner is her, and she has already anticipated everything in every detail! Evrything ? Maybe not... In any case, a marriage is managed by two ... And conflicts too! When we say for better or for worse, the worst is certainly the preparations for a wedding! Whether married, engaged, in a relationship, just friends or single, this comedy is for you! Come and discover the preparations for a colorful wedding before taking the plunge!"  
      }  
    ]  
  },  
  "webSite": {  
    "type": "Property",  
    "value": "http://www.theatrebellecour.com"  
  },  
  "contentURL": {  
    "type": "Property",  
    "value": "https://www.nicetourisme.com/resources/ref/events/12552/mariage-d-enfer_168.jpg"  
  },  
  "url": {  
    "type": "string",  
    "value": "https://www.notikumi.com/2019/6/8/evento-de-revolver-en-salamanca"  
  },  
  "performer": {  
    "type": "Property",  
    "value": [  
      "Lise Giraudier"  
    ]  
  },  
  "actor": {  
    "type": "Property",  
    "value": [  
      "Lise Giraudier",  
      "Richard Zanca",  
      "Vanessa Bellagamba",  
      "Yann Bruno-Martinez"  
    ]  
  },  
  "composer": {  
    "type": "Property",  
    "value": [  
      "Céline Cara"  
    ]  
  },  
  "director": {  
    "type": "Property",  
    "value": [  
      "Sébastien El Fassi"  
    ]  
  },  
  "criticReview": {  
    "type": "Property",  
    "value": [  
      {  
        "language": "fr",  
        "reviews": [  
          {  
            "article": "Comédie à ne pas rater. Tout y est la mère, la belle mère, les copains et avant tout les rires les quiproquos, les retournements et tout cela  enchaîne avec une grande vitesse.  Alors allez  pour feliciter les époux et rire de bon coeur avec eux.",  
            "origin": "Revue Theatrale - L. Dupont",  
            "ratingValue": 9,  
            "starRating": 6  
          }  
        ]  
      }  
    ]  
  },  
  "ratingValueAverage": {  
    "type": "number",  
    "value": 9.2  
  },  
  "starRatingDetailed": {  
    "type": "object",  
    "value": {  
      "5": 94,  
      "4": 6,  
      "3": 0,  
      "2": 0,  
      "1": 0  
    }  
  },  
  "audience": {  
    "type": "Property",  
    "value": [  
      "allPublic"  
    ]  
  },  
  "wheelChairAccessible": {  
    "type": "boolean",  
    "value": "true"  
  },  
  "maximumAttendeeCapacity": {  
    "type": "number",  
    "value": 60  
  },  
  "isAccessibleForFree": {  
    "type": "boolean",  
    "value": "false"  
  },  
  "eventPriceFrom": {  
    "type": "number",  
    "value": 10.95  
  },  
  "eventPriceTo": {  
    "type": "number",  
    "value": 19.5  
  },  
  "priceSpecification": {  
    "type": "Property",  
    "value": [  
      {  
        "categoryDescription": "Category 1 : Seat Range 1 to 2",  
        "eligibleQuantity": 20,  
        "price": 19.5  
      },  
      {  
        "categoryDescription": "Category 2 : Seat Range 3 to 6",  
        "eligibleQuantity": 40,  
        "price": 15.95  
      },  
      {  
        "categoryDescription": "Special price from Monday to Wednesday : Category 1 - 2",  
        "eligibleQuantity": 60,  
        "price": 10.95  
      }  
    ]  
  },  
  "paymentAccepted": {  
    "type": "Property",  
    "value": [  
      "Cash",  
      "CreditCard"  
    ]  
  },  
  "currencyAccepted": {  
    "type": "Property",  
    "value": [  
      "EUR",  
      "USD"  
    ]  
  },  
  "routeType": {  
    "type": "Property",  
    "value": [  
      "tram",  
      "subway",  
      "bus"  
    ]  
  },  
  "transportServices": {  
    "type": "Property",  
    "value": [  
      "taxi",  
      "uber",  
      "vtc",  
      "parkingShuttle"  
    ]  
  },  
  "electricTransport": {  
    "type": "Property",  
    "value": [  
      "electricBicycle",  
      "electricMotorBike"  
    ]  
  },  
  "offeredBy": {  
    "type": "Property",  
    "value": {  
      "type": "Organization",  
      "name": "Notikumi",  
      "url": "https://www.notikumi.com/"  
    }  
  },  
  "touristType": {  
    "type": "Property",  
    "value": "EVENTS AND FESTIVALS TOURISM"  
  },  
  "@context": [  
    "https://smartdatamodelsorg/context.jsonld"  
  ]  
}  
```  
See [FAQ 10](https://smartdatamodels.org/index.php/faqs/) to get an answer on how to deal with magnitude units

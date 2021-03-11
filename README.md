Rejseplanen XSD documents
=========================

## Motivation

As it seems these schemas are not available on the internet anymore, or at least not on the url referenced in the XML files, I decided to recreate them from the PDF documentation.

[The source PDF](https://p3.zdassets.com/hc/theme_assets/497496/200019391/ReST_documentation_Rejseplanen_Latest.pdf)

## Schemas

#### Location response

The location consists of a list of entries, which are either stops/stations or named coordinates.

The root element of the response is `LocationList`

[hafasRestLocation.xsd](schema/hafasRestLocation.xsd)

#### Trip response

The trip response consists of a list of trips.

Every trip has one to many legs with an origin and destination. 

The root element of the response is `TripList`.

[hafasRestTrip.xsd](schema/hafasRestTrip.xsd)

#### Departure board response

The departure board response contains a list of departures incl. all information concerning times, tracks, realtime data and journey.

It also contains reference URLs to get more details for the different journeys.

The root element is `DepartureBoard`

[hafasRestDepartureBoard.xsd](schema/hafasRestDepartureBoard.xsd)

#### Arrival board response

The arrival board response contains a list of arrivals incl. all information concerning times, tracks, realtime data and journeys.

It also contains reference URLs to get more details for the different journeys.

The root element is `ArrivalBoard`

[hafasRestArrivalBoard.xsd](schema/hafasRestArrivalBoard.xsd)

#### Multi departure board response

The multi departure board response contains a list of departures incl. all information concerning times, tracks, realtime data and journeys.

It also contains reference URLs to get more details for the different journeys.

The root element is `MultiDepartureBoard`

[hafasRestMultiDepartureBoard.xsd](schema/hafasRestMultiDepartureBoard.xsd)

#### Stops nearby response

The stops nearby response contains a list of stop locations.

The root element is `LocationList`

[hafasRestStopsNearby.xsd](schema/hafasRestStopsNearby.xsd)

#### Journey detail response

The journey detail response delivers all information about a single journey (vehicle route).

It contains a list of a stops including their indexes on the route and their coordinates.

It contains also all times, tracks and realtime information if available for the whole route.

It also contains the journeys name and type (there might be different names and types on parts of the journey), finally it contains notes including information about their validity on segments of the total route and messages which can contain additional information for a journey.

The root element is `JourneyDetail`

[hafasRestJourneyDetail.xsd](schema/hafasRestJourneyDetail.xsd)

## XSD in `_play`

Just my own mess to make the XSDs streamlined - Do NOT use!

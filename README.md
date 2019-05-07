# ![LOGO](logo.png) ClickMeter **flow**ground Connector

## Description

A generated **flow**ground connector for the ClickMeter API (version v2).

Generated from: https://api.apis.guru/v2/specs/clickmeter.com/v2/swagger.json<br/>
Generated at: 2019-05-07T17:40:03+03:00

## API Description

Api dashboard for ClickMeter API

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Retrieve current account data

*Tags:* `Account`

### Update current account data

*Tags:* `Account`

### Retrieve list of a domains allowed to redirect in DDU mode

*Tags:* `Account`

#### Input Parameters
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number

### Create an domain entry

*Tags:* `Account`

### Delete an domain entry

*Tags:* `Account`

#### Input Parameters
* `whitelistId` - _required_ - The id of the domain to delete

### Retrieve list of a guest

*Tags:* `Account`

#### Input Parameters
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `textSearch` - _optional_ - Filter fields by this pattern

### Create a guest

*Tags:* `Account`

### Retrieve count of guests

*Tags:* `Account`

#### Input Parameters
* `textSearch` - _optional_ - Filter fields by this pattern

### Delete a guest

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest

### Retrieve a guest

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest

### Update a guest

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest

### Retrieve permissions for a guest

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest
* `entityType` - _optional_ - Can be "datapoint" or "group"
    Possible values: datapoint, group.
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `type` - _optional_ - Can be "w" or "r"
    Possible values: r, w.
* `entityId` - _optional_ - Optional id of the datapoint/group entity to filter by

### Retrieve count of the permissions for a guest

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest
* `entityType` - _optional_ - Can be "datapoint" or "group"
    Possible values: datapoint, group.
* `type` - _optional_ - Can be "w" or "r"
    Possible values: r, w.
* `entityId` - _optional_ - Optional id of the datapoint/group entity to filter by

### Change the permission on a shared object

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest
* `type` - _required_ - Can be "datapoint" or "group"
    Possible values: datapoint, group.

### Change the permission on a shared object

*Tags:* `Account`

#### Input Parameters
* `guestId` - _required_ - Id of the guest
* `type` - _required_ - Can be "datapoint" or "group"
    Possible values: datapoint, group.

### Retrieve list of a ip to exclude from event tracking

*Tags:* `Account`

#### Input Parameters
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number

### Create an ip blacklist entry

*Tags:* `Account`

### Delete an ip blacklist entry

*Tags:* `Account`

#### Input Parameters
* `blacklistId` - _required_ - The id of the ip to delete

### Retrieve current account plan

*Tags:* `Account`

### Retrieve statistics about this customer for a timeframe

*Tags:* `Aggregated`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail
* `onlyFavorites` - _optional_

### Retrieve statistics about this customer for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `Aggregated`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Retrieve statistics about a subset of conversions for a timeframe with conversions data

*Tags:* `Aggregated`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of conversion ("deleted"/"active")
    Possible values: deleted, active.
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `textSearch` - _optional_ - Filter fields by this pattern

### Retrieve statistics about a subset of datapoints for a timeframe with datapoints data

*Tags:* `Aggregated`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `type` - _required_ - Type of datapoint ("tl"/"tp")
    Possible values: tp, tl.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
    Possible values: deleted, active, paused, spam.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the datapoint marked as favourite
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `groupId` - _optional_ - Filter by this group id
* `textSearch` - _optional_ - Filter fields by this pattern

### Retrieve statistics about a subset of groups for a timeframe with groups data

*Tags:* `Aggregated`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of group ("deleted"/"active")
    Possible values: deleted, active.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the group marked as favourite
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `textSearch` - _optional_ - Filter fields by this pattern

### Retrieve the latest list of events of this account. Limited to last 100.

*Tags:* `ClickStream`

#### Input Parameters
* `group` - _optional_ - Filter by this group id (mutually exclusive with "datapoint" and "conversion")
* `datapoint` - _optional_ - Filter by this datapoint id (mutually exclusive with "group" and "conversion")
* `conversion` - _optional_ - Filter by this conversion id (mutually exclusive with "datapoint" and "group")
* `pageSize` - _optional_ - Limit results to this number
* `filter` - _optional_ - Filter event type ("spiders"/"uniques"/"nonuniques"/"conversions")
    Possible values: , spiders, uniques, nonuniques, conversions.

### Retrieve a list of conversions

*Tags:* `Conversions`

#### Input Parameters
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `status` - _optional_ - Status of conversion ("deleted"/"active")
    Possible values: deleted, active.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude conversions created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude conversions created after this date (YYYYMMDD)

### Create a conversion

*Tags:* `Conversions`

### Retrieve statistics about this customer for a timeframe related to a subset of conversions grouped by some temporal entity (day/week/month)

*Tags:* `Conversions`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of conversion ("deleted"/"active")
    Possible values: deleted, active.
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Retrieve a count of conversions

*Tags:* `Conversions`

#### Input Parameters
* `status` - _optional_ - Status of conversion ("deleted"/"active")
    Possible values: deleted, active.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude conversions created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude conversions created after this date (YYYYMMDD)

### Delete conversion specified by id

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Retrieve conversion specified by id

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Update conversion specified by id

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Retrieve statistics about this conversion for a timeframe

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `tag` - _optional_ - Filter by this tag name
* `favourite` - _optional_ - Is the datapoint marked as favourite
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail

### Retrieve statistics about this conversion for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Retrieve a list of datapoints connected to this conversion

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `type` - _optional_ - Type of datapoint ("tl"/"tp")
    Possible values: tp, tl.
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - Filter by this tag name
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Modify the association between a conversion and multiple datapoints

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Retrieve a count of datapoints connected to this conversion

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `type` - _optional_ - Type of datapoint ("tl"/"tp")
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
* `tags` - _optional_ - Filter by this tag name
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Modify the association between a conversion and a datapoint

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Retrieve the list of events related to this conversion.

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, custom.
* `limit` - _optional_ - Limit results to this number
* `offset` - _optional_ - Offset where to start from (it's the lastKey field in the response object)
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `filter` - _optional_ - Filter event type ("spiders"/"uniques"/"nonuniques"/"conversions")
    Possible values: spiders, uniques, nonuniques, conversions.

### Fast patch the "notes" field of a conversion

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion

### Retrieve a top report connected to this conversion

*Tags:* `Conversions`

#### Input Parameters
* `conversionId` - _required_ - Id of the conversion
* `type` - _required_ - Type of the report.
    Possible values: datapoints, groups, browsers, browsersfamilies, platforms, cities, countries, keywords, referrers, convparameters, destinations, languages, params.
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, beginning, custom.
* `hittype` - _optional_ - Type of the event you want to filter this report with. By default no filter is applied.
    Possible values: clicks, views.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)

### List of all the datapoints associated to the user

*Tags:* `DataPoints`

#### Input Parameters
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Create a datapoint

*Tags:* `DataPoints`

### Retrieve statistics about this customer for a timeframe by groups

*Tags:* `DataPoints`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `type` - _optional_ - Type of datapoint ("tl"/"tp")
    Possible values: tp, tl.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
    Possible values: deleted, active, paused, spam.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the datapoint is marked as favourite

### Retrieve statistics about all datapoints of this customer for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `DataPoints`

#### Input Parameters
* `type` - _required_ - Type of datapoint ("tl"/"tp")
    Possible values: tp, tl.
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
    Possible values: deleted, active, paused, spam.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the datapoint is marked as favourite
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Delete multiple datapoints

*Tags:* `DataPoints`

### Update multiple datapoints

*Tags:* `DataPoints`

### Create multiple datapoints

*Tags:* `DataPoints`

### Count the datapoints associated to the user

*Tags:* `DataPoints`

#### Input Parameters
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Delete a datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - The id of the datapoint

### Get a datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - The id of the datapoint

### Update a datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - The id of the datapoint

### Retrieve statistics about this datapoint for a timeframe

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail

### Retrieve statistics about this datapoint for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Fast switch the "favourite" field of a datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint

### Retrieve the list of events related to this datapoint.

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, custom.
* `limit` - _optional_ - Limit results to this number
* `offset` - _optional_ - Offset where to start from (it's the lastKey field in the response object)
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `filter` - _optional_ - Filter event type ("spiders"/"uniques"/"nonuniques"/"conversions")
    Possible values: spiders, uniques, nonuniques, conversions.

### Fast patch the "notes" field of a datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint

### Retrieve a top report connected to this datapoint

*Tags:* `DataPoints`

#### Input Parameters
* `id` - _required_ - Id of the datapoint
* `type` - _required_ - Type of the report.
    Possible values: browsers, browsersfamilies, platforms, cities, countries, isps, ips, oss, ossfamilies, keywords, referrers, destinations, languages, params.
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)

### Retrieve a list of domains

*Tags:* `Domains`

#### Input Parameters
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `type` - _optional_ - Type of domain ("system"/"go"/"personal"/"dedicated"). If not specified default is "system"
    Possible values: system, go, personal, dedicated.
* `name` - _optional_ - Filter domains with this anmen

### Create a domain

*Tags:* `Domains`

### Retrieve count of domains

*Tags:* `Domains`

#### Input Parameters
* `type` - _optional_ - Type of domain ("system"/"go"/"personal"/"dedicated"). If not specified default is "system"
    Possible values: system, go, personal, dedicated.
* `name` - _optional_ - Filter domains with this anmen

### Delete a domain

*Tags:* `Domains`

#### Input Parameters
* `id` - _required_ - Id of domain

### Get a domain

*Tags:* `Domains`

#### Input Parameters
* `id` - _required_ - Id of domain

### Update a domain

*Tags:* `Domains`

#### Input Parameters
* `id` - _required_ - Id of domain

### List of all the groups associated to the user.

*Tags:* `Groups`

#### Input Parameters
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `status` - _optional_ - Status of the group
    Possible values: deleted, active.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude groups created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude groups created after this date (YYYYMMDD)
* `write` - _optional_ - Write permission

### Create a group

*Tags:* `Groups`

### Retrieve statistics about this customer for a timeframe by groups

*Tags:* `Groups`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail
* `status` - _optional_ - Status of group ("deleted"/"active")
    Possible values: deleted, active.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the group is marked as favourite

### Retrieve statistics about all groups of this customer for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `Groups`

#### Input Parameters
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of group ("deleted"/"active")
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the group is marked as favourite
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: deleted, active.

### Count the groups associated to the user.

*Tags:* `Groups`

#### Input Parameters
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude groups created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude groups created after this date (YYYYMMDD)
* `write` - _optional_ - Write permission

### Delete group specified by id

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group

### Get a group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - The id of the group

### Update a group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - The id of the group

### Retrieve statistics about this group for a timeframe

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `hourly` - _optional_ - If using "yesterday" or "today" timeframe you can ask for the hourly detail

### Retrieve statistics about this group for a timeframe grouped by some temporal entity (day/week/month)

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `groupBy` - _optional_ - The temporal entity you want to group by ("week"/"month"). If unspecified is "day".
    Possible values: week, month.

### Retrieve statistics about a subset of datapoints for a timeframe with datapoints data

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Filter by this group id
* `timeFrame` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: today, yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, last12months, lastyear, currentyear, beginning, custom.
* `type` - _optional_ - Type of datapoint ("tl"/"tp")
    Possible values: tp, tl.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `status` - _optional_ - Status of datapoint ("deleted"/"active"/"paused"/"spam")
    Possible values: deleted, active.
* `tag` - _optional_ - A comma separated list of tags you want to filter with.
* `favourite` - _optional_ - Is the datapoint marked as favourite
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `offset` - _optional_ - Offset where to start from
* `limit` - _optional_ - Limit results to this number
* `textSearch` - _optional_ - Filter fields by this pattern

### List of all the datapoints associated to the user in this group.

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Create a datapoint in this group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - The id of the group

### Count the datapoints associated to the user in this group.

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Fast switch the "favourite" field of a group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group

### Retrieve the list of events related to this group.

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, custom.
* `limit` - _optional_ - Limit results to this number
* `offset` - _optional_ - Offset where to start from (it's the lastKey field in the response object)
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `filter` - _optional_ - Filter event type ("spiders"/"uniques"/"nonuniques"/"conversions")
    Possible values: spiders, uniques, nonuniques, conversions.

### Fast patch the "notes" field of a group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group

### Retrieve a top report connected to this group

*Tags:* `Groups`

#### Input Parameters
* `id` - _required_ - Id of the group
* `type` - _required_ - Type of the report.
    Possible values: browsers, browsersfamilies, platforms, cities, countries, isps, ips, oss, ossfamilies, keywords, referrers, destinations, languages, params.
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, beginning, custom.
* `hittype` - _optional_ - Type of the event you want to filter this report with. By default no filter is applied.
    Possible values: clicks, views.
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)

### Retrieve the list of events related to this account.

*Tags:* `Hits`

#### Input Parameters
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, custom.
* `limit` - _optional_ - Limit results to this number
* `offset` - _optional_ - Offset where to start from (it's the lastKey field in the response object)
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)
* `filter` - _optional_ - Filter event type ("spiders"/"uniques"/"nonuniques"/"conversions")
    Possible values: spiders, uniques, nonuniques, conversions.

### Retrieve current account data

*Tags:* `Me`

### Retrieve current account plan

*Tags:* `Me`

### Retrieve a top report

*Tags:* `Reports`

#### Input Parameters
* `type` - _required_ - Type of the report.
    Possible values: browsers, browsersfamilies, platforms, cities, countries, isps, ips, oss, ossfamilies, keywords, referrers, destinations, languages, params.
* `timeframe` - _required_ - Timeframe of the request. See list at $timeframeList
    Possible values: yesterday, last7, last30, lastmonth, currentmonth, previousmonth, last90, last120, last180, beginning, custom.
* `hittype` - _optional_ - Type of the event you want to filter this report with. By default no filter is applied.
* `group` - _optional_ - Filter by this group id (mutually exclusive with "datapoint" and "conversion")
* `datapoint` - _optional_ - Filter by this datapoint id (mutually exclusive with "group" and "conversion")
* `conversion` - _optional_ - Filter by this conversion id (mutually exclusive with "datapoint" and "group")
* `fromDay` - _optional_ - If using a "custom" timeFrame you can specify the starting day (YYYYMMDD)
* `toDay` - _optional_ - If using a "custom" timeFrame you can specify the ending day (YYYYMMDD)

### List of all the retargeting scripts associated to the user

*Tags:* `Retargeting`

#### Input Parameters
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.

### Creates a retargeting script

*Tags:* `Retargeting`

### Retrieve count of retargeting scripts

*Tags:* `Retargeting`

### Deletes a retargeting script (and remove associations)

*Tags:* `Retargeting`

#### Input Parameters
* `id` - _required_ - The id of the retargeting script

### Get a retargeting script object

*Tags:* `Retargeting`

#### Input Parameters
* `id` - _required_ - The id of the retargeting script

### Updates a retargeting script

*Tags:* `Retargeting`

#### Input Parameters
* `id` - _required_ - The id of the retargeting script

### List of all the datapoints associated to the retargeting script.

*Tags:* `Retargeting`

#### Input Parameters
* `id` - _required_ - Id of the retargeting script
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `sortBy` - _optional_ - Field to sort by
* `sortDirection` - _optional_ - Direction of sort "asc" or "desc"
    Possible values: asc, desc.
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Count the datapoints associated to the retargeting script.

*Tags:* `Retargeting`

#### Input Parameters
* `id` - _required_ - Id of the group
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `tags` - _optional_ - A comma separated list of tags you want to filter with.
* `textSearch` - _optional_ - Filter fields by this pattern
* `onlyFavorites` - _optional_ - Filter fields by favourite status
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### List of all the groups associated to the user filtered by this tag.

*Tags:* `Tags`

#### Input Parameters
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `name` - _optional_ - Name of the tag
* `datapoints` - _optional_ - Comma separated list of datapoints id to filter by
* `groups` - _optional_ - Comma separated list of groups id to filter by
* `type` - _optional_ - Type of entity related to the tag
    Possible values: tp, tl, dp, gr.

### Create a tag

*Tags:* `Tags`

### List of all the groups associated to the user filtered by this tag.

*Tags:* `Tags`

#### Input Parameters
* `name` - _optional_ - Name of the tag
* `datapoints` - _optional_ - Comma separated list of datapoints id to filter by
* `groups` - _optional_ - Comma separated list of groups id to filter by
* `type` - _optional_ - Type of entity related to the tag
    Possible values: tp, tl, dp, gr.

### Delete a tag

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### Retrieve a tag

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### Delete the association of this tag with all datapoints

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### List of all the datapoints associated to the user filtered by this tag

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag.
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Count the datapoints associated to the user filtered by this tag

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag.
* `type` - _optional_ - Type of the datapoint ("tp"/"tl")
    Possible values: tp, tl.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active, paused, spam.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude datapoints created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude datapoints created after this date (YYYYMMDD)

### Associate/Deassociate a tag with a datapoint

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### Delete the association of this tag with all groups

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### List of all the groups associated to the user filtered by this tag.

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag.
* `offset` - _optional_ - Where to start when retrieving elements. Default is 0 if not specified.
* `limit` - _optional_ - Maximum elements to retrieve. Default to 20 if not specified.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude groups created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude groups created after this date (YYYYMMDD)

### Count the groups associated to the user filtered by this tag

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag.
* `status` - _optional_ - Status of the datapoint
    Possible values: deleted, active.
* `textSearch` - _optional_ - Filter fields by this pattern
* `createdAfter` - _optional_ - Exclude groups created before this date (YYYYMMDD)
* `createdBefore` - _optional_ - Exclude groups created after this date (YYYYMMDD)

### Associate/Deassociate a tag with a group

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

### Fast patch a tag name

*Tags:* `Tags`

#### Input Parameters
* `tagId` - _required_ - Id of the tag

## License

**flow**ground :- Telekom iPaaS / clickmeter-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.

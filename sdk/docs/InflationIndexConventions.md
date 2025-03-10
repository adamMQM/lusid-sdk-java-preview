

# InflationIndexConventions

A set of conventions that describe the conventions for an inflation index.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**inflationIndexName** | **String** | Name of the index, e.g. UKRPI. | 
**currency** | **String** | Currency of the inflation index convention. | 
**observationLag** | **String** | Observation lag. This is a string that must have units of Month.  This field is typically 3 or 4 months, but can vary, older bonds and swaps have 8 months lag.  For Bonds with a calculation type of Ratio, this property, if set, must be 0Invalid. | 
**inflationInterpolation** | **String** | Inflation Interpolation. This is optional and defaults to Linear if not set.    Supported string (enumeration) values are: [Linear, Flat]. |  [optional]
**inflationFrequency** | **String** | Frequency of inflation updated. Optional and defaults to Monthly which is the most common.  However both Australian and New Zealand inflation is published Quarterly. Only tenors of 1M or 3M are supported. |  [optional]
**inflationRollDay** | **Integer** | Day of the month that inflation rolls from one month to the next. This is optional and defaults to 1, which is  the typically value for the majority of inflation bonds (exceptions include Japan which rolls on the 10th  and some LatAm bonds which roll on the 15th). |  [optional]






# OptionalitySchedule

Optionality Schedule represents a class for creation of schedules for optionality (call, put)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**exerciseType** | **String** | The exercise type of the optionality schedule (American or European).  For American type, the bond is perpetually callable from a given exercise date until it matures, or the next date in the schedule.  For European type, the bond is only callable on a given exercise date.    Supported string (enumeration) values are: [European, American]. |  [optional]
**optionEntries** | [**List&lt;OptionEntry&gt;**](OptionEntry.md) | The dates at which the bond call/put may be actioned, and associated strikes. |  [optional]
**optionType** | **String** | Type of optionality for the schedule.    Supported string (enumeration) values are: [Call, Put]. |  [optional]




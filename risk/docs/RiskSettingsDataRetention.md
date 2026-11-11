# RiskSettingsDataRetention

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NewDeviceInDays** | **int32** | The number of days that data for the New Device predictor should be retained. Minimum is 1, maximum is 180. | 
**UserBasedRiskBehaviorInDays** | **int32** | The number of days that data for the User Based Risk Behavior predictor should be retained. Minimum is 30, maximum is 180. | 
**UserLocationAnomalyInDays** | **int32** | The number of days that data for the User Location Anomaly predictor should be retained. Minimum is 30, maximum is 90. | 

## Methods

### NewRiskSettingsDataRetention

`func NewRiskSettingsDataRetention(newDeviceInDays int32, userBasedRiskBehaviorInDays int32, userLocationAnomalyInDays int32, ) *RiskSettingsDataRetention`

NewRiskSettingsDataRetention instantiates a new RiskSettingsDataRetention object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRiskSettingsDataRetentionWithDefaults

`func NewRiskSettingsDataRetentionWithDefaults() *RiskSettingsDataRetention`

NewRiskSettingsDataRetentionWithDefaults instantiates a new RiskSettingsDataRetention object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNewDeviceInDays

`func (o *RiskSettingsDataRetention) GetNewDeviceInDays() int32`

GetNewDeviceInDays returns the NewDeviceInDays field if non-nil, zero value otherwise.

### GetNewDeviceInDaysOk

`func (o *RiskSettingsDataRetention) GetNewDeviceInDaysOk() (*int32, bool)`

GetNewDeviceInDaysOk returns a tuple with the NewDeviceInDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewDeviceInDays

`func (o *RiskSettingsDataRetention) SetNewDeviceInDays(v int32)`

SetNewDeviceInDays sets NewDeviceInDays field to given value.


### GetUserBasedRiskBehaviorInDays

`func (o *RiskSettingsDataRetention) GetUserBasedRiskBehaviorInDays() int32`

GetUserBasedRiskBehaviorInDays returns the UserBasedRiskBehaviorInDays field if non-nil, zero value otherwise.

### GetUserBasedRiskBehaviorInDaysOk

`func (o *RiskSettingsDataRetention) GetUserBasedRiskBehaviorInDaysOk() (*int32, bool)`

GetUserBasedRiskBehaviorInDaysOk returns a tuple with the UserBasedRiskBehaviorInDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserBasedRiskBehaviorInDays

`func (o *RiskSettingsDataRetention) SetUserBasedRiskBehaviorInDays(v int32)`

SetUserBasedRiskBehaviorInDays sets UserBasedRiskBehaviorInDays field to given value.


### GetUserLocationAnomalyInDays

`func (o *RiskSettingsDataRetention) GetUserLocationAnomalyInDays() int32`

GetUserLocationAnomalyInDays returns the UserLocationAnomalyInDays field if non-nil, zero value otherwise.

### GetUserLocationAnomalyInDaysOk

`func (o *RiskSettingsDataRetention) GetUserLocationAnomalyInDaysOk() (*int32, bool)`

GetUserLocationAnomalyInDaysOk returns a tuple with the UserLocationAnomalyInDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserLocationAnomalyInDays

`func (o *RiskSettingsDataRetention) SetUserLocationAnomalyInDays(v int32)`

SetUserLocationAnomalyInDays sets UserLocationAnomalyInDays field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



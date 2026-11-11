# RiskSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Links** | Pointer to [**map[string]LinksHATEOASValue**](LinksHATEOASValue.md) |  | [optional] [readonly] 
**DataRetention** | Pointer to [**RiskSettingsDataRetention**](RiskSettingsDataRetention.md) |  | [optional] 
**Environment** | Pointer to [**ObjectEnvironment**](ObjectEnvironment.md) |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** | The date and time the Protect settings were last updated (format ISO-8061). | [optional] [readonly] 

## Methods

### NewRiskSettings

`func NewRiskSettings() *RiskSettings`

NewRiskSettings instantiates a new RiskSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRiskSettingsWithDefaults

`func NewRiskSettingsWithDefaults() *RiskSettings`

NewRiskSettingsWithDefaults instantiates a new RiskSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLinks

`func (o *RiskSettings) GetLinks() map[string]LinksHATEOASValue`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *RiskSettings) GetLinksOk() (*map[string]LinksHATEOASValue, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *RiskSettings) SetLinks(v map[string]LinksHATEOASValue)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *RiskSettings) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### GetDataRetention

`func (o *RiskSettings) GetDataRetention() RiskSettingsDataRetention`

GetDataRetention returns the DataRetention field if non-nil, zero value otherwise.

### GetDataRetentionOk

`func (o *RiskSettings) GetDataRetentionOk() (*RiskSettingsDataRetention, bool)`

GetDataRetentionOk returns a tuple with the DataRetention field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataRetention

`func (o *RiskSettings) SetDataRetention(v RiskSettingsDataRetention)`

SetDataRetention sets DataRetention field to given value.

### HasDataRetention

`func (o *RiskSettings) HasDataRetention() bool`

HasDataRetention returns a boolean if a field has been set.

### GetEnvironment

`func (o *RiskSettings) GetEnvironment() ObjectEnvironment`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *RiskSettings) GetEnvironmentOk() (*ObjectEnvironment, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *RiskSettings) SetEnvironment(v ObjectEnvironment)`

SetEnvironment sets Environment field to given value.

### HasEnvironment

`func (o *RiskSettings) HasEnvironment() bool`

HasEnvironment returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *RiskSettings) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *RiskSettings) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *RiskSettings) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *RiskSettings) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



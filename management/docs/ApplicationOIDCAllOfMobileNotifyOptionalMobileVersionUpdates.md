# ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Set &#x60;notifyOptionalMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60; if you want to notify your users that there is a newer version of the PingID app available if they want to update. The notification is displayed as soon as the user opens the app. When set to &#x60;true&#x60;, you must provide a value for &#x60;notifyOptionalMobileVersionUpdates.android&#x60;, &#x60;notifyOptionalMobileVersionUpdates.ios&#x60;, or both. | [optional] 
**Android** | Pointer to **string** | If you set &#x60;notifyOptionalMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60;, use &#x60;android&#x60; to specify the version of the app that you want to notify Android device users about. Set the value to &#x60;latest&#x60; if you want to always notify users about the latest version of the PingID app that is available. | [optional] 
**Ios** | Pointer to **string** | If you set &#x60;notifyOptionalMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60;, use &#x60;ios&#x60; to specify the version of the app that you want to notify iOS device users about. Set the value to &#x60;latest&#x60; if you want to always notify users about the latest version of the PingID app that is available. | [optional] 

## Methods

### NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates

`func NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates() *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates`

NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates instantiates a new ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdatesWithDefaults

`func NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdatesWithDefaults() *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates`

NewApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdatesWithDefaults instantiates a new ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetAndroid() string`

GetAndroid returns the Android field if non-nil, zero value otherwise.

### GetAndroidOk

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetAndroidOk() (*string, bool)`

GetAndroidOk returns a tuple with the Android field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) SetAndroid(v string)`

SetAndroid sets Android field to given value.

### HasAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) HasAndroid() bool`

HasAndroid returns a boolean if a field has been set.

### GetIos

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetIos() string`

GetIos returns the Ios field if non-nil, zero value otherwise.

### GetIosOk

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) GetIosOk() (*string, bool)`

GetIosOk returns a tuple with the Ios field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIos

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) SetIos(v string)`

SetIos sets Ios field to given value.

### HasIos

`func (o *ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates) HasIos() bool`

HasIos returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Set &#x60;notifyRequireMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60; if you want to require a minimum version of the PingID app and notify the user that they must update the app if they are using an older version. The notification is displayed as soon as the user opens the app. When set to &#x60;true&#x60;, you must provide a value for &#x60;notifyRequireMobileVersionUpdates.android&#x60;, &#x60;notifyRequireMobileVersionUpdates.ios&#x60;, or both. | [optional] 
**Android** | Pointer to **string** | If you set &#x60;notifyRequireMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60;, use &#x60;android&#x60; to specify the minimum version of the app that you want to require on Android devices. Set the value to &#x60;latest&#x60; if you want to require your users to always be running the latest version of the PingID app. | [optional] 
**Ios** | Pointer to **string** | If you set &#x60;notifyRequireMobileVersionUpdates.enabled&#x60; to &#x60;true&#x60;, use &#x60;ios&#x60; to specify the minimum version of the app that you want to require on iOS devices. Set the value to &#x60;latest&#x60; if you want to require your users to always be running the latest version of the PingID app. | [optional] 

## Methods

### NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates

`func NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates() *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates`

NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates instantiates a new ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdatesWithDefaults

`func NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdatesWithDefaults() *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates`

NewApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdatesWithDefaults instantiates a new ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetAndroid() string`

GetAndroid returns the Android field if non-nil, zero value otherwise.

### GetAndroidOk

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetAndroidOk() (*string, bool)`

GetAndroidOk returns a tuple with the Android field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) SetAndroid(v string)`

SetAndroid sets Android field to given value.

### HasAndroid

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) HasAndroid() bool`

HasAndroid returns a boolean if a field has been set.

### GetIos

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetIos() string`

GetIos returns the Ios field if non-nil, zero value otherwise.

### GetIosOk

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) GetIosOk() (*string, bool)`

GetIosOk returns a tuple with the Ios field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIos

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) SetIos(v string)`

SetIos sets Ios field to given value.

### HasIos

`func (o *ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates) HasIos() bool`

HasIos returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



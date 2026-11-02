# ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Set to &#x60;true&#x60; if you want to require the user to enter a security PIN to access the PingID mobile app. | [optional] 
**RequireForAllDevices** | Pointer to **bool** | If &#x60;mobile.mobileAppSecurityPinRequire.enabled&#x60; is set to &#x60;true&#x60;, then by default, the PIN is required only if a device PIN or biometrics have not been defined for the device. Set &#x60;requireForAllDevices&#x60; to &#x60;true&#x60; if you want to require PIN use for all devices. | [optional] 
**SecurityPinDigit** | Pointer to [**EnumMobileAppSecurityPinDigit**](EnumMobileAppSecurityPinDigit.md) |  | [optional] 

## Methods

### NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequire

`func NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequire() *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire`

NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequire instantiates a new ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequireWithDefaults

`func NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequireWithDefaults() *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire`

NewApplicationOIDCAllOfMobileMobileAppSecurityPinRequireWithDefaults instantiates a new ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetRequireForAllDevices

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetRequireForAllDevices() bool`

GetRequireForAllDevices returns the RequireForAllDevices field if non-nil, zero value otherwise.

### GetRequireForAllDevicesOk

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetRequireForAllDevicesOk() (*bool, bool)`

GetRequireForAllDevicesOk returns a tuple with the RequireForAllDevices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequireForAllDevices

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) SetRequireForAllDevices(v bool)`

SetRequireForAllDevices sets RequireForAllDevices field to given value.

### HasRequireForAllDevices

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) HasRequireForAllDevices() bool`

HasRequireForAllDevices returns a boolean if a field has been set.

### GetSecurityPinDigit

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetSecurityPinDigit() EnumMobileAppSecurityPinDigit`

GetSecurityPinDigit returns the SecurityPinDigit field if non-nil, zero value otherwise.

### GetSecurityPinDigitOk

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) GetSecurityPinDigitOk() (*EnumMobileAppSecurityPinDigit, bool)`

GetSecurityPinDigitOk returns a tuple with the SecurityPinDigit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecurityPinDigit

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) SetSecurityPinDigit(v EnumMobileAppSecurityPinDigit)`

SetSecurityPinDigit sets SecurityPinDigit field to given value.

### HasSecurityPinDigit

`func (o *ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire) HasSecurityPinDigit() bool`

HasSecurityPinDigit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



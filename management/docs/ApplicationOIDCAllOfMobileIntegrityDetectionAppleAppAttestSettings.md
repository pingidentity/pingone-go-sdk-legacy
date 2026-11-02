# ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Set the value of &#x60;appleAppAttestSettings.enabled&#x60; to &#x60;true&#x60; if you have enabled device integrity checking for your iOS app and you want to use Apple App Attest for the check. If the value is set to &#x60;true&#x60;, you must also include a value for &#x60;mobile.appleTeamId&#x60;. | [optional] 

## Methods

### NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings

`func NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings() *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings`

NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings instantiates a new ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettingsWithDefaults

`func NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettingsWithDefaults() *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings`

NewApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettingsWithDefaults instantiates a new ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *ApplicationOIDCAllOfMobileIntegrityDetectionAppleAppAttestSettings) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



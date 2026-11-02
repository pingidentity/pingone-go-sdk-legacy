# ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Required** | Pointer to **bool** | If you have allowed biometric authentication methods in the MFA policy, then by default, the user is required to use a biometric method with PingID if one is available on their device. If you want to specify that users can authenticate with the PingID mobile app only if they have a biometric method configured, set &#x60;mobile.mobileDeviceBiometricsSetting.required&#x60; to &#x60;true&#x60;. | [optional] 
**DevicePasscodeFallbackEnabled** | Pointer to **bool** | Set &#x60;devicePasscodeFallbackEnabled&#x60; to &#x60;true&#x60; if you want to allow iOS users to authenticate using the device passcode if biometric authentication fails. | [optional] 
**FaceIdConsentEnabled** | Pointer to **bool** | For iOS devices, set &#x60;faceIdConsentEnabled&#x60; to &#x60;true&#x60; if you want to prevent users with FaceID defined from authenticating by mistake. When set to &#x60;true&#x60;, the user is prompted to consent explicitly before each face scan is taken. | [optional] 
**NotificationActionsEnabled** | Pointer to **bool** | Set &#x60;notificationActionsEnabled&#x60; to &#x60;true&#x60; if you want to allow users to approve notification requests from their device&#39;s lock screen. | [optional] 

## Methods

### NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting

`func NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting() *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting`

NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting instantiates a new ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSettingWithDefaults

`func NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSettingWithDefaults() *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting`

NewApplicationOIDCAllOfMobileMobileDeviceBiometricsSettingWithDefaults instantiates a new ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRequired

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetDevicePasscodeFallbackEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetDevicePasscodeFallbackEnabled() bool`

GetDevicePasscodeFallbackEnabled returns the DevicePasscodeFallbackEnabled field if non-nil, zero value otherwise.

### GetDevicePasscodeFallbackEnabledOk

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetDevicePasscodeFallbackEnabledOk() (*bool, bool)`

GetDevicePasscodeFallbackEnabledOk returns a tuple with the DevicePasscodeFallbackEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDevicePasscodeFallbackEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) SetDevicePasscodeFallbackEnabled(v bool)`

SetDevicePasscodeFallbackEnabled sets DevicePasscodeFallbackEnabled field to given value.

### HasDevicePasscodeFallbackEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) HasDevicePasscodeFallbackEnabled() bool`

HasDevicePasscodeFallbackEnabled returns a boolean if a field has been set.

### GetFaceIdConsentEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetFaceIdConsentEnabled() bool`

GetFaceIdConsentEnabled returns the FaceIdConsentEnabled field if non-nil, zero value otherwise.

### GetFaceIdConsentEnabledOk

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetFaceIdConsentEnabledOk() (*bool, bool)`

GetFaceIdConsentEnabledOk returns a tuple with the FaceIdConsentEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaceIdConsentEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) SetFaceIdConsentEnabled(v bool)`

SetFaceIdConsentEnabled sets FaceIdConsentEnabled field to given value.

### HasFaceIdConsentEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) HasFaceIdConsentEnabled() bool`

HasFaceIdConsentEnabled returns a boolean if a field has been set.

### GetNotificationActionsEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetNotificationActionsEnabled() bool`

GetNotificationActionsEnabled returns the NotificationActionsEnabled field if non-nil, zero value otherwise.

### GetNotificationActionsEnabledOk

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) GetNotificationActionsEnabledOk() (*bool, bool)`

GetNotificationActionsEnabledOk returns a tuple with the NotificationActionsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotificationActionsEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) SetNotificationActionsEnabled(v bool)`

SetNotificationActionsEnabled sets NotificationActionsEnabled field to given value.

### HasNotificationActionsEnabled

`func (o *ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting) HasNotificationActionsEnabled() bool`

HasNotificationActionsEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ApplicationOIDCAllOfMobile

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AppleTeamId** | Pointer to **string** | If you set &#x60;mobile.integrityDetection.appleAppAttestSettings.enabled&#x60; to &#x60;true&#x60; to use Apple App Attest for device integrity checking, you must also set &#x60;mobile.appleTeamId&#x60; to the Team ID from your Apple Developer account. | [optional] 
**BundleId** | Pointer to **string** | A string that specifies the bundle associated with the application, for push notifications in native apps. The value of the bundleId property is unique per environment, and once defined, is immutable.  this setting overrides the top-level bundleId field | [optional] 
**PackageName** | Pointer to **string** | A string that specifies the package name associated with the application, for push notifications in native apps. The value of the mobile.packageName property is unique per environment, and once defined, is immutable.  this setting overrides the top-level packageName field. | [optional] 
**HuaweiAppId** | Pointer to **string** | The unique identifier for the app on the device and in the Huawei Mobile Service AppGallery. The value of the &#x60;huaweiAppId&#x60; property is unique per environment, and once defined, is immutable. Used only for applications for the Huawei ecosystem. | [optional] 
**HuaweiPackageName** | Pointer to **string** | The package name associated with the application, for push notifications in native apps. The value of the &#x60;huaweiPackageName&#x60; property is unique per environment, and once defined, is immutable. Used only for applications for the Huawei ecosystem. | [optional] 
**PasscodeGracePeriod** | Pointer to **int32** | To cover time synchronization issues, you can use this field to customize the grace period during which the passcode can still be used even after the passcode has been refreshed. The value of the parameter should be the number of windows to use (min 1, max 10). In this context, a window is equal to the passcode refresh period in either direction. For example, if you defined a passcode refresh duration of 30 seconds and a grace period of 2 windows, the passcode is valid for 150 seconds (from 60 seconds behind the time of issue until 60 seconds past the expiration time). When this field is not included, the default value used is 5 windows. | [optional] 
**PasscodeRefreshDuration** | Pointer to [**ApplicationOIDCAllOfMobilePasscodeRefreshDuration**](ApplicationOIDCAllOfMobilePasscodeRefreshDuration.md) |  | [optional] 
**IntegrityDetection** | Pointer to [**ApplicationOIDCAllOfMobileIntegrityDetection**](ApplicationOIDCAllOfMobileIntegrityDetection.md) |  | [optional] 
**Push** | Pointer to [**ApplicationOIDCAllOfMobilePush**](ApplicationOIDCAllOfMobilePush.md) |  | [optional] 
**UriPrefix** | Pointer to **string** | A string that specifies a URI prefix that enables direct triggering of the mobile application when scanning a QR code. The URI prefix can be set to a universal link with a valid value (which can be a URL address that starts with &#x60;HTTP://&#x60; or &#x60;HTTPS://&#x60;, such as &#x60;https://www.acme.com&#x60;), or an app schema, which is just a string and requires no special validation. | [optional] 
**PingIDSettings** | Pointer to **bool** | Must be set to &#x60;true&#x60;. | [optional] 
**AllowAuthenticationDeviceLocked** | Pointer to [**ApplicationOIDCAllOfMobileAllowAuthenticationDeviceLocked**](ApplicationOIDCAllOfMobileAllowAuthenticationDeviceLocked.md) |  | [optional] 
**AllowUnPairAndChangeDeviceFromApp** | Pointer to [**ApplicationOIDCAllOfMobileAllowUnPairAndChangeDeviceFromApp**](ApplicationOIDCAllOfMobileAllowUnPairAndChangeDeviceFromApp.md) |  | [optional] 
**MobileAppSecurityPinRequire** | Pointer to [**ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire**](ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire.md) |  | [optional] 
**MobileDeviceBiometricsSetting** | Pointer to [**ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting**](ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting.md) |  | [optional] 
**NotifyOptionalMobileVersionUpdates** | Pointer to [**ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates**](ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates.md) |  | [optional] 
**NotifyRequireMobileVersionUpdates** | Pointer to [**ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates**](ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates.md) |  | [optional] 
**OtpPushNotificationEnabled** | Pointer to [**ApplicationOIDCAllOfMobileOtpPushNotificationEnabled**](ApplicationOIDCAllOfMobileOtpPushNotificationEnabled.md) |  | [optional] 
**ShowAuthenticationInformation** | Pointer to [**ApplicationOIDCAllOfMobileShowAuthenticationInformation**](ApplicationOIDCAllOfMobileShowAuthenticationInformation.md) |  | [optional] 

## Methods

### NewApplicationOIDCAllOfMobile

`func NewApplicationOIDCAllOfMobile() *ApplicationOIDCAllOfMobile`

NewApplicationOIDCAllOfMobile instantiates a new ApplicationOIDCAllOfMobile object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationOIDCAllOfMobileWithDefaults

`func NewApplicationOIDCAllOfMobileWithDefaults() *ApplicationOIDCAllOfMobile`

NewApplicationOIDCAllOfMobileWithDefaults instantiates a new ApplicationOIDCAllOfMobile object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAppleTeamId

`func (o *ApplicationOIDCAllOfMobile) GetAppleTeamId() string`

GetAppleTeamId returns the AppleTeamId field if non-nil, zero value otherwise.

### GetAppleTeamIdOk

`func (o *ApplicationOIDCAllOfMobile) GetAppleTeamIdOk() (*string, bool)`

GetAppleTeamIdOk returns a tuple with the AppleTeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAppleTeamId

`func (o *ApplicationOIDCAllOfMobile) SetAppleTeamId(v string)`

SetAppleTeamId sets AppleTeamId field to given value.

### HasAppleTeamId

`func (o *ApplicationOIDCAllOfMobile) HasAppleTeamId() bool`

HasAppleTeamId returns a boolean if a field has been set.

### GetBundleId

`func (o *ApplicationOIDCAllOfMobile) GetBundleId() string`

GetBundleId returns the BundleId field if non-nil, zero value otherwise.

### GetBundleIdOk

`func (o *ApplicationOIDCAllOfMobile) GetBundleIdOk() (*string, bool)`

GetBundleIdOk returns a tuple with the BundleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBundleId

`func (o *ApplicationOIDCAllOfMobile) SetBundleId(v string)`

SetBundleId sets BundleId field to given value.

### HasBundleId

`func (o *ApplicationOIDCAllOfMobile) HasBundleId() bool`

HasBundleId returns a boolean if a field has been set.

### GetPackageName

`func (o *ApplicationOIDCAllOfMobile) GetPackageName() string`

GetPackageName returns the PackageName field if non-nil, zero value otherwise.

### GetPackageNameOk

`func (o *ApplicationOIDCAllOfMobile) GetPackageNameOk() (*string, bool)`

GetPackageNameOk returns a tuple with the PackageName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackageName

`func (o *ApplicationOIDCAllOfMobile) SetPackageName(v string)`

SetPackageName sets PackageName field to given value.

### HasPackageName

`func (o *ApplicationOIDCAllOfMobile) HasPackageName() bool`

HasPackageName returns a boolean if a field has been set.

### GetHuaweiAppId

`func (o *ApplicationOIDCAllOfMobile) GetHuaweiAppId() string`

GetHuaweiAppId returns the HuaweiAppId field if non-nil, zero value otherwise.

### GetHuaweiAppIdOk

`func (o *ApplicationOIDCAllOfMobile) GetHuaweiAppIdOk() (*string, bool)`

GetHuaweiAppIdOk returns a tuple with the HuaweiAppId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHuaweiAppId

`func (o *ApplicationOIDCAllOfMobile) SetHuaweiAppId(v string)`

SetHuaweiAppId sets HuaweiAppId field to given value.

### HasHuaweiAppId

`func (o *ApplicationOIDCAllOfMobile) HasHuaweiAppId() bool`

HasHuaweiAppId returns a boolean if a field has been set.

### GetHuaweiPackageName

`func (o *ApplicationOIDCAllOfMobile) GetHuaweiPackageName() string`

GetHuaweiPackageName returns the HuaweiPackageName field if non-nil, zero value otherwise.

### GetHuaweiPackageNameOk

`func (o *ApplicationOIDCAllOfMobile) GetHuaweiPackageNameOk() (*string, bool)`

GetHuaweiPackageNameOk returns a tuple with the HuaweiPackageName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHuaweiPackageName

`func (o *ApplicationOIDCAllOfMobile) SetHuaweiPackageName(v string)`

SetHuaweiPackageName sets HuaweiPackageName field to given value.

### HasHuaweiPackageName

`func (o *ApplicationOIDCAllOfMobile) HasHuaweiPackageName() bool`

HasHuaweiPackageName returns a boolean if a field has been set.

### GetPasscodeGracePeriod

`func (o *ApplicationOIDCAllOfMobile) GetPasscodeGracePeriod() int32`

GetPasscodeGracePeriod returns the PasscodeGracePeriod field if non-nil, zero value otherwise.

### GetPasscodeGracePeriodOk

`func (o *ApplicationOIDCAllOfMobile) GetPasscodeGracePeriodOk() (*int32, bool)`

GetPasscodeGracePeriodOk returns a tuple with the PasscodeGracePeriod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasscodeGracePeriod

`func (o *ApplicationOIDCAllOfMobile) SetPasscodeGracePeriod(v int32)`

SetPasscodeGracePeriod sets PasscodeGracePeriod field to given value.

### HasPasscodeGracePeriod

`func (o *ApplicationOIDCAllOfMobile) HasPasscodeGracePeriod() bool`

HasPasscodeGracePeriod returns a boolean if a field has been set.

### GetPasscodeRefreshDuration

`func (o *ApplicationOIDCAllOfMobile) GetPasscodeRefreshDuration() ApplicationOIDCAllOfMobilePasscodeRefreshDuration`

GetPasscodeRefreshDuration returns the PasscodeRefreshDuration field if non-nil, zero value otherwise.

### GetPasscodeRefreshDurationOk

`func (o *ApplicationOIDCAllOfMobile) GetPasscodeRefreshDurationOk() (*ApplicationOIDCAllOfMobilePasscodeRefreshDuration, bool)`

GetPasscodeRefreshDurationOk returns a tuple with the PasscodeRefreshDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasscodeRefreshDuration

`func (o *ApplicationOIDCAllOfMobile) SetPasscodeRefreshDuration(v ApplicationOIDCAllOfMobilePasscodeRefreshDuration)`

SetPasscodeRefreshDuration sets PasscodeRefreshDuration field to given value.

### HasPasscodeRefreshDuration

`func (o *ApplicationOIDCAllOfMobile) HasPasscodeRefreshDuration() bool`

HasPasscodeRefreshDuration returns a boolean if a field has been set.

### GetIntegrityDetection

`func (o *ApplicationOIDCAllOfMobile) GetIntegrityDetection() ApplicationOIDCAllOfMobileIntegrityDetection`

GetIntegrityDetection returns the IntegrityDetection field if non-nil, zero value otherwise.

### GetIntegrityDetectionOk

`func (o *ApplicationOIDCAllOfMobile) GetIntegrityDetectionOk() (*ApplicationOIDCAllOfMobileIntegrityDetection, bool)`

GetIntegrityDetectionOk returns a tuple with the IntegrityDetection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegrityDetection

`func (o *ApplicationOIDCAllOfMobile) SetIntegrityDetection(v ApplicationOIDCAllOfMobileIntegrityDetection)`

SetIntegrityDetection sets IntegrityDetection field to given value.

### HasIntegrityDetection

`func (o *ApplicationOIDCAllOfMobile) HasIntegrityDetection() bool`

HasIntegrityDetection returns a boolean if a field has been set.

### GetPush

`func (o *ApplicationOIDCAllOfMobile) GetPush() ApplicationOIDCAllOfMobilePush`

GetPush returns the Push field if non-nil, zero value otherwise.

### GetPushOk

`func (o *ApplicationOIDCAllOfMobile) GetPushOk() (*ApplicationOIDCAllOfMobilePush, bool)`

GetPushOk returns a tuple with the Push field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPush

`func (o *ApplicationOIDCAllOfMobile) SetPush(v ApplicationOIDCAllOfMobilePush)`

SetPush sets Push field to given value.

### HasPush

`func (o *ApplicationOIDCAllOfMobile) HasPush() bool`

HasPush returns a boolean if a field has been set.

### GetUriPrefix

`func (o *ApplicationOIDCAllOfMobile) GetUriPrefix() string`

GetUriPrefix returns the UriPrefix field if non-nil, zero value otherwise.

### GetUriPrefixOk

`func (o *ApplicationOIDCAllOfMobile) GetUriPrefixOk() (*string, bool)`

GetUriPrefixOk returns a tuple with the UriPrefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUriPrefix

`func (o *ApplicationOIDCAllOfMobile) SetUriPrefix(v string)`

SetUriPrefix sets UriPrefix field to given value.

### HasUriPrefix

`func (o *ApplicationOIDCAllOfMobile) HasUriPrefix() bool`

HasUriPrefix returns a boolean if a field has been set.

### GetPingIDSettings

`func (o *ApplicationOIDCAllOfMobile) GetPingIDSettings() bool`

GetPingIDSettings returns the PingIDSettings field if non-nil, zero value otherwise.

### GetPingIDSettingsOk

`func (o *ApplicationOIDCAllOfMobile) GetPingIDSettingsOk() (*bool, bool)`

GetPingIDSettingsOk returns a tuple with the PingIDSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPingIDSettings

`func (o *ApplicationOIDCAllOfMobile) SetPingIDSettings(v bool)`

SetPingIDSettings sets PingIDSettings field to given value.

### HasPingIDSettings

`func (o *ApplicationOIDCAllOfMobile) HasPingIDSettings() bool`

HasPingIDSettings returns a boolean if a field has been set.

### GetAllowAuthenticationDeviceLocked

`func (o *ApplicationOIDCAllOfMobile) GetAllowAuthenticationDeviceLocked() ApplicationOIDCAllOfMobileAllowAuthenticationDeviceLocked`

GetAllowAuthenticationDeviceLocked returns the AllowAuthenticationDeviceLocked field if non-nil, zero value otherwise.

### GetAllowAuthenticationDeviceLockedOk

`func (o *ApplicationOIDCAllOfMobile) GetAllowAuthenticationDeviceLockedOk() (*ApplicationOIDCAllOfMobileAllowAuthenticationDeviceLocked, bool)`

GetAllowAuthenticationDeviceLockedOk returns a tuple with the AllowAuthenticationDeviceLocked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowAuthenticationDeviceLocked

`func (o *ApplicationOIDCAllOfMobile) SetAllowAuthenticationDeviceLocked(v ApplicationOIDCAllOfMobileAllowAuthenticationDeviceLocked)`

SetAllowAuthenticationDeviceLocked sets AllowAuthenticationDeviceLocked field to given value.

### HasAllowAuthenticationDeviceLocked

`func (o *ApplicationOIDCAllOfMobile) HasAllowAuthenticationDeviceLocked() bool`

HasAllowAuthenticationDeviceLocked returns a boolean if a field has been set.

### GetAllowUnPairAndChangeDeviceFromApp

`func (o *ApplicationOIDCAllOfMobile) GetAllowUnPairAndChangeDeviceFromApp() ApplicationOIDCAllOfMobileAllowUnPairAndChangeDeviceFromApp`

GetAllowUnPairAndChangeDeviceFromApp returns the AllowUnPairAndChangeDeviceFromApp field if non-nil, zero value otherwise.

### GetAllowUnPairAndChangeDeviceFromAppOk

`func (o *ApplicationOIDCAllOfMobile) GetAllowUnPairAndChangeDeviceFromAppOk() (*ApplicationOIDCAllOfMobileAllowUnPairAndChangeDeviceFromApp, bool)`

GetAllowUnPairAndChangeDeviceFromAppOk returns a tuple with the AllowUnPairAndChangeDeviceFromApp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowUnPairAndChangeDeviceFromApp

`func (o *ApplicationOIDCAllOfMobile) SetAllowUnPairAndChangeDeviceFromApp(v ApplicationOIDCAllOfMobileAllowUnPairAndChangeDeviceFromApp)`

SetAllowUnPairAndChangeDeviceFromApp sets AllowUnPairAndChangeDeviceFromApp field to given value.

### HasAllowUnPairAndChangeDeviceFromApp

`func (o *ApplicationOIDCAllOfMobile) HasAllowUnPairAndChangeDeviceFromApp() bool`

HasAllowUnPairAndChangeDeviceFromApp returns a boolean if a field has been set.

### GetMobileAppSecurityPinRequire

`func (o *ApplicationOIDCAllOfMobile) GetMobileAppSecurityPinRequire() ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire`

GetMobileAppSecurityPinRequire returns the MobileAppSecurityPinRequire field if non-nil, zero value otherwise.

### GetMobileAppSecurityPinRequireOk

`func (o *ApplicationOIDCAllOfMobile) GetMobileAppSecurityPinRequireOk() (*ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire, bool)`

GetMobileAppSecurityPinRequireOk returns a tuple with the MobileAppSecurityPinRequire field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMobileAppSecurityPinRequire

`func (o *ApplicationOIDCAllOfMobile) SetMobileAppSecurityPinRequire(v ApplicationOIDCAllOfMobileMobileAppSecurityPinRequire)`

SetMobileAppSecurityPinRequire sets MobileAppSecurityPinRequire field to given value.

### HasMobileAppSecurityPinRequire

`func (o *ApplicationOIDCAllOfMobile) HasMobileAppSecurityPinRequire() bool`

HasMobileAppSecurityPinRequire returns a boolean if a field has been set.

### GetMobileDeviceBiometricsSetting

`func (o *ApplicationOIDCAllOfMobile) GetMobileDeviceBiometricsSetting() ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting`

GetMobileDeviceBiometricsSetting returns the MobileDeviceBiometricsSetting field if non-nil, zero value otherwise.

### GetMobileDeviceBiometricsSettingOk

`func (o *ApplicationOIDCAllOfMobile) GetMobileDeviceBiometricsSettingOk() (*ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting, bool)`

GetMobileDeviceBiometricsSettingOk returns a tuple with the MobileDeviceBiometricsSetting field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMobileDeviceBiometricsSetting

`func (o *ApplicationOIDCAllOfMobile) SetMobileDeviceBiometricsSetting(v ApplicationOIDCAllOfMobileMobileDeviceBiometricsSetting)`

SetMobileDeviceBiometricsSetting sets MobileDeviceBiometricsSetting field to given value.

### HasMobileDeviceBiometricsSetting

`func (o *ApplicationOIDCAllOfMobile) HasMobileDeviceBiometricsSetting() bool`

HasMobileDeviceBiometricsSetting returns a boolean if a field has been set.

### GetNotifyOptionalMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) GetNotifyOptionalMobileVersionUpdates() ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates`

GetNotifyOptionalMobileVersionUpdates returns the NotifyOptionalMobileVersionUpdates field if non-nil, zero value otherwise.

### GetNotifyOptionalMobileVersionUpdatesOk

`func (o *ApplicationOIDCAllOfMobile) GetNotifyOptionalMobileVersionUpdatesOk() (*ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates, bool)`

GetNotifyOptionalMobileVersionUpdatesOk returns a tuple with the NotifyOptionalMobileVersionUpdates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotifyOptionalMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) SetNotifyOptionalMobileVersionUpdates(v ApplicationOIDCAllOfMobileNotifyOptionalMobileVersionUpdates)`

SetNotifyOptionalMobileVersionUpdates sets NotifyOptionalMobileVersionUpdates field to given value.

### HasNotifyOptionalMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) HasNotifyOptionalMobileVersionUpdates() bool`

HasNotifyOptionalMobileVersionUpdates returns a boolean if a field has been set.

### GetNotifyRequireMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) GetNotifyRequireMobileVersionUpdates() ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates`

GetNotifyRequireMobileVersionUpdates returns the NotifyRequireMobileVersionUpdates field if non-nil, zero value otherwise.

### GetNotifyRequireMobileVersionUpdatesOk

`func (o *ApplicationOIDCAllOfMobile) GetNotifyRequireMobileVersionUpdatesOk() (*ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates, bool)`

GetNotifyRequireMobileVersionUpdatesOk returns a tuple with the NotifyRequireMobileVersionUpdates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotifyRequireMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) SetNotifyRequireMobileVersionUpdates(v ApplicationOIDCAllOfMobileNotifyRequireMobileVersionUpdates)`

SetNotifyRequireMobileVersionUpdates sets NotifyRequireMobileVersionUpdates field to given value.

### HasNotifyRequireMobileVersionUpdates

`func (o *ApplicationOIDCAllOfMobile) HasNotifyRequireMobileVersionUpdates() bool`

HasNotifyRequireMobileVersionUpdates returns a boolean if a field has been set.

### GetOtpPushNotificationEnabled

`func (o *ApplicationOIDCAllOfMobile) GetOtpPushNotificationEnabled() ApplicationOIDCAllOfMobileOtpPushNotificationEnabled`

GetOtpPushNotificationEnabled returns the OtpPushNotificationEnabled field if non-nil, zero value otherwise.

### GetOtpPushNotificationEnabledOk

`func (o *ApplicationOIDCAllOfMobile) GetOtpPushNotificationEnabledOk() (*ApplicationOIDCAllOfMobileOtpPushNotificationEnabled, bool)`

GetOtpPushNotificationEnabledOk returns a tuple with the OtpPushNotificationEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOtpPushNotificationEnabled

`func (o *ApplicationOIDCAllOfMobile) SetOtpPushNotificationEnabled(v ApplicationOIDCAllOfMobileOtpPushNotificationEnabled)`

SetOtpPushNotificationEnabled sets OtpPushNotificationEnabled field to given value.

### HasOtpPushNotificationEnabled

`func (o *ApplicationOIDCAllOfMobile) HasOtpPushNotificationEnabled() bool`

HasOtpPushNotificationEnabled returns a boolean if a field has been set.

### GetShowAuthenticationInformation

`func (o *ApplicationOIDCAllOfMobile) GetShowAuthenticationInformation() ApplicationOIDCAllOfMobileShowAuthenticationInformation`

GetShowAuthenticationInformation returns the ShowAuthenticationInformation field if non-nil, zero value otherwise.

### GetShowAuthenticationInformationOk

`func (o *ApplicationOIDCAllOfMobile) GetShowAuthenticationInformationOk() (*ApplicationOIDCAllOfMobileShowAuthenticationInformation, bool)`

GetShowAuthenticationInformationOk returns a tuple with the ShowAuthenticationInformation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShowAuthenticationInformation

`func (o *ApplicationOIDCAllOfMobile) SetShowAuthenticationInformation(v ApplicationOIDCAllOfMobileShowAuthenticationInformation)`

SetShowAuthenticationInformation sets ShowAuthenticationInformation field to given value.

### HasShowAuthenticationInformation

`func (o *ApplicationOIDCAllOfMobile) HasShowAuthenticationInformation() bool`

HasShowAuthenticationInformation returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



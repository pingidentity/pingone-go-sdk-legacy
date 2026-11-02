# ApplicationWSFED

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Links** | Pointer to [**map[string]LinksHATEOASValue**](LinksHATEOASValue.md) |  | [optional] [readonly] 
**AccessControl** | Pointer to [**ApplicationAccessControl**](ApplicationAccessControl.md) |  | [optional] 
**CreatedAt** | Pointer to **time.Time** | The time the resource was created. | [optional] [readonly] 
**Description** | Pointer to **string** | A string that specifies the description of the application. | [optional] 
**Enabled** | **bool** | A string that specifies the current enabled state of the application. Options are ENABLED or DISABLED. | 
**Environment** | Pointer to [**ObjectEnvironment**](ObjectEnvironment.md) |  | [optional] 
**HiddenFromAppPortal** | Pointer to **bool** | A boolean to specify whether the application is hidden in the application portal despite the configured group access policy. | [optional] 
**Icon** | Pointer to [**ApplicationIcon**](ApplicationIcon.md) |  | [optional] 
**Id** | Pointer to **string** | A string that specifies the application ID. | [optional] [readonly] 
**LoginPageUrl** | Pointer to **string** | A string that specifies the custom login page URL for the application. If you set the loginPageUrl property for applications in an environment that sets a custom domain, the URL should include the top-level domain and at least one additional domain level. Warning To avoid issues with third-party cookies in some browsers, a custom domain must be used, giving your PingOne environment the same parent domain as your authentication application. For more information about custom domains, see Custom domains. | [optional] 
**Name** | **string** | A string that specifies the name of the application. This is a required property. | 
**Protocol** | [**EnumApplicationProtocol**](EnumApplicationProtocol.md) |  | 
**Type** | [**EnumApplicationType**](EnumApplicationType.md) |  | 
**UpdatedAt** | Pointer to **time.Time** | The time the resource was last updated. | [optional] [readonly] 
**AssertionDuration** | Pointer to **int32** | The assertion validity duration in seconds. The default value is 300 seconds (5 minutes). Valid values are between 300 and 3932100. | [optional] [default to 300]
**AudienceRestriction** | Pointer to **string** | The service provider ID. Defaults to &#x60;urn:federation:MicrosoftOnline&#x60;. | [optional] [default to "urn:federation:MicrosoftOnline"]
**CorsSettings** | Pointer to [**ApplicationCorsSettings**](ApplicationCorsSettings.md) |  | [optional] 
**DomainName** | **string** | The federated domain name (for example, the Azure custom domain). | 
**HybridJoinDeviceAttribute** | Pointer to **string** | Required for Entra ID hybrid join. The value must be the name of a custom user attribute that an administrator has created. See [Creating attributes and a population for hybrid joined devices](https://docs.pingidentity.com/pingone/use_cases/p1_microsoft_entra_hybrid_join.html#p1-create-attributes) for more information. | [optional] 
**StsTokenType** | Pointer to [**EnumApplicationWSFEDStsTokenType**](EnumApplicationWSFEDStsTokenType.md) |  | [optional] 
**UseMex13** | Pointer to **bool** | Must be &#x60;true&#x60; to enable Entra ID hybrid join. After it&#39;s set to &#x60;true&#x60;, update Entra ID to use the new metadata exchange endpoint. See [Updating the federated IdP setting](https://docs.pingidentity.com/pingone/use_cases/p1_microsoft_entra_hybrid_join.html#p1-update-federated-idp) for more information. | [optional] 
**UserAttributeUsernameMatch** | Pointer to **string** | Specifies the PingOne user attribute used to match the username from a Security Token Service (STS) request to an existing user profile. By default, PingOne matches the username against the user&#39;s email address. Configure this setting if the username in the token is the user&#39;s user principal name (&#x60;userPrincipalName&#x60; attribute in Active Directory) but it differs from their email address (&#x60;mail&#x60; attribute in Active Directory), or if the username is something other than the user&#39;s user principal name or email address. The selected attribute must match the username format in the token to ensure successful identification. When specifying a PingOne custom user attribute as the &#x60;userAttributeUsernameMatch&#x60; property value, the admin must ensure the attribute is configured with the schemaType &#x60;CUSTOM&#x60;, type &#x60;STRING&#x60;, unique &#x60;true&#x60;, enabled &#x60;true&#x60;, and multiValued &#x60;false&#x60;. | [optional] 
**UserAttributeX509Match** | Pointer to **string** | The user attribute to match against the user information in the X.509 certificate. Supports Microsoft Windows primary refresh token (PRT) operations when users log on to their Windows devices, or unlock their locked Windows devices, using PingID. See [Integrating PingID with Windows Login](https://docs.pingidentity.com/pingid/pingid_integrations/pid_integrating_with_windows_login_passwordless.html). If this setting isn&#39;t specified, Windows PRT operations are still supported, but only when users log on to (or unlock) their Windows devices using their username and password. | [optional] 
**ValidIssuanceCertificates** | Pointer to [**[]ApplicationWSFEDAllOfValidIssuanceCertificates**](ApplicationWSFEDAllOfValidIssuanceCertificates.md) | Contains the list of valid issuance certificate IDs for the application. A maximum of 10 certificate IDs can be specified. Supports Microsoft Windows primary refresh token (PRT) operations when users log on to their Windows devices, or unlock their locked Windows devices, using PingID. See [Integrating PingID with Windows Login](https://docs.pingidentity.com/pingid/pingid_integrations/pid_integrating_with_windows_login_passwordless.html). If this setting isn&#39;t specified, Windows PRT operations are still supported, but only when users log on to (or unlock) their Windows devices using their username and password. | [optional] 
**IdpSigning** | [**ApplicationWSFEDAllOfIdpSigning**](ApplicationWSFEDAllOfIdpSigning.md) |  | 
**Kerberos** | Pointer to [**ApplicationWSFEDAllOfKerberos**](ApplicationWSFEDAllOfKerberos.md) |  | [optional] 
**ReplyUrl** | **string** | The URL that the replying party (such as, Office365) uses to accept submissions of RequestSecurityTokenResponse messages that are a result of SSO requests. | 
**SloEndpoint** | Pointer to **string** | The single logout endpoint URL. | [optional] 
**SubjectNameIdentifierFormat** | Pointer to [**EnumApplicationWSFEDSubjectNameIdentifierFormat**](EnumApplicationWSFEDSubjectNameIdentifierFormat.md) |  | [optional] 
**WsTrustVersion** | Pointer to [**EnumApplicationWSFEDWsTrustVersion**](EnumApplicationWSFEDWsTrustVersion.md) |  | [optional] 

## Methods

### NewApplicationWSFED

`func NewApplicationWSFED(enabled bool, name string, protocol EnumApplicationProtocol, type_ EnumApplicationType, domainName string, idpSigning ApplicationWSFEDAllOfIdpSigning, replyUrl string, ) *ApplicationWSFED`

NewApplicationWSFED instantiates a new ApplicationWSFED object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationWSFEDWithDefaults

`func NewApplicationWSFEDWithDefaults() *ApplicationWSFED`

NewApplicationWSFEDWithDefaults instantiates a new ApplicationWSFED object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLinks

`func (o *ApplicationWSFED) GetLinks() map[string]LinksHATEOASValue`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *ApplicationWSFED) GetLinksOk() (*map[string]LinksHATEOASValue, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *ApplicationWSFED) SetLinks(v map[string]LinksHATEOASValue)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *ApplicationWSFED) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### GetAccessControl

`func (o *ApplicationWSFED) GetAccessControl() ApplicationAccessControl`

GetAccessControl returns the AccessControl field if non-nil, zero value otherwise.

### GetAccessControlOk

`func (o *ApplicationWSFED) GetAccessControlOk() (*ApplicationAccessControl, bool)`

GetAccessControlOk returns a tuple with the AccessControl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessControl

`func (o *ApplicationWSFED) SetAccessControl(v ApplicationAccessControl)`

SetAccessControl sets AccessControl field to given value.

### HasAccessControl

`func (o *ApplicationWSFED) HasAccessControl() bool`

HasAccessControl returns a boolean if a field has been set.

### GetCreatedAt

`func (o *ApplicationWSFED) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ApplicationWSFED) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ApplicationWSFED) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ApplicationWSFED) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetDescription

`func (o *ApplicationWSFED) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ApplicationWSFED) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ApplicationWSFED) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ApplicationWSFED) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetEnabled

`func (o *ApplicationWSFED) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *ApplicationWSFED) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *ApplicationWSFED) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetEnvironment

`func (o *ApplicationWSFED) GetEnvironment() ObjectEnvironment`

GetEnvironment returns the Environment field if non-nil, zero value otherwise.

### GetEnvironmentOk

`func (o *ApplicationWSFED) GetEnvironmentOk() (*ObjectEnvironment, bool)`

GetEnvironmentOk returns a tuple with the Environment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironment

`func (o *ApplicationWSFED) SetEnvironment(v ObjectEnvironment)`

SetEnvironment sets Environment field to given value.

### HasEnvironment

`func (o *ApplicationWSFED) HasEnvironment() bool`

HasEnvironment returns a boolean if a field has been set.

### GetHiddenFromAppPortal

`func (o *ApplicationWSFED) GetHiddenFromAppPortal() bool`

GetHiddenFromAppPortal returns the HiddenFromAppPortal field if non-nil, zero value otherwise.

### GetHiddenFromAppPortalOk

`func (o *ApplicationWSFED) GetHiddenFromAppPortalOk() (*bool, bool)`

GetHiddenFromAppPortalOk returns a tuple with the HiddenFromAppPortal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHiddenFromAppPortal

`func (o *ApplicationWSFED) SetHiddenFromAppPortal(v bool)`

SetHiddenFromAppPortal sets HiddenFromAppPortal field to given value.

### HasHiddenFromAppPortal

`func (o *ApplicationWSFED) HasHiddenFromAppPortal() bool`

HasHiddenFromAppPortal returns a boolean if a field has been set.

### GetIcon

`func (o *ApplicationWSFED) GetIcon() ApplicationIcon`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *ApplicationWSFED) GetIconOk() (*ApplicationIcon, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *ApplicationWSFED) SetIcon(v ApplicationIcon)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *ApplicationWSFED) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### GetId

`func (o *ApplicationWSFED) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApplicationWSFED) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApplicationWSFED) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ApplicationWSFED) HasId() bool`

HasId returns a boolean if a field has been set.

### GetLoginPageUrl

`func (o *ApplicationWSFED) GetLoginPageUrl() string`

GetLoginPageUrl returns the LoginPageUrl field if non-nil, zero value otherwise.

### GetLoginPageUrlOk

`func (o *ApplicationWSFED) GetLoginPageUrlOk() (*string, bool)`

GetLoginPageUrlOk returns a tuple with the LoginPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoginPageUrl

`func (o *ApplicationWSFED) SetLoginPageUrl(v string)`

SetLoginPageUrl sets LoginPageUrl field to given value.

### HasLoginPageUrl

`func (o *ApplicationWSFED) HasLoginPageUrl() bool`

HasLoginPageUrl returns a boolean if a field has been set.

### GetName

`func (o *ApplicationWSFED) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApplicationWSFED) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApplicationWSFED) SetName(v string)`

SetName sets Name field to given value.


### GetProtocol

`func (o *ApplicationWSFED) GetProtocol() EnumApplicationProtocol`

GetProtocol returns the Protocol field if non-nil, zero value otherwise.

### GetProtocolOk

`func (o *ApplicationWSFED) GetProtocolOk() (*EnumApplicationProtocol, bool)`

GetProtocolOk returns a tuple with the Protocol field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtocol

`func (o *ApplicationWSFED) SetProtocol(v EnumApplicationProtocol)`

SetProtocol sets Protocol field to given value.


### GetType

`func (o *ApplicationWSFED) GetType() EnumApplicationType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ApplicationWSFED) GetTypeOk() (*EnumApplicationType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ApplicationWSFED) SetType(v EnumApplicationType)`

SetType sets Type field to given value.


### GetUpdatedAt

`func (o *ApplicationWSFED) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ApplicationWSFED) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ApplicationWSFED) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *ApplicationWSFED) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### GetAssertionDuration

`func (o *ApplicationWSFED) GetAssertionDuration() int32`

GetAssertionDuration returns the AssertionDuration field if non-nil, zero value otherwise.

### GetAssertionDurationOk

`func (o *ApplicationWSFED) GetAssertionDurationOk() (*int32, bool)`

GetAssertionDurationOk returns a tuple with the AssertionDuration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssertionDuration

`func (o *ApplicationWSFED) SetAssertionDuration(v int32)`

SetAssertionDuration sets AssertionDuration field to given value.

### HasAssertionDuration

`func (o *ApplicationWSFED) HasAssertionDuration() bool`

HasAssertionDuration returns a boolean if a field has been set.

### GetAudienceRestriction

`func (o *ApplicationWSFED) GetAudienceRestriction() string`

GetAudienceRestriction returns the AudienceRestriction field if non-nil, zero value otherwise.

### GetAudienceRestrictionOk

`func (o *ApplicationWSFED) GetAudienceRestrictionOk() (*string, bool)`

GetAudienceRestrictionOk returns a tuple with the AudienceRestriction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAudienceRestriction

`func (o *ApplicationWSFED) SetAudienceRestriction(v string)`

SetAudienceRestriction sets AudienceRestriction field to given value.

### HasAudienceRestriction

`func (o *ApplicationWSFED) HasAudienceRestriction() bool`

HasAudienceRestriction returns a boolean if a field has been set.

### GetCorsSettings

`func (o *ApplicationWSFED) GetCorsSettings() ApplicationCorsSettings`

GetCorsSettings returns the CorsSettings field if non-nil, zero value otherwise.

### GetCorsSettingsOk

`func (o *ApplicationWSFED) GetCorsSettingsOk() (*ApplicationCorsSettings, bool)`

GetCorsSettingsOk returns a tuple with the CorsSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCorsSettings

`func (o *ApplicationWSFED) SetCorsSettings(v ApplicationCorsSettings)`

SetCorsSettings sets CorsSettings field to given value.

### HasCorsSettings

`func (o *ApplicationWSFED) HasCorsSettings() bool`

HasCorsSettings returns a boolean if a field has been set.

### GetDomainName

`func (o *ApplicationWSFED) GetDomainName() string`

GetDomainName returns the DomainName field if non-nil, zero value otherwise.

### GetDomainNameOk

`func (o *ApplicationWSFED) GetDomainNameOk() (*string, bool)`

GetDomainNameOk returns a tuple with the DomainName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomainName

`func (o *ApplicationWSFED) SetDomainName(v string)`

SetDomainName sets DomainName field to given value.


### GetHybridJoinDeviceAttribute

`func (o *ApplicationWSFED) GetHybridJoinDeviceAttribute() string`

GetHybridJoinDeviceAttribute returns the HybridJoinDeviceAttribute field if non-nil, zero value otherwise.

### GetHybridJoinDeviceAttributeOk

`func (o *ApplicationWSFED) GetHybridJoinDeviceAttributeOk() (*string, bool)`

GetHybridJoinDeviceAttributeOk returns a tuple with the HybridJoinDeviceAttribute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHybridJoinDeviceAttribute

`func (o *ApplicationWSFED) SetHybridJoinDeviceAttribute(v string)`

SetHybridJoinDeviceAttribute sets HybridJoinDeviceAttribute field to given value.

### HasHybridJoinDeviceAttribute

`func (o *ApplicationWSFED) HasHybridJoinDeviceAttribute() bool`

HasHybridJoinDeviceAttribute returns a boolean if a field has been set.

### GetStsTokenType

`func (o *ApplicationWSFED) GetStsTokenType() EnumApplicationWSFEDStsTokenType`

GetStsTokenType returns the StsTokenType field if non-nil, zero value otherwise.

### GetStsTokenTypeOk

`func (o *ApplicationWSFED) GetStsTokenTypeOk() (*EnumApplicationWSFEDStsTokenType, bool)`

GetStsTokenTypeOk returns a tuple with the StsTokenType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStsTokenType

`func (o *ApplicationWSFED) SetStsTokenType(v EnumApplicationWSFEDStsTokenType)`

SetStsTokenType sets StsTokenType field to given value.

### HasStsTokenType

`func (o *ApplicationWSFED) HasStsTokenType() bool`

HasStsTokenType returns a boolean if a field has been set.

### GetUseMex13

`func (o *ApplicationWSFED) GetUseMex13() bool`

GetUseMex13 returns the UseMex13 field if non-nil, zero value otherwise.

### GetUseMex13Ok

`func (o *ApplicationWSFED) GetUseMex13Ok() (*bool, bool)`

GetUseMex13Ok returns a tuple with the UseMex13 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUseMex13

`func (o *ApplicationWSFED) SetUseMex13(v bool)`

SetUseMex13 sets UseMex13 field to given value.

### HasUseMex13

`func (o *ApplicationWSFED) HasUseMex13() bool`

HasUseMex13 returns a boolean if a field has been set.

### GetUserAttributeUsernameMatch

`func (o *ApplicationWSFED) GetUserAttributeUsernameMatch() string`

GetUserAttributeUsernameMatch returns the UserAttributeUsernameMatch field if non-nil, zero value otherwise.

### GetUserAttributeUsernameMatchOk

`func (o *ApplicationWSFED) GetUserAttributeUsernameMatchOk() (*string, bool)`

GetUserAttributeUsernameMatchOk returns a tuple with the UserAttributeUsernameMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserAttributeUsernameMatch

`func (o *ApplicationWSFED) SetUserAttributeUsernameMatch(v string)`

SetUserAttributeUsernameMatch sets UserAttributeUsernameMatch field to given value.

### HasUserAttributeUsernameMatch

`func (o *ApplicationWSFED) HasUserAttributeUsernameMatch() bool`

HasUserAttributeUsernameMatch returns a boolean if a field has been set.

### GetUserAttributeX509Match

`func (o *ApplicationWSFED) GetUserAttributeX509Match() string`

GetUserAttributeX509Match returns the UserAttributeX509Match field if non-nil, zero value otherwise.

### GetUserAttributeX509MatchOk

`func (o *ApplicationWSFED) GetUserAttributeX509MatchOk() (*string, bool)`

GetUserAttributeX509MatchOk returns a tuple with the UserAttributeX509Match field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserAttributeX509Match

`func (o *ApplicationWSFED) SetUserAttributeX509Match(v string)`

SetUserAttributeX509Match sets UserAttributeX509Match field to given value.

### HasUserAttributeX509Match

`func (o *ApplicationWSFED) HasUserAttributeX509Match() bool`

HasUserAttributeX509Match returns a boolean if a field has been set.

### GetValidIssuanceCertificates

`func (o *ApplicationWSFED) GetValidIssuanceCertificates() []ApplicationWSFEDAllOfValidIssuanceCertificates`

GetValidIssuanceCertificates returns the ValidIssuanceCertificates field if non-nil, zero value otherwise.

### GetValidIssuanceCertificatesOk

`func (o *ApplicationWSFED) GetValidIssuanceCertificatesOk() (*[]ApplicationWSFEDAllOfValidIssuanceCertificates, bool)`

GetValidIssuanceCertificatesOk returns a tuple with the ValidIssuanceCertificates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidIssuanceCertificates

`func (o *ApplicationWSFED) SetValidIssuanceCertificates(v []ApplicationWSFEDAllOfValidIssuanceCertificates)`

SetValidIssuanceCertificates sets ValidIssuanceCertificates field to given value.

### HasValidIssuanceCertificates

`func (o *ApplicationWSFED) HasValidIssuanceCertificates() bool`

HasValidIssuanceCertificates returns a boolean if a field has been set.

### GetIdpSigning

`func (o *ApplicationWSFED) GetIdpSigning() ApplicationWSFEDAllOfIdpSigning`

GetIdpSigning returns the IdpSigning field if non-nil, zero value otherwise.

### GetIdpSigningOk

`func (o *ApplicationWSFED) GetIdpSigningOk() (*ApplicationWSFEDAllOfIdpSigning, bool)`

GetIdpSigningOk returns a tuple with the IdpSigning field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdpSigning

`func (o *ApplicationWSFED) SetIdpSigning(v ApplicationWSFEDAllOfIdpSigning)`

SetIdpSigning sets IdpSigning field to given value.


### GetKerberos

`func (o *ApplicationWSFED) GetKerberos() ApplicationWSFEDAllOfKerberos`

GetKerberos returns the Kerberos field if non-nil, zero value otherwise.

### GetKerberosOk

`func (o *ApplicationWSFED) GetKerberosOk() (*ApplicationWSFEDAllOfKerberos, bool)`

GetKerberosOk returns a tuple with the Kerberos field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKerberos

`func (o *ApplicationWSFED) SetKerberos(v ApplicationWSFEDAllOfKerberos)`

SetKerberos sets Kerberos field to given value.

### HasKerberos

`func (o *ApplicationWSFED) HasKerberos() bool`

HasKerberos returns a boolean if a field has been set.

### GetReplyUrl

`func (o *ApplicationWSFED) GetReplyUrl() string`

GetReplyUrl returns the ReplyUrl field if non-nil, zero value otherwise.

### GetReplyUrlOk

`func (o *ApplicationWSFED) GetReplyUrlOk() (*string, bool)`

GetReplyUrlOk returns a tuple with the ReplyUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplyUrl

`func (o *ApplicationWSFED) SetReplyUrl(v string)`

SetReplyUrl sets ReplyUrl field to given value.


### GetSloEndpoint

`func (o *ApplicationWSFED) GetSloEndpoint() string`

GetSloEndpoint returns the SloEndpoint field if non-nil, zero value otherwise.

### GetSloEndpointOk

`func (o *ApplicationWSFED) GetSloEndpointOk() (*string, bool)`

GetSloEndpointOk returns a tuple with the SloEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSloEndpoint

`func (o *ApplicationWSFED) SetSloEndpoint(v string)`

SetSloEndpoint sets SloEndpoint field to given value.

### HasSloEndpoint

`func (o *ApplicationWSFED) HasSloEndpoint() bool`

HasSloEndpoint returns a boolean if a field has been set.

### GetSubjectNameIdentifierFormat

`func (o *ApplicationWSFED) GetSubjectNameIdentifierFormat() EnumApplicationWSFEDSubjectNameIdentifierFormat`

GetSubjectNameIdentifierFormat returns the SubjectNameIdentifierFormat field if non-nil, zero value otherwise.

### GetSubjectNameIdentifierFormatOk

`func (o *ApplicationWSFED) GetSubjectNameIdentifierFormatOk() (*EnumApplicationWSFEDSubjectNameIdentifierFormat, bool)`

GetSubjectNameIdentifierFormatOk returns a tuple with the SubjectNameIdentifierFormat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectNameIdentifierFormat

`func (o *ApplicationWSFED) SetSubjectNameIdentifierFormat(v EnumApplicationWSFEDSubjectNameIdentifierFormat)`

SetSubjectNameIdentifierFormat sets SubjectNameIdentifierFormat field to given value.

### HasSubjectNameIdentifierFormat

`func (o *ApplicationWSFED) HasSubjectNameIdentifierFormat() bool`

HasSubjectNameIdentifierFormat returns a boolean if a field has been set.

### GetWsTrustVersion

`func (o *ApplicationWSFED) GetWsTrustVersion() EnumApplicationWSFEDWsTrustVersion`

GetWsTrustVersion returns the WsTrustVersion field if non-nil, zero value otherwise.

### GetWsTrustVersionOk

`func (o *ApplicationWSFED) GetWsTrustVersionOk() (*EnumApplicationWSFEDWsTrustVersion, bool)`

GetWsTrustVersionOk returns a tuple with the WsTrustVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWsTrustVersion

`func (o *ApplicationWSFED) SetWsTrustVersion(v EnumApplicationWSFEDWsTrustVersion)`

SetWsTrustVersion sets WsTrustVersion field to given value.

### HasWsTrustVersion

`func (o *ApplicationWSFED) HasWsTrustVersion() bool`

HasWsTrustVersion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
# Get app state

Get the given app status on the device
[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
## Example Usage

```java
// Java
driver.queryAppState('com.apple.Preferences');
driver.queryAppState('io.appium.android.apis');

```

```python
# Python
driver.query_app_state('com.apple.Preferences')
driver.query_app_state('io.appium.android.apis')

```

```javascript
// Javascript
// webdriver.io example
driver.queryAppState(null, 'com.apple.Preferences')
driver.queryAppState('io.appium.android.apis')

// wd example
// Supports only `mobile: queryAppState` for iOS, XCUITest

```

```ruby
# Ruby
# ruby_lib example
app_state('com.apple.Preferences')
query_app_state('io.appium.android.apis') # `query_` prefix is also available

# ruby_lib_core example
@driver.app_state('com.apple.Preferences')
@driver.query_app_state('io.appium.android.apis') # `query_` prefix is also available

```

```csharp
// C#
// Supports only `mobile: queryAppState` for iOS, XCUITest

```

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
## Description

iOS tests with XCUITest can also use the `mobile: queryAppState` method. See detailed [documentation](http://appium.io/docs/en/writing-running-appium/ios/ios-xctest-mobile-apps-management/index.html#mobile-queryappstate).


[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
## Support

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | None | None | None |
| Android | [Espresso](/docs/en/drivers/android-espresso.md) | ?+ | 1.9.0+ | All |
|  | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.3+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | None | None | None |
| Windows | [Windows](/docs/en/drivers/windows.md) | None | None | None |


[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### Appium Clients

|Language|Support|Documentation|
|--------|-------|-------------|
|[Java](https://github.com/appium/java-client/releases/latest)| All | [appium.github.io](https://appium.github.io/java-client/io/appium/java_client/InteractsWithApps.html#queryAppState-java.lang.String-) |
|[Python](https://github.com/appium/python-client/releases/latest)| All | [appium.github.io](https://appium.github.io/python-client-sphinx/webdriver.extensions.html#webdriver.extensions.applications.Applications.query_app_state) |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |  |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All | [github.com](https://github.com/admc/wd/blob/master/lib/commands.js) |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All | [www.rubydoc.info](https://www.rubydoc.info/github/appium/ruby_lib_core/Appium/Core/Base/Driver#app_state-instance_method) |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All | [github.com](https://github.com/appium/appium-dotnet-driver/) |

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
## HTTP API Specifications

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### Endpoint

`POST /session/:session_id/appium/device/app_state`

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### JSON Parameters

|name|type|description|
|----|----|-----------|
| bundleId or appId | `string` | BundleId for iOS. Package name for Android. |

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
### Response

Current the target app status. (Clients wrap the response properly) `0` is not installed. `1` is not running. `2` is running in background or suspended. `3` is running in background. `4` is running in foreground. (`number`)

[//]: # (DO NOT EDIT THIS FILE! This is an auto-generated file. Editing for this document happens in /commands-yml/commands/device/app/app-state.yml)
## See Also

* [JSONWP Specification](https://github.com/appium/appium-base-driver/blob/master/lib/protocol/routes.js#L481)

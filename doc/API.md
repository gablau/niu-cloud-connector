## Objects

<dl>
<dt><a href="#niuCloudConnector">niuCloudConnector</a> : <code>object</code></dt>
<dd><p>NIU cloud connector</p>
</dd>
</dl>

## Typedefs

<dl>
<dt><a href="#Error">Error</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#Token">Token</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#Vehicles">Vehicles</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#VehiclePos">VehiclePos</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#OverallTally">OverallTally</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#TrackDetail">TrackDetail</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#CompartmentBatteryInfo">CompartmentBatteryInfo</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#BatteryInfo">BatteryInfo</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#CompartmentBatteryInfoHealth">CompartmentBatteryInfoHealth</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#BatteryInfoHealth">BatteryInfoHealth</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#BatteryChartData">BatteryChartData</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#BatteryChart">BatteryChart</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#CompartmentMotorData">CompartmentMotorData</a> : <code>Object</code></dt>
<dd></dd>
<dt><a href="#MotorData">MotorData</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#Tracks">Tracks</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#FirmwareVersion">FirmwareVersion</a> : <code>Promise</code></dt>
<dd></dd>
<dt><a href="#UpdateInfo">UpdateInfo</a> : <code>Promise</code></dt>
<dd></dd>
</dl>

<a name="niuCloudConnector"></a>

## niuCloudConnector : <code>object</code>
NIU cloud connector

**Kind**: global namespace  

* [niuCloudConnector](#niuCloudConnector) : <code>object</code>
    * [.Client](#niuCloudConnector.Client)
        * [new niuCloudConnector.Client()](#new_niuCloudConnector.Client_new)
        * [._isDebugMode](#niuCloudConnector.Client+_isDebugMode)
        * [._token](#niuCloudConnector.Client+_token)
        * [._acceptLanguage](#niuCloudConnector.Client+_acceptLanguage)
        * [._niuAppVersion](#niuCloudConnector.Client+_niuAppVersion)
        * [._userAgent](#niuCloudConnector.Client+_userAgent)
        * [._appId](#niuCloudConnector.Client+_appId)
        * [.enableDebugMode(enableDebugMode)](#niuCloudConnector.Client+enableDebugMode)
        * [.createSessionToken(data)](#niuCloudConnector.Client+createSessionToken) ⇒ [<code>Token</code>](#Token)
        * [.setSessionToken(options)](#niuCloudConnector.Client+setSessionToken) ⇒ <code>Promise</code>
        * [.getVehicles()](#niuCloudConnector.Client+getVehicles) ⇒ [<code>Vehicles</code>](#Vehicles)
        * [.getVehiclePos(options)](#niuCloudConnector.Client+getVehiclePos) ⇒ [<code>VehiclePos</code>](#VehiclePos)
        * [.getOverallTally(options)](#niuCloudConnector.Client+getOverallTally) ⇒ [<code>OverallTally</code>](#OverallTally)
        * [.getTrackDetail(options)](#niuCloudConnector.Client+getTrackDetail) ⇒ [<code>TrackDetail</code>](#TrackDetail)
        * [.getBatteryInfo(options)](#niuCloudConnector.Client+getBatteryInfo) ⇒ [<code>BatteryInfo</code>](#BatteryInfo)
        * [.getBatteryHealth(options)](#niuCloudConnector.Client+getBatteryHealth) ⇒ [<code>BatteryInfoHealth</code>](#BatteryInfoHealth)
        * [.getBatteryChart(options)](#niuCloudConnector.Client+getBatteryChart) ⇒ [<code>BatteryChart</code>](#BatteryChart)
        * [.getMotorInfo(options)](#niuCloudConnector.Client+getMotorInfo) ⇒ [<code>MotorData</code>](#MotorData)
        * [.getTracks(options)](#niuCloudConnector.Client+getTracks) ⇒ [<code>Tracks</code>](#Tracks)
        * [.getFirmwareVersion(options)](#niuCloudConnector.Client+getFirmwareVersion) ⇒ [<code>FirmwareVersion</code>](#FirmwareVersion)
        * [.getUpdateInfo(options)](#niuCloudConnector.Client+getUpdateInfo) ⇒ [<code>UpdateInfo</code>](#UpdateInfo)
    * [.AccountBaseUrl](#niuCloudConnector.AccountBaseUrl)
    * [.AppApiBaseUrl](#niuCloudConnector.AppApiBaseUrl)

<a name="niuCloudConnector.Client"></a>

### niuCloudConnector.Client
**Kind**: static class of [<code>niuCloudConnector</code>](#niuCloudConnector)  

* [.Client](#niuCloudConnector.Client)
    * [new niuCloudConnector.Client()](#new_niuCloudConnector.Client_new)
    * [._isDebugMode](#niuCloudConnector.Client+_isDebugMode)
    * [._token](#niuCloudConnector.Client+_token)
    * [._acceptLanguage](#niuCloudConnector.Client+_acceptLanguage)
    * [._niuAppVersion](#niuCloudConnector.Client+_niuAppVersion)
    * [._userAgent](#niuCloudConnector.Client+_userAgent)
    * [._appId](#niuCloudConnector.Client+_appId)
    * [.enableDebugMode(enableDebugMode)](#niuCloudConnector.Client+enableDebugMode)
    * [.createSessionToken(data)](#niuCloudConnector.Client+createSessionToken) ⇒ [<code>Token</code>](#Token)
    * [.setSessionToken(options)](#niuCloudConnector.Client+setSessionToken) ⇒ <code>Promise</code>
    * [.getVehicles()](#niuCloudConnector.Client+getVehicles) ⇒ [<code>Vehicles</code>](#Vehicles)
    * [.getVehiclePos(options)](#niuCloudConnector.Client+getVehiclePos) ⇒ [<code>VehiclePos</code>](#VehiclePos)
    * [.getOverallTally(options)](#niuCloudConnector.Client+getOverallTally) ⇒ [<code>OverallTally</code>](#OverallTally)
    * [.getTrackDetail(options)](#niuCloudConnector.Client+getTrackDetail) ⇒ [<code>TrackDetail</code>](#TrackDetail)
    * [.getBatteryInfo(options)](#niuCloudConnector.Client+getBatteryInfo) ⇒ [<code>BatteryInfo</code>](#BatteryInfo)
    * [.getBatteryHealth(options)](#niuCloudConnector.Client+getBatteryHealth) ⇒ [<code>BatteryInfoHealth</code>](#BatteryInfoHealth)
    * [.getBatteryChart(options)](#niuCloudConnector.Client+getBatteryChart) ⇒ [<code>BatteryChart</code>](#BatteryChart)
    * [.getMotorInfo(options)](#niuCloudConnector.Client+getMotorInfo) ⇒ [<code>MotorData</code>](#MotorData)
    * [.getTracks(options)](#niuCloudConnector.Client+getTracks) ⇒ [<code>Tracks</code>](#Tracks)
    * [.getFirmwareVersion(options)](#niuCloudConnector.Client+getFirmwareVersion) ⇒ [<code>FirmwareVersion</code>](#FirmwareVersion)
    * [.getUpdateInfo(options)](#niuCloudConnector.Client+getUpdateInfo) ⇒ [<code>UpdateInfo</code>](#UpdateInfo)

<a name="new_niuCloudConnector.Client_new"></a>

#### new niuCloudConnector.Client()
NIU cloud connector client.

<a name="niuCloudConnector.Client+_isDebugMode"></a>

#### client.\_isDebugMode
Enable/Disable debug output

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+_token"></a>

#### client.\_token
Session token

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+_acceptLanguage"></a>

#### client.\_acceptLanguage
Accept language, used in HTTP request header.

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+_niuAppVersion"></a>

#### client.\_niuAppVersion
The NIU app version, which the niu-cloud-connector is derrived from.

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+_userAgent"></a>

#### client.\_userAgent
User agent, used in HTTP request header.

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+_appId"></a>

#### client.\_appId
APP id

**Kind**: instance property of [<code>Client</code>](#niuCloudConnector.Client)  
<a name="niuCloudConnector.Client+enableDebugMode"></a>

#### client.enableDebugMode(enableDebugMode)
Enable/Disable the debug mode.In the debug mode the whole HTTP response is printed to console.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  

| Param | Type | Description |
| --- | --- | --- |
| enableDebugMode | <code>boolean</code> | Enable/Disable debug mode. |

<a name="niuCloudConnector.Client+createSessionToken"></a>

#### client.createSessionToken(data) ⇒ [<code>Token</code>](#Token)
Create a session token, to get access to the cloud API.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>Token</code>](#Token) - Session token.  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>Object</code> | Data. |
| data.account | <code>string</code> | EMail address or mobile phone number or username. |
| data.password | <code>string</code> | Account password. |

<a name="niuCloudConnector.Client+setSessionToken"></a>

#### client.setSessionToken(options) ⇒ <code>Promise</code>
Set a previous created session token, to get access to the cloud API.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: <code>Promise</code> - Nothing.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.token | <code>string</code> | Session token. |

<a name="niuCloudConnector.Client+getVehicles"></a>

#### client.getVehicles() ⇒ [<code>Vehicles</code>](#Vehicles)
Get a list of vehicles.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>Vehicles</code>](#Vehicles) - Vehicles.  
<a name="niuCloudConnector.Client+getVehiclePos"></a>

#### client.getVehiclePos(options) ⇒ [<code>VehiclePos</code>](#VehiclePos)
Get current position of a vehicle.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>VehiclePos</code>](#VehiclePos) - Vehicle position.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getOverallTally"></a>

#### client.getOverallTally(options) ⇒ [<code>OverallTally</code>](#OverallTally)
Get overall tally of vehicle.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>OverallTally</code>](#OverallTally) - Overall tally.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getTrackDetail"></a>

#### client.getTrackDetail(options) ⇒ [<code>TrackDetail</code>](#TrackDetail)
Get track details.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>TrackDetail</code>](#TrackDetail) - Track detail.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |
| options.trackId | <code>string</code> | Track identification number. |
| options.trackDate | <code>string</code> | Track date in yyyymmdd format. |

<a name="niuCloudConnector.Client+getBatteryInfo"></a>

#### client.getBatteryInfo(options) ⇒ [<code>BatteryInfo</code>](#BatteryInfo)
Get battery info of vehicle.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>BatteryInfo</code>](#BatteryInfo) - Battery info.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getBatteryHealth"></a>

#### client.getBatteryHealth(options) ⇒ [<code>BatteryInfoHealth</code>](#BatteryInfoHealth)
Get battery health of vehicle.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>BatteryInfoHealth</code>](#BatteryInfoHealth) - Battery info health.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getBatteryChart"></a>

#### client.getBatteryChart(options) ⇒ [<code>BatteryChart</code>](#BatteryChart)
Get battery chart data.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>BatteryChart</code>](#BatteryChart) - Battery chart information.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |
| options.bmsId | <code>number</code> | Selects the battery (1: Battery A / 2: Battery B / 3: Battery ???). |
| options.page | <code>number</code> | The page number selects the data. Start always with 1. |
| options.pageSize | <code>string</code> | 'A' or 'B'. Using 'B' instead of 'A' results in getting more data at once. |
| options.pageLength | <code>number</code> | [1; 2]. Controls whether the result contains a second array of data. |

<a name="niuCloudConnector.Client+getMotorInfo"></a>

#### client.getMotorInfo(options) ⇒ [<code>MotorData</code>](#MotorData)
Get motor info of vehicle.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>MotorData</code>](#MotorData) - Motor data.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getTracks"></a>

#### client.getTracks(options) ⇒ [<code>Tracks</code>](#Tracks)
Get recorded tracks.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>Tracks</code>](#Tracks) - Tracks.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |
| options.index | <code>number</code> | Start from this index. |
| options.pageSize | <code>number</code> | Number of tracks. |

<a name="niuCloudConnector.Client+getFirmwareVersion"></a>

#### client.getFirmwareVersion(options) ⇒ [<code>FirmwareVersion</code>](#FirmwareVersion)
Get firmware version.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>FirmwareVersion</code>](#FirmwareVersion) - Firmware version.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.Client+getUpdateInfo"></a>

#### client.getUpdateInfo(options) ⇒ [<code>UpdateInfo</code>](#UpdateInfo)
Get firmware version.

**Kind**: instance method of [<code>Client</code>](#niuCloudConnector.Client)  
**Returns**: [<code>UpdateInfo</code>](#UpdateInfo) - Update information.  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | Options. |
| options.sn | <code>string</code> | Vehicle serial number. |

<a name="niuCloudConnector.AccountBaseUrl"></a>

### niuCloudConnector.AccountBaseUrl
URL to NIU login, used for retrieving an access token.

**Kind**: static property of [<code>niuCloudConnector</code>](#niuCloudConnector)  
<a name="niuCloudConnector.AppApiBaseUrl"></a>

### niuCloudConnector.AppApiBaseUrl
URL to the NIU app API.

**Kind**: static property of [<code>niuCloudConnector</code>](#niuCloudConnector)  
<a name="Error"></a>

## Error : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type |
| --- | --- |
| error | <code>Object</code> | 
| [error.message] | <code>string</code> | 

<a name="Token"></a>

## Token : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>string</code> | Session token |

<a name="Vehicles"></a>

## Vehicles : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Array.&lt;Object&gt;</code> | Response data |
| data.sn | <code>string</code> | Vehicle serial number |
| data.specialEdition | <code>string</code> | ? |
| data.vehicleColorImg | <code>string</code> | URL to vehicle color image |
| data.vehicleLogoImg | <code>string</code> | URL to vehicle logo image |
| data.vehicleTypeId | <code>string</code> | Vehicle type id |
| data.indexHeaderBg | <code>string</code> | URL to background image |
| data.scootorImg | <code>string</code> | URL to vehicle image |
| data.batteryInfoBg | <code>string</code> | URL to battery info background image |
| data.myPageHeaderBg | <code>string</code> | URL to my page header background |
| data.listScooterImg | <code>string</code> | URL to scooter list background image |
| data.name | <code>string</code> | Vehicle name, given by the user |
| data.frameNo | <code>string</code> | Vehicle identification number (VIN) |
| data.engineNo | <code>string</code> | Engine identification number |
| data.isSelected | <code>boolean</code> | ? |
| data.isMaster | <code>boolean</code> | ? |
| data.bindNum | <code>number</code> | ? |
| data.renovated | <code>boolean</code> | ? |
| data.bindDate | <code>number</code> | ? timestamp in epoch unix timestamp format (13 digits) |
| data.isShow | <code>boolean</code> | ? |
| data.isLite | <code>boolean</code> | ? |
| data.gpsTimestamp | <code>number</code> | GPS timestamp in epoch unix timestamp format (13 digits) |
| data.infoTimestamp | <code>number</code> | Info timestamp in epoch unix timestamp format (13 digits) |
| data.productType | <code>string</code> | Product type, e.g. "native" |
| data.process | <code>string</code> | ? |
| data.brand | <code>string</code> | ? |
| data.isDoubleBattery | <code>boolean</code> | Vehicle has one or two batteries |
| data.features | <code>Array.&lt;Object&gt;</code> | List of features |
| data.features.featureName | <code>string</code> | Feature name |
| data.features.isSupport | <code>boolean</code> | ? |
| data.features.switch_status | <code>string</code> | ? |
| data.type | <code>string</code> | Vehicle model, e.g. "NGT  Black with Red Stripes" |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="VehiclePos"></a>

## VehiclePos : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.lat | <code>number</code> | Latitude in decimal degree (WGS 84) |
| data.lng | <code>number</code> | Longitude in decimal degree (WGS 84) |
| data.timestamp | <code>number</code> | Timestamp in unix timestamp epoch format (13 digits) |
| data.gps | <code>number</code> | ? |
| data.gpsPrecision | <code>number</code> | GPS precision |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="OverallTally"></a>

## OverallTally : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.bindDaysCount | <code>number</code> | Number of days the vehicle is at the customer |
| data.totalMileage | <code>number</code> | Total mileage in km |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="TrackDetail"></a>

## TrackDetail : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.trackItems | <code>Array.&lt;Object&gt;</code> | Track items (end point at index 0) |
| data.trackItems.lng | <code>number</code> | Longitude in decimal degree (WGS 84) |
| data.trackItems.lat | <code>number</code> | Latitude in decimal degree (WGS 84) |
| data.trackItems.date | <code>number</code> | Date in unix timestamp epoch format (13 digits) |
| data.startPoint | <code>Object</code> | Start point |
| data.startPoint.lng | <code>string</code> | Longitude in decimal degree (WGS 84) |
| data.startPoint.lat | <code>string</code> | Latitude in decimal degree (WGS 84) |
| data.lastPoint | <code>Object</code> | Start point |
| data.lastPoint.lng | <code>string</code> | Longitude in decimal degree (WGS 84) |
| data.lastPoint.lat | <code>string</code> | Latitude in decimal degree (WGS 84) |
| data.startTime | <code>string</code> | Start time in unix timestamp epoch format (13 digits) |
| data.lastDate | <code>string</code> | Last time in unix timestamp epoch format (13 digits) |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="CompartmentBatteryInfo"></a>

## CompartmentBatteryInfo : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| items | <code>Array.&lt;Object&gt;</code> | ? |
| items.x | <code>number</code> | ? |
| items.y | <code>number</code> | ? |
| items.z | <code>number</code> | ? |
| totalPoint | <code>number</code> | Number of items |
| bmsId | <code>string</code> | Battery management identification number |
| isConnected | <code>boolean</code> | Is battery connected or not |
| batteryCharging | <code>number</code> | State of charge in percent |
| chargedTimes | <code>string</code> | Charging cycles |
| temperature | <code>number</code> | Battery temperature in degree celsius |
| temperatureDesc | <code>string</code> | Battery temperature status |
| energyConsumedTody | <code>number</code> | Energy consumption of today |
| gradeBattery | <code>string</code> | Battery grade points |

<a name="BatteryInfo"></a>

## BatteryInfo : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.batteries | <code>Object</code> | Batteries |
| data.batteries.compartmentA | [<code>CompartmentBatteryInfo</code>](#CompartmentBatteryInfo) | Battery of compartment A |
| [data.batteries.compartmentB] | [<code>CompartmentBatteryInfo</code>](#CompartmentBatteryInfo) | Battery of compartment B |
| data.isCharging | <code>number</code> | Is charging |
| data.centreCtrlBattery | <code>string</code> | Centre control battery |
| data.batteryDetail | <code>boolean</code> | Battery detail |
| data.estimatedMileage | <code>number</code> | Estimated mileage in km |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="CompartmentBatteryInfoHealth"></a>

## CompartmentBatteryInfoHealth : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| bmsId | <code>string</code> | Battery management system identification number |
| isConnected | <code>boolean</code> | Is connected or not |
| gradeBattery | <code>string</code> | Battery grade points |
| faults | <code>Array.&lt;Object&gt;</code> | List of faults |
| healthRecords | <code>Array.&lt;Object&gt;</code> | List of health records |
| healthRecords.result | <code>string</code> | Battery lost grade points |
| healthRecords.chargeCount | <code>string</code> | Charging cycles |
| healthRecords.color | <code>string</code> | HTML color in #RGB format |
| healthRecords.time | <code>number</code> | Timestamp in unix timstamp epoch format (13 digits) |
| healthRecords.name | <code>string</code> | Name |

<a name="BatteryInfoHealth"></a>

## BatteryInfoHealth : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.batteries | <code>Object</code> | Batteries |
| data.batteries.compartmentA | [<code>CompartmentBatteryInfoHealth</code>](#CompartmentBatteryInfoHealth) | Battery compartment A |
| [data.batteries.compartmentB] | [<code>CompartmentBatteryInfoHealth</code>](#CompartmentBatteryInfoHealth) | Battery compratment B |
| data.isDoubleBattery | <code>boolean</code> | Vehicle has one or two batteries |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="BatteryChartData"></a>

## BatteryChartData : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| m | <code>string</code> | Mileage in km |
| b | <code>string</code> | Battery SOC in percent |

<a name="BatteryChart"></a>

## BatteryChart : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.items1 | [<code>BatteryChartData</code>](#BatteryChartData) | Battery data 1 |
| [data.items2] | [<code>BatteryChartData</code>](#BatteryChartData) | Battery data 2 |
| data.isDoubleBattery | <code>boolean</code> | Vehicle has one or two batteries |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="CompartmentMotorData"></a>

## CompartmentMotorData : <code>Object</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| bmsId | <code>string</code> | Battery management system identification number |
| isConnected | <code>boolean</code> | Battery is connected or not |
| batteryCharging | <code>number</code> | Battery is charging or not |
| gradeBattery | <code>string</code> | Battery grade points |

<a name="MotorData"></a>

## MotorData : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.isCharging | <code>number</code> | Is charging |
| data.lockStatus | <code>number</code> | Lock status |
| data.isAccOn | <code>number</code> | Is adaptive cruise control on or not |
| data.isFortificationOn | <code>string</code> | Is fortification on or not |
| data.isConnected | <code>boolean</code> | Is connected or not |
| data.postion | <code>Object</code> | Current position |
| data.postion.lat | <code>number</code> | Latitude in decimal degree (WGS 84) |
| data.postion.lng | <code>number</code> | Longitude in decimal degree (WGS 84) |
| data.hdop | <code>number</code> | Horizontal dilution of precision [0; 50]. A good HDOP is up to 2.5. For navigation a value up to 8 is acceptable. |
| data.time | <code>number</code> | Time in unix timestamp epoch format (13 digits) |
| data.batteries | <code>Object</code> | Batteries |
| data.batteries.compartmentA | [<code>CompartmentMotorData</code>](#CompartmentMotorData) | Battery compartment A |
| [data.batteries.compartmentB] | [<code>CompartmentMotorData</code>](#CompartmentMotorData) | Battery compartment B |
| data.leftTime | <code>string</code> | Left time |
| data.estimatedMileage | <code>number</code> | Estimated mileage in km |
| data.gpsTimestamp | <code>number</code> | GPS timestamp in unix timestamp epoch format (13 digits) |
| data.infoTimestamp | <code>number</code> | Info timestamp in unix timestamp epoch format (13 digits) |
| data.nowSpeed | <code>number</code> | Current speed in km/h |
| data.batteryDetail | <code>boolean</code> | Battery detail |
| data.centreCtrlBattery | <code>number</code> | Centre control battery |
| data.ss_protocol_ver | <code>number</code> | SS protocol version |
| data.ss_online_sta | <code>string</code> | SS online status |
| data.gps | <code>number</code> | GPS signal strength |
| data.gsm | <code>number</code> | GSM signal strength |
| data.lastTrack | <code>Object</code> | Last track information |
| data.lastTrack.ridingTime | <code>number</code> | Riding time in s |
| data.lastTrack.distance | <code>number</code> | Distance in m |
| data.lastTrack.time | <code>number</code> | Timestamp in unix timestamp epoch format (13 digits) |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="Tracks"></a>

## Tracks : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.items | <code>Array.&lt;Object&gt;</code> | Track items array |
| data.items.id | <code>string</code> | Identification number |
| data.items.trackId | <code>string</code> | Track identification number |
| data.items.startTime | <code>number</code> | Start time in unix timestamp epoch format (13 digits) |
| data.items.endTime | <code>number</code> | Stop time in unix timestamp epoch format (13 digits) |
| data.items.distance | <code>number</code> | Distance in m |
| data.items.avespeed | <code>number</code> | Average speed in km/h |
| data.items.ridingtime | <code>number</code> | Riding time in minutes |
| data.items.type | <code>string</code> | Type |
| data.items.date | <code>string</code> | Date in the format yyyymmdd |
| data.items.startPoint | <code>Object</code> | Start point |
| data.items.startPoint.lng | <code>string</code> | Longitude in decimal degree (WGS 84) |
| data.items.startPoint.lat | <code>string</code> | Latitude in decimal degree (WGS 84) |
| data.items.lastPoint | <code>Object</code> | Start point |
| data.items.lastPoint.lng | <code>string</code> | Longitude in decimal degree (WGS 84) |
| data.items.lastPoint.lat | <code>string</code> | Latitude in decimal degree (WGS 84) |
| data.items.track_thumb | <code>string</code> | URL to maps thumbnail |
| data.items.power_consumption | <code>number</code> | Power consumption |
| data.items.meet_count | <code>number</code> | Meet count |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="FirmwareVersion"></a>

## FirmwareVersion : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.nowVersion | <code>string</code> | Current version |
| data.version | <code>string</code> | Current version |
| data.hardVersion | <code>string</code> | Current hard version |
| data.ss_protocol_ver | <code>number</code> | ? |
| data.byteSize | <code>string</code> | Byte size |
| data.date | <code>number</code> | Date |
| data.isSupportUpdate | <code>boolean</code> | Is the update mechanism supported? |
| data.needUpdate | <code>boolean</code> | Is update necessary? |
| data.otaDescribe | <code>string</code> | Over the air update description |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |

<a name="UpdateInfo"></a>

## UpdateInfo : <code>Promise</code>
**Kind**: global typedef  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| client | [<code>Client</code>](#niuCloudConnector.Client) | Client |
| result | <code>Object</code> | Received response |
| data | <code>Object</code> | Response data |
| data.csq | <code>number</code> | ? |
| data.centreCtrlBattery | <code>string</code> | Centre control battery |
| data.date | <code>number</code> | Current hard version |
| result.desc | <code>string</code> | Response status description |
| result.trace | <code>string</code> | For debug purposes |
| result.status | <code>number</code> | Response status number |


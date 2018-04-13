<a id="vscp"></a>
## vscp : <code>object</code>
Namespace for all functionality of the VSCP provided libraries.

**Kind**: global namespace  

* [vscp](#vscp) : <code>object</code>
  * [.Event](#vscp.Event)
    * [new vscp.Event(options)](#new_vscp.Event_new)
    * [.vscpHead](#vscp.Event+vscpHead) : <code>number</code>
    * [.vscpClass](#vscp.Event+vscpClass) : <code>number</code>
    * [.vscpType](#vscp.Event+vscpType) : <code>number</code>
    * [.vscpObId](#vscp.Event+vscpObId) : <code>number</code>
    * [.vscpTimeStamp](#vscp.Event+vscpTimeStamp) : <code>number</code>
    * [.vscpDateTime](#vscp.Event+vscpDateTime) : <code>date</code>
    * [.vscpGuid](#vscp.Event+vscpGuid) : <code>string</code>
    * [.vscpData](#vscp.Event+vscpData) : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
    * [.setIPV6Addr()](#vscp.Event+setIPV6Addr)
    * [.isIPV6Addr()](#vscp.Event+isIPV6Addr) ⇒ <code>boolean</code>
    * [.setDumbNode()](#vscp.Event+setDumbNode)
    * [.isDumbNode()](#vscp.Event+isDumbNode) ⇒ <code>boolean</code>
    * [.setPriority(priority)](#vscp.Event+setPriority)
    * [.getPriority()](#vscp.Event+getPriority) ⇒ <code>number</code>
    * [.setHardCodedAddr()](#vscp.Event+setHardCodedAddr)
    * [.isHardCodedAddr()](#vscp.Event+isHardCodedAddr) ⇒ <code>boolean</code>
    * [.setDoNotCalcCRC()](#vscp.Event+setDoNotCalcCRC)
    * [.isDoNotCalcCRC()](#vscp.Event+isDoNotCalcCRC) ⇒ <code>boolean</code>
    * [.getText()](#vscp.Event+getText) ⇒ <code>string</code>
  * [.version](#vscp.version)
  * [.constants](#vscp.constants) : <code>object</code>
    * [.classes](#vscp.constants.classes) : <code>enum</code>
    * [.types](#vscp.constants.types) : <code>enum</code>
    * [.priorities](#vscp.constants.priorities) : <code>enum</code>
    * [.varTypes](#vscp.constants.varTypes) : <code>enum</code>
    * [.varTypeNames](#vscp.constants.varTypeNames)
  * [.utility](#vscp.utility) : <code>object</code>
    * [.readValue(input)](#vscp.utility.readValue) ⇒ <code>number</code>
    * [.getTime()](#vscp.utility.getTime) ⇒ <code>string</code>
    * [.guidToStr(guid)](#vscp.utility.guidToStr) ⇒ <code>string</code>
    * [.strToGuid(guid)](#vscp.utility.strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
    * [.getNodeId(guid)](#vscp.utility.getNodeId) ⇒ <code>number</code>
  * [.rest](#vscp.rest) : <code>object</code>
    * [.Client](#vscp.rest.Client)
      * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
      * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
      * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
      * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
      * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
      * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
      * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
      * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
      * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
      * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
      * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
      * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
      * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
      * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
      * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
      * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
      * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
      * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
      * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
      * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>
  * [.ws](#vscp.ws) : <code>object</code>
    * [.Client](#vscp.ws.Client)
      * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
      * _instance_
        * [.states](#vscp.ws.Client+states) : <code>enum</code>
        * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
        * [.socket](#vscp.ws.Client+socket) : <code>object</code>
        * [.url](#vscp.ws.Client+url) : <code>string</code>
        * [.userName](#vscp.ws.Client+userName) : <code>string</code>
        * [.userId](#vscp.ws.Client+userId) : <code>number</code>
        * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
        * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
        * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
        * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
        * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
        * [.password](#vscp.ws.Client+password) : <code>string</code>
        * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
        * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
        * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
        * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
        * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
        * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
        * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
        * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
        * [.state](#vscp.ws.Client+state) : <code>number</code>
        * [.substate](#vscp.ws.Client+substate) : <code>number</code>
        * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
        * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
        * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
        * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
        * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
        * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
        * [.signalConnError()](#vscp.ws.Client+signalConnError)
        * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
        * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
        * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
        * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
        * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
        * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
        * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
        * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
        * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
        * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
        * [.connect(options)](#vscp.ws.Client+connect)
        * [.disconnect()](#vscp.ws.Client+disconnect)
        * [.start(options)](#vscp.ws.Client+start)
        * [.stop(options)](#vscp.ws.Client+stop)
        * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
        * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
        * [.setFilter(options)](#vscp.ws.Client+setFilter)
        * [.createVar(options)](#vscp.ws.Client+createVar)
        * [.readVar(options)](#vscp.ws.Client+readVar)
        * [.writeVar(options)](#vscp.ws.Client+writeVar)
        * [.resetVar(options)](#vscp.ws.Client+resetVar)
        * [.removeVar(options)](#vscp.ws.Client+removeVar)
        * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
        * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
        * [.listVar(options)](#vscp.ws.Client+listVar)
        * [.readTable(options)](#vscp.ws.Client+readTable)
      * _inner_
        * [~Command](#vscp.ws.Client..Command)
          * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
          * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
          * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
          * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
        * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
        * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>
  * [._createNS(namespace)](#vscp._createNS)
  * [.getVarTypeName(n)](#vscp.getVarTypeName) ⇒ <code>string</code>
  * [.getVarTypeNumerical(str)](#vscp.getVarTypeNumerical) ⇒ <code>number</code>
  * [.getEditorModeFromType(n)](#vscp.getEditorModeFromType) ⇒ <code>string</code>
  * [.b64EncodeUnicode(str)](#vscp.b64EncodeUnicode) ⇒ <code>string</code>
  * [.b64DecodeUnicode(str)](#vscp.b64DecodeUnicode) ⇒ <code>string</code>
  * [.isBase64Type(type)](#vscp.isBase64Type) ⇒ <code>bool</code>
  * [.decodeValueIfBase64(type, value)](#vscp.decodeValueIfBase64) ⇒ <code>string</code>
  * [.encodeValueIfBase64(type, value)](#vscp.encodeValueIfBase64) ⇒ <code>string</code>

<a id="vscp.Event"></a>
### vscp.Event
**Kind**: static class of <code>[vscp](#vscp)</code>  

* [.Event](#vscp.Event)
  * [new vscp.Event(options)](#new_vscp.Event_new)
  * [.vscpHead](#vscp.Event+vscpHead) : <code>number</code>
  * [.vscpClass](#vscp.Event+vscpClass) : <code>number</code>
  * [.vscpType](#vscp.Event+vscpType) : <code>number</code>
  * [.vscpObId](#vscp.Event+vscpObId) : <code>number</code>
  * [.vscpTimeStamp](#vscp.Event+vscpTimeStamp) : <code>number</code>
  * [.vscpDateTime](#vscp.Event+vscpDateTime) : <code>date</code>
  * [.vscpGuid](#vscp.Event+vscpGuid) : <code>string</code>
  * [.vscpData](#vscp.Event+vscpData) : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
  * [.setIPV6Addr()](#vscp.Event+setIPV6Addr)
  * [.isIPV6Addr()](#vscp.Event+isIPV6Addr) ⇒ <code>boolean</code>
  * [.setDumbNode()](#vscp.Event+setDumbNode)
  * [.isDumbNode()](#vscp.Event+isDumbNode) ⇒ <code>boolean</code>
  * [.setPriority(priority)](#vscp.Event+setPriority)
  * [.getPriority()](#vscp.Event+getPriority) ⇒ <code>number</code>
  * [.setHardCodedAddr()](#vscp.Event+setHardCodedAddr)
  * [.isHardCodedAddr()](#vscp.Event+isHardCodedAddr) ⇒ <code>boolean</code>
  * [.setDoNotCalcCRC()](#vscp.Event+setDoNotCalcCRC)
  * [.isDoNotCalcCRC()](#vscp.Event+isDoNotCalcCRC) ⇒ <code>boolean</code>
  * [.getText()](#vscp.Event+getText) ⇒ <code>string</code>

<a id="new_vscp.Event_new"></a>
#### new vscp.Event(options)
VSCP event.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.vscpHead | <code>number</code> | Event head |
| options.guidIsIpV6Addr | <code>boolean</code> | GUID is a IPv6 address |
| options.dumpNode | <code>boolean</code> | Node is a dump node |
| options.vscpPriority | <code>number</code> | Priority |
| options.vscpHardCoded | <code>boolean</code> | Hard coded node id |
| options.vscpCalcCRC | <code>boolean</code> | Calculate CRC |
| options.vscpClass | <code>number</code> | VSCP class |
| options.vscpType | <code>number</code> | VSCP type |
| options.vscpObId | <code>number</code> | Object id |
| options.vscpTimeStamp | <code>number</code> | Timestamp |
| options.vscpGuid | <code>string</code> | GUID string |
| options.vscpData | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | Event data |

<a id="vscp.Event+vscpHead"></a>
#### event.vscpHead : <code>number</code>
VSCP event head

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpClass"></a>
#### event.vscpClass : <code>number</code>
VSCP class

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpType"></a>
#### event.vscpType : <code>number</code>
VSCP type

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpObId"></a>
#### event.vscpObId : <code>number</code>
VSCP object id used by driver for channel info and etc.

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpTimeStamp"></a>
#### event.vscpTimeStamp : <code>number</code>
Relative timestamp for package in us

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpDateTime"></a>
#### event.vscpDateTime : <code>date</code>
Date/Time for package

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpGuid"></a>
#### event.vscpGuid : <code>string</code>
Node global unique id LSB(15) -> MSB(0)

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpData"></a>
#### event.vscpData : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
Data array or string

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+setIPV6Addr"></a>
#### event.setIPV6Addr()
Set GUID as IP v6 address

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isIPV6Addr"></a>
#### event.isIPV6Addr() ⇒ <code>boolean</code>
Is GUID a IP v6 address or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the GUID is a IP v6 address, it will return true, otherwise false.  
<a id="vscp.Event+setDumbNode"></a>
#### event.setDumbNode()
Set dumb node. No MDF, registers, nothing.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isDumbNode"></a>
#### event.isDumbNode() ⇒ <code>boolean</code>
Is node a dump node or not?
Dumb node means no MDF, registers, nothing.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the node is a dumb node, it will return true, otherwise false.  
<a id="vscp.Event+setPriority"></a>
#### event.setPriority(priority)
Set the VSCP event priority.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  

| Param | Type | Description |
| --- | --- | --- |
| priority | <code>number</code> | Priority |

<a id="vscp.Event+getPriority"></a>
#### event.getPriority() ⇒ <code>number</code>
Get the VSCP event priority.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>number</code> - Priority of the event.  
<a id="vscp.Event+setHardCodedAddr"></a>
#### event.setHardCodedAddr()
Set the node id of the event sender as hard coded?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isHardCodedAddr"></a>
#### event.isHardCodedAddr() ⇒ <code>boolean</code>
Is the node id of the event sender hard coded or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the node id is hard coded, it will return true, otherwise false.  
<a id="vscp.Event+setDoNotCalcCRC"></a>
#### event.setDoNotCalcCRC()
Set flag for no CRC calculation?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isDoNotCalcCRC"></a>
#### event.isDoNotCalcCRC() ⇒ <code>boolean</code>
Is CRC calculated or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If nor CRC should be calculated true is returned.  
<a id="vscp.Event+getText"></a>
#### event.getText() ⇒ <code>string</code>
Get event as string.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>string</code> - Event as string  
<a id="vscp.version"></a>
### vscp.version
VSCP websocket library version

**Kind**: static property of <code>[vscp](#vscp)</code>  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| major | <code>number</code> | Major version number |
| minor | <code>number</code> | Minor version number |
| patch | <code>number</code> | Sub-minor version number |

<a id="vscp.constants"></a>
### vscp.constants : <code>object</code>
VSCP constants

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.constants](#vscp.constants) : <code>object</code>
  * [.classes](#vscp.constants.classes) : <code>enum</code>
  * [.types](#vscp.constants.types) : <code>enum</code>
  * [.priorities](#vscp.constants.priorities) : <code>enum</code>
  * [.varTypes](#vscp.constants.varTypes) : <code>enum</code>
  * [.varTypeNames](#vscp.constants.varTypeNames)

<a id="vscp.constants.classes"></a>
#### constants.classes : <code>enum</code>
VSCP classes

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| VSCP_CLASS1_PROTOCOL | <code>number</code> | <code>0</code> | 
| VSCP_CLASS1_ALARM | <code>number</code> | <code>1</code> | 
| VSCP_CLASS1_SECURITY | <code>number</code> | <code>2</code> | 
| VSCP_CLASS1_MEASUREMENT | <code>number</code> | <code>10</code> | 
| VSCP_CLASS1_DATA | <code>number</code> | <code>15</code> | 
| VSCP_CLASS1_INFORMATION | <code>number</code> | <code>20</code> | 
| VSCP_CLASS1_CONTROL | <code>number</code> | <code>30</code> | 
| VSCP_CLASS1_MULTIMEDIA | <code>number</code> | <code>40</code> | 
| VSCP_CLASS1_AOL | <code>number</code> | <code>50</code> | 
| VSCP_CLASS1_MEASUREMENT64 | <code>number</code> | <code>60</code> | 
| VSCP_CLASS1_MEASUREZONE | <code>number</code> | <code>65</code> | 
| VSCP_CLASS1_MEASUREMENT32 | <code>number</code> | <code>70</code> | 
| VSCP_CLASS1_SETVALUEZONE | <code>number</code> | <code>85</code> | 
| VSCP_CLASS1_WEATHER | <code>number</code> | <code>90</code> | 
| VSCP_CLASS1_WEATHER_FORECAST | <code>number</code> | <code>95</code> | 
| VSCP_CLASS1_PHONE | <code>number</code> | <code>100</code> | 
| VSCP_CLASS1_LIN | <code>number</code> | <code>101</code> | 
| VSCP_CLASS1_DISPLAY | <code>number</code> | <code>102</code> | 
| VSCP_CLASS1_REMOTE | <code>number</code> | <code>110</code> | 
| VSCP_CLASS1_GPS | <code>number</code> | <code>206</code> | 
| VSCP_CLASS1_WIRELESS | <code>number</code> | <code>212</code> | 
| VSCP_CLASS1_DIAGNOSTIC | <code>number</code> | <code>506</code> | 
| VSCP_CLASS1_ERROR | <code>number</code> | <code>508</code> | 
| VSCP_CLASS1_LOG | <code>number</code> | <code>509</code> | 
| VSCP_CLASS1_LAB | <code>number</code> | <code>510</code> | 
| VSCP_CLASS1_LOCAL | <code>number</code> | <code>511</code> | 
| VSCP_CLASS2_LEVEL1_PROTOCOL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_ALARM | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_SECURITY | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_DATA | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_INFORMATION | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_CONTROL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MULTIMEDIA | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_AOL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT64 | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREZONE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT32 | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_SETVALUEZONE | <code>number</code> | <code></code> | 
| VSCP_CLASS1_LEVEL1_WEATHER | <code>number</code> | <code>90</code> | 
| VSCP_CLASS1_LEVEL1_WEATHER_FORECAST | <code>number</code> | <code>95</code> | 
| VSCP_CLASS2_LEVEL1_PHONE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_REMOTE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_GPS | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_WIRELESS | <code>number</code> | <code></code> | 
| VSCP_CLASS1_LEVEL1_DIAGNOSTIC | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LOG | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LAB | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LOCAL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_PROTOCOL | <code>number</code> | <code>1024</code> | 
| VSCP_CLASS2_CONTROL | <code>number</code> | <code>1025</code> | 
| VSCP_CLASS2_INFORMATION | <code>number</code> | <code>1026</code> | 
| VSCP_CLASS2_TEXT2SPEECH | <code>number</code> | <code>1028</code> | 
| VSCP_CLASS2_CUSTOM | <code>number</code> | <code>1029</code> | 
| VSCP_CLASS2_DISPLAY | <code>number</code> | <code>1030</code> | 
| VSCP_CLASS2_MEASUREMENT_STR | <code>number</code> | <code>1040</code> | 
| VSCP_CLASS2_MEASUREMENT_FLOAT | <code>number</code> | <code>1060</code> | 
| VSCP_CLASS2_VSCPD | <code>number</code> | <code>65535</code> | 

<a id="vscp.constants.types"></a>
#### constants.types : <code>enum</code>
VSCP class types

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| VSCP_TYPE_UNDEFINED | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_PROTOCOL_SEGCTRL_HEARTBEAT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_PROTOCOL_NEW_NODE_ONLINE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_PROTOCOL_PROBE_ACK | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_PROTOCOL_SET_NICKNAME | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_PROTOCOL_NICKNAME_ACCEPTED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_PROTOCOL_DROP_NICKNAME | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_PROTOCOL_READ_REGISTER | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_PROTOCOL_RW_RESPONSE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_PROTOCOL_WRITE_REGISTER | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_PROTOCOL_ENTER_BOOT_LOADER | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_PROTOCOL_ACK_BOOT_LOADER | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_PROTOCOL_NACK_BOOT_LOADER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA_ACK | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA_NACK | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA_ACK | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA_NACK | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_PROTOCOL_RESET_DEVICE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_PROTOCOL_PAGE_READ | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_PROTOCOL_PAGE_WRITE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_PROTOCOL_RW_PAGE_RESPONSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_PROTOCOL_HIGH_END_SERVER_PROBE | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_PROTOCOL_HIGH_END_SERVER_RESPONSE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_PROTOCOL_INCREMENT_REGISTER | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_PROTOCOL_DECREMENT_REGISTER | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_PROTOCOL_WHO_IS_THERE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_PROTOCOL_WHO_IS_THERE_RESPONSE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_PROTOCOL_GET_MATRIX_INFO | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_PROTOCOL_GET_MATRIX_INFO_RESPONSE | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_PROTOCOL_GET_EMBEDDED_MDF | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_PROTOCOL_GET_EMBEDDED_MDF_RESPONSE | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_READ | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_WRITE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_RESPONSE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_PROTOCOL_GET_EVENT_INTEREST | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_PROTOCOL_GET_EVENT_INTEREST_RESPONSE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE_ACK | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE_NACK | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK_ACK | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK_NACK | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_ALARM_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_ALARM_WARNING | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_ALARM_ALARM | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_ALARM_SOUND | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_ALARM_LIGHT | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_ALARM_POWER | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_STOP | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_PAUSE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_RESET | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_RESUME | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_ALARM_ARM | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_ALARM_DISARM | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SECURITY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_SECURITY_MOTION | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_SECURITY_GLASS_BREAK | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_SECURITY_BEAM_BREAK | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_SECURITY_SENSOR_TAMPER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_SECURITY_SHOCK_SENSOR | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_SECURITY_SMOKE_SENSOR | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_SECURITY_HEAT_SENSOR | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_SECURITY_PANIC_SWITCH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_SECURITY_DOOR_OPEN | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_SECURITY_WINDOW_OPEN | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_SECURITY_CO_SENSOR | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SECURITY_FROST_DETECTED | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_SECURITY_FLAME_DETECTED | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_SECURITY_OXYGEN_LOW | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_SECURITY_WEIGHT_DETECTED | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_SECURITY_WATER_DETECTED | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_SECURITY_CONDENSATION_DETECTED | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_SECURITY_SOUND_DETECTED | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_SECURITY_HARMFUL_SOUND_LEVEL | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_SECURITY_TAMPER | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_RESISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_DATA_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DATA_IO | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DATA_AD | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DATA_DA | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DATA_RELATIVE_STRENGTH | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DATA_SIGNAL_LEVEL | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DATA_SIGNAL_QUALITY | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_INFORMATION_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_INFORMATION_BUTTON | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_INFORMATION_MOUSE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_INFORMATION_ON | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_INFORMATION_OFF | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_INFORMATION_ALIVE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_INFORMATION_TERMINATING | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_INFORMATION_OPENED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_INFORMATION_CLOSED | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_INFORMATION_NODE_HEARTBEAT | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_INFORMATION_BELOW_LIMIT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_INFORMATION_ABOVE_LIMIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_INFORMATION_PULSE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_INFORMATION_ERROR | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_INFORMATION_RESUMED | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_INFORMATION_PAUSED | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_INFORMATION_SLEEP | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_INFORMATION_GOOD_MORNING | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_INFORMATION_GOOD_DAY | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_INFORMATION_GOOD_AFTERNOON | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_INFORMATION_GOOD_EVENING | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_INFORMATION_GOOD_NIGHT | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_INFORMATION_SEE_YOU_SOON | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_INFORMATION_GOODBYE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_INFORMATION_STOP | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_INFORMATION_START | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_INFORMATION_RESET_COMPLETED | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_INFORMATION_INTERRUPTED | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_INFORMATION_PREPARING_TO_SLEEP | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_INFORMATION_WOKEN_UP | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_INFORMATION_DUSK | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_INFORMATION_DAWN | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_INFORMATION_ACTIVE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_INFORMATION_INACTIVE | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_INFORMATION_BUSY | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_INFORMATION_IDLE | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_INFORMATION_STREAM_DATA | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_INFORMATION_TOKEN_ACTIVITY | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_INFORMATION_STREAM_DATA_WITH_ZONE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_INFORMATION_CONFIRM | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_INFORMATION_LEVEL_CHANGED | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_INFORMATION_WARNING | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_INFORMATION_STATE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_INFORMATION_ACTION_TRIGGER | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_INFORMATION_SUNRISE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_INFORMATION_SUNSET | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_INFORMATION_START_OF_RECORD | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_INFORMATION_END_OF_RECORD | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_INFORMATION_PRESET_ACTIVE | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_INFORMATION_DETECT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_INFORMATION_OVERFLOW | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_INFORMATION_BIG_LEVEL_CHANGED | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_INFORMATION_SUNRISE_TWILIGHT_START | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_INFORMATION_SUNSET_TWILIGHT_START | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_INFORMATION_NAUTICAL_SUNRISE_TWILIGHT_START | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_INFORMATION_NAUTICAL_SUNSET_TWILIGHT_START | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_INFORMATION_ASTRONOMICAL_SUNRISE_TWILIGHT_START | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_INFORMATION_ASTRONOMICAL_SUNSET_TWILIGHT_START | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_INFORMATION_CALCULATED_NOON | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_UP | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_DOWN | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_LEFT | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_RIGHT | <code>number</code> | <code>62</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_TOP | <code>number</code> | <code>63</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_BOTTOM | <code>number</code> | <code>64</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_MIDDLE | <code>number</code> | <code>65</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_PRESET | <code>number</code> | <code>66</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_LEFT | <code>number</code> | <code>67</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_RIGHT | <code>number</code> | <code>68</code> | 
| VSCP_TYPE_INFORMATION_LONG_CLICK | <code>number</code> | <code>69</code> | 
| VSCP_TYPE_INFORMATION_SINGLE_CLICK | <code>number</code> | <code>70</code> | 
| VSCP_TYPE_INFORMATION_DOUBLE_CLICK | <code>number</code> | <code>71</code> | 
| VSCP_TYPE_INFORMATION_DATE | <code>number</code> | <code>72</code> | 
| VSCP_TYPE_INFORMATION_TIME | <code>number</code> | <code>73</code> | 
| VSCP_TYPE_INFORMATION_WEEKDAY | <code>number</code> | <code>74</code> | 
| VSCP_TYPE_INFORMATION_LOCK | <code>number</code> | <code>75</code> | 
| VSCP_TYPE_INFORMATION_UNLOCK | <code>number</code> | <code>76</code> | 
| VSCP_TYPE_CONTROL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_CONTROL_MUTE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_CONTROL_OPEN | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_CONTROL_CLOSE | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_CONTROL_TURNON | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_CONTROL_TURNOFF | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_CONTROL_START | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_CONTROL_STOP | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_CONTROL_RESET | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_CONTROL_INTERRUPT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_CONTROL_SLEEP | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_CONTROL_WAKEUP | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_CONTROL_RESUME | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_CONTROL_PAUSE | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_CONTROL_ACTIVATE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_CONTROL_DEACTIVATE | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_CONTROL_DIM_LAMPS | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_CONTROL_CHANGE_CHANNEL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_CONTROL_CHANGE_LEVEL | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_CONTROL_RELATIVE_CHANGE_LEVEL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_CONTROL_MEASUREMENT_REQUEST | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_CONTROL_STREAM_DATA | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_CONTROL_SYNC | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_CONTROL_ZONED_STREAM_DATA | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_CONTROL_SET_PRESET | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_CONTROL_TOGGLE_STATE | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_CONTROL_TIMED_PULSE_ON | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_CONTROL_TIMED_PULSE_OFF | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_CONTROL_SET_COUNTRY_LANGUAGE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_CONTROL_BIG_CHANGE_LEVEL | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_UP | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_DOWN | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_LEFT | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_RIGHT | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_MIDDLE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_PRESET | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS_ON | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS_OFF | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_CONTROL_LOCK | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_CONTROL_UNLOCK | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MULTIMEDIA_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MULTIMEDIA_PLAYBACK | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MULTIMEDIA_NAVIGATOR_KEY_ENG | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_CONTRAST | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_FOCUS | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_TINT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_COLOUR_BALANCE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_BRIGHTNESS | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_HUE | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_BASS | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_TREBLE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_MASTER_VOLUME | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_FRONT_VOLUME | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_CENTRE_VOLUME | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_REAR_VOLUME | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SIDE_VOLUME | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_DISK | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_TRACK | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_ALBUM | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_CHANNEL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_PAGE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_CHAPTER | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_SCREEN_FORMAT | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_INPUT_SOURCE | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_OUTPUT | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MULTIMEDIA_RECORD | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MULTIMEDIA_SET_RECORDING_VOLUME | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MULTIMEDIA_TIVO_FUNCTION | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MULTIMEDIA_GET_CURRENT_TITLE | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MULTIMEDIA_SET_POSITION | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MULTIMEDIA_GET_MEDIA_INFO | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MULTIMEDIA_REMOVE_ITEM | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MULTIMEDIA_REMOVE_ALL_ITEMS | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MULTIMEDIA_SAVE_ALBUM | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MULTIMEDIA_CONTROL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MULTIMEDIA_CONTROL_RESPONSE | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_AOL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_AOL_UNPLUGGED_POWER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_AOL_UNPLUGGED_LAN | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_AOL_CHASSIS_INTRUSION | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_AOL_PROCESSOR_REMOVAL | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_AOL_ENVIRONMENT_ERROR | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_AOL_HIGH_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_AOL_FAN_SPEED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_AOL_VOLTAGE_FLUCTUATIONS | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_AOL_OS_ERROR | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_AOL_POWER_ON_ERROR | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_AOL_SYSTEM_HUNG | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_AOL_COMPONENT_FAILURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_AOL_REBOOT_UPON_FAILURE | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_AOL_REPAIR_OPERATING_SYSTEM | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_AOL_UPDATE_BIOS_IMAGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_AOL_UPDATE_DIAGNOSTIC_PROCEDURE | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT64_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT64_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT64_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT64_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT64_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT64_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT64_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT64_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT64_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT64_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT64_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT64_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT64_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT64_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT64_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT64_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT64_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT64_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT64_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT64_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT64_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT64_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT64_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT64_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT64_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT64_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT64_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT64_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT64_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT64_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT64_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT64_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT64_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT64_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT64_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT64_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT64_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT64_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT64_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT64_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MEASUREZONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREZONE_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREZONE_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREZONE_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREZONE_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREZONE_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREZONE_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREZONE_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREZONE_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREZONE_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREZONE_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREZONE_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREZONE_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREZONE_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREZONE_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREZONE_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREZONE_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREZONE_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREZONE_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREZONE_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREZONE_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREZONE_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREZONE_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREZONE_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREZONE_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREZONE_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREZONE_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREZONE_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREZONE_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREZONE_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREZONE_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREZONE_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREZONE_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREZONE_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREZONE_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREZONE_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREZONE_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREZONE_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREZONE_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREZONE_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREZONE_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREZONE_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREZONE_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREZONE_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MEASUREMENT32_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT32_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT32_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT32_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT32_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT32_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT32_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT32_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT32_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT32_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT32_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT32_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT32_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT32_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT32_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT32_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT32_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT32_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT32_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT32_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT32_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT32_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT32_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT32_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT32_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT32_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT32_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT32_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT32_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT32_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT32_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT32_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT32_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT32_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT32_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT32_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT32_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT32_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT32_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT32_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_SETVALUEZONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_SETVALUEZONE_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_SETVALUEZONE_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_SETVALUEZONE_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_SETVALUEZONE_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_SETVALUEZONE_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_SETVALUEZONE_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_SETVALUEZONE_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_SETVALUEZONE_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_SETVALUEZONE_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SETVALUEZONE_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_SETVALUEZONE_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_SETVALUEZONE_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_SETVALUEZONE_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_SETVALUEZONE_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_SETVALUEZONE_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_SETVALUEZONE_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_SETVALUEZONE_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_SETVALUEZONE_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_SETVALUEZONE_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_SETVALUEZONE_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_SETVALUEZONE_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_SETVALUEZONE_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_SETVALUEZONE_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_SETVALUEZONE_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_SETVALUEZONE_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_SETVALUEZONE_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_SETVALUEZONE_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_SETVALUEZONE_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_SETVALUEZONE_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_SETVALUEZONE_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_SETVALUEZONE_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_SETVALUEZONE_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_SETVALUEZONE_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_SETVALUEZONE_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_SETVALUEZONE_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_SETVALUEZONE_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_SETVALUEZONE_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_SETVALUEZONE_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_SETVALUEZONE_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_WEATHER_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WEATHER_SEASONS_WINTER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_WEATHER_SEASONS_SPRING | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WEATHER_SEASONS_SUMMER | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_WEATHER_SEASONS_AUTUMN | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_WEATHER_WIND_NONE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_WEATHER_WIND_LOW | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_WEATHER_WIND_MEDIUM | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_WEATHER_WIND_HIGH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_WEATHER_WIND_VERY_HIGH | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_WEATHER_AIR_FOGGY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_WEATHER_AIR_FREEZING | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_WEATHER_AIR_VERY_COLD | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_WEATHER_AIR_COLD | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_WEATHER_AIR_NORMAL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_WEATHER_AIR_HOT | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_WEATHER_AIR_VERY_HOT | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_LOW | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_MEDIUM | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_HIGH | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_WEATHER_AIR_HUMID | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_WEATHER_AIR_DRY | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_WEATHER_SOIL_HUMID | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_WEATHER_SOIL_DRY | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_WEATHER_RAIN_NONE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_WEATHER_RAIN_LIGHT | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_WEATHER_RAIN_HEAVY | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_WEATHER_RAIN_VERY_HEAVY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_WEATHER_SUN_NONE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_WEATHER_SUN_LIGHT | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_WEATHER_SUN_HEAVY | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_WEATHER_SNOW_NONE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_WEATHER_SNOW_LIGHT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_WEATHER_SNOW_HEAVY | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_WEATHER_DEW_POINT | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_WEATHER_STORM | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_WEATHER_FLOOD | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_WEATHER_EARTHQUAKE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_WEATHER_NUCLEAR_DISASTER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_WEATHER_FIRE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_WEATHER_LIGHTNING | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_LOW | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_MEDIUM | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_NORMAL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_HIGH | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_VERY_HIGH | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL1 | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL2 | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL3 | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL4 | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL5 | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_WEATHER_ARMAGEDON | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_WEATHER_FORECAST_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_WINTER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_SPRING | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_SUMMER | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_AUTUMN | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_NONE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_LOW | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_MEDIUM | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_HIGH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_VERY_HIGH | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_FOGGY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_FREEZING | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_VERY_COLD | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_COLD | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_NORMAL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_HOT | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_VERY_HOT | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_LOW | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_MEDIUM | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_HIGH | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_HUMID | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_DRY | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SOIL_HUMID | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SOIL_DRY | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_NONE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_LIGHT | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_HEAVY | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_VERY_HEAVY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_NONE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_LIGHT | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_HEAVY | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_NONE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_LIGHT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_HEAVY | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_WEATHER_FORECAST_DEW_POINT | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_WEATHER_FORECAST_STORM | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_WEATHER_FORECAST_FLOOD | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_WEATHER_FORECAST_EARTHQUAKE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_WEATHER_FORECAST_NUCLEAR_DISASTER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_WEATHER_FORECAST_FIRE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_WEATHER_FORECAST_LIGHTNING | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_LOW | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_MEDIUM | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_NORMAL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_HIGH | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_VERY_HIGH | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL1 | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL2 | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL3 | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL4 | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL5 | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_WEATHER_FORECAST_ARMAGEDDON | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_PHONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_PHONE_INCOMING_CALL | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_PHONE_OUTGOING_CALL | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_PHONE_RING | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_PHONE_ANSWER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_PHONE_HANGUP | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_PHONE_GIVEUP | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_PHONE_TRANSFER | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_PHONE_DATABASE_INFO | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_DISPLAY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DISPLAY_CLEAR_DISPLAY | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DISPLAY_POSITION_CURSOR | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DISPLAY_WRITE_DISPLAY | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DISPLAY_WRITE_DISPLAY_BUFFER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DISPLAY_SHOW_DISPLAY_BUFFER | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DISPLAY_SET_DISPLAY_BUFFER_PARAM | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_DISPLAY_SHOW_TEXT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_DISPLAY_SHOW_LED | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_DISPLAY_SHOW_LED_COLOR | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_REMOTE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_REMOTE_RC5 | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_REMOTE_SONY12 | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_REMOTE_LIRC | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_REMOTE_VSCP | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_GPS_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_GPS_POSITION | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_GPS_SATELLITES | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WIRELESS_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WIRELESS_GSM_CELL | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DIAGNOSTIC_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERVOLTAGE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DIAGNOSTIC_UNDERVOLTAGE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DIAGNOSTIC_VBUS_LOW | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_LOW | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_FULL | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_ERROR | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_OK | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERCURRENT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_DIAGNOSTIC_CIRCUIT_ERROR | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_DIAGNOSTIC_SHORT_CIRCUIT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_DIAGNOSTIC_OPEN_CIRCUIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_DIAGNOSTIC_MOIST | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIRE_FAIL | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIRELESS_FAIL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_DIAGNOSTIC_IR_FAIL | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_DIAGNOSTIC_1WIRE_FAIL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS222_FAIL | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS232_FAIL | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS423_FAIL | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS485_FAIL | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_DIAGNOSTIC_CAN_FAIL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_DIAGNOSTIC_LAN_FAIL | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_DIAGNOSTIC_USB_FAIL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIFI_FAIL | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_DIAGNOSTIC_NFC_RFID_FAIL | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_DIAGNOSTIC_LOW_SIGNAL | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_DIAGNOSTIC_HIGH_SIGNAL | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_DIAGNOSTIC_ADC_FAIL | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_DIAGNOSTIC_ALU_FAIL | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_DIAGNOSTIC_ASSERT | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_DIAGNOSTIC_DAC_FAIL | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_DIAGNOSTIC_DMA_FAIL | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_DIAGNOSTIC_ETH_FAIL | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_DIAGNOSTIC_EXCEPTION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_DIAGNOSTIC_FPU_FAIL | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_DIAGNOSTIC_GPIO_FAIL | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_DIAGNOSTIC_I2C_FAIL | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_DIAGNOSTIC_I2S_FAIL | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_DIAGNOSTIC_INVALID_CONFIG | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_DIAGNOSTIC_MMU_FAIL | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_DIAGNOSTIC_NMI | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERHEAT | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_DIAGNOSTIC_PLL_FAIL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_DIAGNOSTIC_POR_FAIL | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_DIAGNOSTIC_PWM_FAIL | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_DIAGNOSTIC_RAM_FAIL | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_DIAGNOSTIC_ROM_FAIL | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_DIAGNOSTIC_SPI_FAIL | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_DIAGNOSTIC_STACK_FAIL | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_DIAGNOSTIC_LIN_FAIL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_DIAGNOSTIC_UART_FAIL | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_DIAGNOSTIC_UNHANDLED_INT | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_DIAGNOSTIC_MEMORY_FAIL | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_DIAGNOSTIC_VARIABLE_RANGE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_DIAGNOSTIC_WDT | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_DIAGNOSTIC_EEPROM_FAIL | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_DIAGNOSTIC_ENCRYPTION_FAIL | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_DIAGNOSTIC_BAD_USER_INPUT | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_DIAGNOSTIC_DECRYPTION_FAIL | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_DIAGNOSTIC_NOISE | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_DIAGNOSTIC_BOOTLOADER_FAIL | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_DIAGNOSTIC_PROGRAMFLOW_FAIL | <code>number</code> | <code>62</code> | 
| VSCP_TYPE_DIAGNOSTIC_RTC_FAIL | <code>number</code> | <code>63</code> | 
| VSCP_TYPE_DIAGNOSTIC_SYSTEM_TEST_FAIL | <code>number</code> | <code>64</code> | 
| VSCP_TYPE_DIAGNOSTIC_SENSOR_FAIL | <code>number</code> | <code>65</code> | 
| VSCP_TYPE_DIAGNOSTIC_SAFESTATE | <code>number</code> | <code>66</code> | 
| VSCP_TYPE_DIAGNOSTIC_SIGNAL_IMPLAUSIBLE | <code>number</code> | <code>67</code> | 
| VSCP_TYPE_DIAGNOSTIC_STORAGE_FAIL | <code>number</code> | <code>68</code> | 
| VSCP_TYPE_DIAGNOSTIC_SELFTEST_FAIL | <code>number</code> | <code>69</code> | 
| VSCP_TYPE_DIAGNOSTIC_ESD_EMC_EMI | <code>number</code> | <code>70</code> | 
| VSCP_TYPE_DIAGNOSTIC_TIMEOUT | <code>number</code> | <code>71</code> | 
| VSCP_TYPE_DIAGNOSTIC_LCD_FAIL | <code>number</code> | <code>72</code> | 
| VSCP_TYPE_DIAGNOSTIC_TOUCHPANEL_FAIL | <code>number</code> | <code>73</code> | 
| VSCP_TYPE_DIAGNOSTIC_NOLOAD | <code>number</code> | <code>74</code> | 
| VSCP_TYPE_DIAGNOSTIC_COOLING_FAIL | <code>number</code> | <code>75</code> | 
| VSCP_TYPE_DIAGNOSTIC_HEATING_FAIL | <code>number</code> | <code>76</code> | 
| VSCP_TYPE_DIAGNOSTIC_TX_FAIL | <code>number</code> | <code>77</code> | 
| VSCP_TYPE_DIAGNOSTIC_RX_FAIL | <code>number</code> | <code>78</code> | 
| VSCP_TYPE_DIAGNOSTIC_EXT_IC_FAIL | <code>number</code> | <code>79</code> | 
| VSCP_TYPE_ERROR_SUCCESS | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_ERROR_ERROR | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_ERROR_CHANNEL | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_ERROR_FIFO_EMPTY | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_ERROR_FIFO_FULL | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_ERROR_FIFO_SIZE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_ERROR_FIFO_WAIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_ERROR_GENERIC | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_ERROR_HARDWARE | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_ERROR_INIT_FAIL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_ERROR_INIT_MISSING | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_ERROR_INIT_READY | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_ERROR_NOT_SUPPORTED | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_ERROR_OVERRUN | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_ERROR_RCV_EMPTY | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_ERROR_REGISTER | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_ERROR_TRM_FULL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_ERROR_LIBRARY | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_ERROR_PROCADDRESS | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_ERROR_ONLY_ONE_INSTANCE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_ERROR_SUB_DRIVER | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_ERROR_TIMEOUT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_ERROR_NOT_OPEN | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_ERROR_PARAMETER | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_ERROR_MEMORY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_ERROR_INTERNAL | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_ERROR_COMMUNICATION | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_ERROR_USER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_ERROR_PASSWORD | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_ERROR_CONNECTION | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_ERROR_INVALID_HANDLE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_ERROR_OPERATION_FAILED | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_LOG_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_LOG_MESSAGE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_LOG_START | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_LOG_STOP | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_LOG_LEVEL | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_LABORATORY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_LOCAL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_PROTOCOL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_PROTOCOL_READ_REGISTER | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_PROTOCOL_WRITE_REGISTER | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_PROTOCOL_READ_WRITE_RESPONSE | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_PROTOCOL_HIGH_END_SERVER_CAPS | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_PROTOCOL_WHO_IS_THERE_RESPONE | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_CONTROL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_INFORMATION_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_INFORMATION_TOKEN_ACTIVITY | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_INFORMATION_HEART_BEAT | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_TEXT2SPEECH_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_TEXT2SPEECH_TALK | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_CUSTOM_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_DISPLAY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_COUNT | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MASS | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TIME | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FORCE | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_POWER | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_POSITION | <code>number</code> | <code>31</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPEED | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TENSION | <code>number</code> | <code>34</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FLOW | <code>number</code> | <code>36</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_AREA | <code>number</code> | <code>52</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_COUNT | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MASS | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TIME | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FORCE | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_POWER | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_POSITION | <code>number</code> | <code>31</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPEED | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TENSION | <code>number</code> | <code>34</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FLOW | <code>number</code> | <code>36</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_AREA | <code>number</code> | <code>52</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP2_TYPE_VSCPD_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_VSCPD_LOOP | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_VSCPD_PAUSE | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_VSCPD_ACTIVATE | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_VSCPD_SECOND | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_VSCPD_MINUTE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_VSCPD_HOUR | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_VSCPD_NOON | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_VSCPD_MIDNIGHT | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_VSCPD_WEEK | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_VSCPD_MONTH | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_VSCPD_QUARTER | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_VSCPD_YEAR | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_MINUTE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_HOUR | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_DAY | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_WEEK | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_MONTH | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_YEAR | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_VSCPD_DUSK | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_VSCPD_DAWN | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_VSCPD_STARTING_UP | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_VSCPD_SHUTTING_DOWN | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_VSCPD_TIMER_STARTED | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_VSCPD_TIMER_PAUSED | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_VSCPD_TIMER_RESUMED | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_VSCPD_TIMER_STOPPED | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_VSCPD_TIMER_ELLAPSED | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_VSCPD_NEW_CALCULATION | <code>number</code> | <code>30</code> | 

<a id="vscp.constants.priorities"></a>
#### constants.priorities : <code>enum</code>
VSCP class priorities

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| PRIORITY_0_HIGH | <code>number</code> | <code>0</code> | 
| PRIORITY_1 | <code>number</code> | <code>1</code> | 
| PRIORITY_2 | <code>number</code> | <code>2</code> | 
| PRIORITY_3_NORMAL | <code>number</code> | <code>3</code> | 
| PRIORITY_4 | <code>number</code> | <code>4</code> | 
| PRIORITY_5 | <code>number</code> | <code>5</code> | 
| PRIORITY_6 | <code>number</code> | <code>6</code> | 
| PRIORITY_7_LOW | <code>number</code> | <code>7</code> | 

<a id="vscp.constants.varTypes"></a>
#### constants.varTypes : <code>enum</code>
VSCP variable types

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| UNASSIGNED | <code>number</code> | <code>0</code> | 
| STRING | <code>number</code> | <code>1</code> | 
| BOOLEAN | <code>number</code> | <code>2</code> | 
| INTEGER | <code>number</code> | <code>3</code> | 
| LONG | <code>number</code> | <code>4</code> | 
| DOUBLE | <code>number</code> | <code>5</code> | 
| MEASUREMENT | <code>number</code> | <code>6</code> | 
| EVENT | <code>number</code> | <code>7</code> | 
| GUID | <code>number</code> | <code>8</code> | 
| EVENT_DATA | <code>number</code> | <code>9</code> | 
| EVENT_CLASS | <code>number</code> | <code>10</code> | 
| EVENT_TYPE | <code>number</code> | <code>11</code> | 
| EVENT_TIMESTAMP | <code>number</code> | <code>12</code> | 
| DATE_TIME | <code>number</code> | <code>13</code> | 
| DATE | <code>number</code> | <code>14</code> | 
| TIME | <code>number</code> | <code>15</code> | 
| BLOB | <code>number</code> | <code>16</code> | 
| MIME | <code>number</code> | <code>100</code> | 
| HTML | <code>number</code> | <code>101</code> | 
| JAVASCIPT | <code>number</code> | <code>102</code> | 
| JSON | <code>number</code> | <code>103</code> | 
| XML | <code>number</code> | <code>104</code> | 
| SQL | <code>number</code> | <code>105</code> | 
| LUA | <code>number</code> | <code>201</code> | 
| LUARES | <code>number</code> | <code>202</code> | 
| UXTYPE1 | <code>number</code> | <code>300</code> | 
| DMROW | <code>number</code> | <code>500</code> | 
| DRIVER | <code>number</code> | <code>501</code> | 
| USER | <code>number</code> | <code>502</code> | 
| FILTER | <code>number</code> | <code>503</code> | 

<a id="vscp.constants.varTypeNames"></a>
#### constants.varTypeNames
VSCP variable type names as string. Use to fill drop down boxes and similar.

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
<a id="vscp.utility"></a>
### vscp.utility : <code>object</code>
Utility functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.utility](#vscp.utility) : <code>object</code>
  * [.readValue(input)](#vscp.utility.readValue) ⇒ <code>number</code>
  * [.getTime()](#vscp.utility.getTime) ⇒ <code>string</code>
  * [.guidToStr(guid)](#vscp.utility.guidToStr) ⇒ <code>string</code>
  * [.strToGuid(guid)](#vscp.utility.strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
  * [.getNodeId(guid)](#vscp.utility.getNodeId) ⇒ <code>number</code>

<a id="vscp.utility.readValue"></a>
#### utility.readValue(input) ⇒ <code>number</code>
Read a hex or decimal value and return as an integer.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>number</code> - Value  

| Param | Type | Description |
| --- | --- | --- |
| input | <code>string</code> | Hex or decimal value as string |

<a id="vscp.utility.getTime"></a>
#### utility.getTime() ⇒ <code>string</code>
Utility function which returns the current time in the following format: hh:mm:ss.us

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>string</code> - Current time in the format hh:mm:ss.us  
<a id="vscp.utility.guidToStr"></a>
#### utility.guidToStr(guid) ⇒ <code>string</code>
Converts a GUID number array to a GUID string.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>string</code> - GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>Array.&lt;number&gt;</code> | GUID number array |

<a id="vscp.utility.strToGuid"></a>
#### utility.strToGuid(guid) ⇒ <code>Array.&lt;number&gt;</code>
Converts a GUID string to a GUID number array.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>Array.&lt;number&gt;</code> - GUID number array  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp.utility.getNodeId"></a>
#### utility.getNodeId(guid) ⇒ <code>number</code>
Get node id from a node GUID string.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>number</code> - Node id  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp.rest"></a>
### vscp.rest : <code>object</code>
VSCP REST api functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.rest](#vscp.rest) : <code>object</code>
  * [.Client](#vscp.rest.Client)
    * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
    * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
    * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
    * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
    * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
    * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
    * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
    * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
    * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
    * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
    * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
    * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
    * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
    * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>

<a id="vscp.rest.Client"></a>
#### rest.Client
**Kind**: static class of <code>[rest](#vscp.rest)</code>  

* [.Client](#vscp.rest.Client)
  * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
  * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
  * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
  * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
  * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
  * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
  * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
  * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
  * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
  * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
  * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
  * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
  * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
  * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
  * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
  * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
  * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
  * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
  * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
  * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>

<a id="new_vscp.rest.Client_new"></a>
##### new vscp.rest.Client(config)
The VSCP client class handles the basic REST api of the VSCP daemon.
The function interface uses jquery ajax call in the background and will
return object with the jquery promise interface.


| Param | Type | Description |
| --- | --- | --- |
| config | <code>string</code> | Configuration |
| [config.baseUrl] | <code>string</code> | VSCP daemon URL (protocol + hostname + port) |
| [options.pathPrefix] | <code>string</code> | Path prefix (default: '/vscp'), which comes right after the base url. |
| [options.apiVersion] | <code>string</code> | API version (for future use) |

<a id="vscp.rest.Client+baseUrl"></a>
##### client.baseUrl : <code>string</code>
Base URL

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+pathPrefix"></a>
##### client.pathPrefix : <code>string</code>
Path prefix

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+apiVersion"></a>
##### client.apiVersion : <code>string</code>
REST API version (future use)

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+sessionKey"></a>
##### client.sessionKey : <code>string</code>
Session key

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+_buildUrl"></a>
##### client._buildUrl(path) ⇒
Build complete URL, including command path.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: URL  

| Param | Type | Description |
| --- | --- | --- |
| path | <code>string</code> | Relative command path, after REST API version. |

<a id="vscp.rest.Client+_makeRequest"></a>
##### client._makeRequest(options) ⇒ <code>object</code>
Make a request to VSCP daemon via REST api.
The onSuccess and onError function parameter are harmonized here.
This makes it easier to process them further.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.path | <code>string</code> | Relative path |
| options.parameter | <code>Array.&lt;string&gt;</code> | Array of URL parameter |
| options.type | <code>string</code> | 'GET', 'POST', or etc. |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+_abort"></a>
##### client._abort(error, [onError]) ⇒ <code>object</code>
Prepare error object, call error callback and return rejected promise.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - Rejected jquery promise  

| Param | Type | Description |
| --- | --- | --- |
| error | <code>string</code> | Error description |
| [onError] | <code>function</code> | Callback |

<a id="vscp.rest.Client+openSession"></a>
##### client.openSession(options) ⇒ <code>object</code>
Open a session.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.user | <code>string</code> | User name |
| options.password | <code>string</code> | Password |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+closeSession"></a>
##### client.closeSession([options]) ⇒ <code>object</code>
Close a session.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+getStatus"></a>
##### client.getStatus([options]) ⇒ <code>object</code>
Get status and how many events are in the queue.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+sendEvent"></a>
##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>object</code> | VSCP event |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+readEvent"></a>
##### client.readEvent([options]) ⇒ <code>object</code>
Read one or more VSCP events.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.count] | <code>object</code> | Number of events to read |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+setFilter"></a>
##### client.setFilter(options) ⇒ <code>object</code>
Set filter.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+clearQueue"></a>
##### client.clearQueue([options]) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+createVar"></a>
##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.type] | <code>number</code> | Variable type (default: string) |
| [options.accessrights] | <code>number</code> | Variable value (default: 744) |
| options.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| options.value | <code>string</code> | Variable Value |
| [options.note] | <code>string</code> | Variable note (optional) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+readVar"></a>
##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+writeVar"></a>
##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+removeVar"></a>
##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+listVar"></a>
##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.listLong | <code>boolean</code> | When false the variable list dos not include value and note. If set to true value and note is included. |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws"></a>
### vscp.ws : <code>object</code>
VSCP websocket api functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.ws](#vscp.ws) : <code>object</code>
  * [.Client](#vscp.ws.Client)
    * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
    * _instance_
      * [.states](#vscp.ws.Client+states) : <code>enum</code>
      * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
      * [.socket](#vscp.ws.Client+socket) : <code>object</code>
      * [.url](#vscp.ws.Client+url) : <code>string</code>
      * [.userName](#vscp.ws.Client+userName) : <code>string</code>
      * [.userId](#vscp.ws.Client+userId) : <code>number</code>
      * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
      * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
      * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
      * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
      * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
      * [.password](#vscp.ws.Client+password) : <code>string</code>
      * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
      * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
      * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
      * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
      * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
      * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
      * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
      * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
      * [.state](#vscp.ws.Client+state) : <code>number</code>
      * [.substate](#vscp.ws.Client+substate) : <code>number</code>
      * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
      * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
      * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
      * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
      * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
      * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
      * [.signalConnError()](#vscp.ws.Client+signalConnError)
      * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
      * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
      * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
      * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
      * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
      * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
      * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
      * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
      * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
      * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
      * [.connect(options)](#vscp.ws.Client+connect)
      * [.disconnect()](#vscp.ws.Client+disconnect)
      * [.start(options)](#vscp.ws.Client+start)
      * [.stop(options)](#vscp.ws.Client+stop)
      * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
      * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
      * [.setFilter(options)](#vscp.ws.Client+setFilter)
      * [.createVar(options)](#vscp.ws.Client+createVar)
      * [.readVar(options)](#vscp.ws.Client+readVar)
      * [.writeVar(options)](#vscp.ws.Client+writeVar)
      * [.resetVar(options)](#vscp.ws.Client+resetVar)
      * [.removeVar(options)](#vscp.ws.Client+removeVar)
      * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
      * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
      * [.listVar(options)](#vscp.ws.Client+listVar)
      * [.readTable(options)](#vscp.ws.Client+readTable)
    * _inner_
      * [~Command](#vscp.ws.Client..Command)
        * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
        * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
        * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
        * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
      * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
      * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>

<a id="vscp.ws.Client"></a>
#### ws.Client
**Kind**: static class of <code>[ws](#vscp.ws)</code>  

* [.Client](#vscp.ws.Client)
  * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
  * _instance_
    * [.states](#vscp.ws.Client+states) : <code>enum</code>
    * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
    * [.socket](#vscp.ws.Client+socket) : <code>object</code>
    * [.url](#vscp.ws.Client+url) : <code>string</code>
    * [.userName](#vscp.ws.Client+userName) : <code>string</code>
    * [.userId](#vscp.ws.Client+userId) : <code>number</code>
    * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
    * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
    * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
    * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
    * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
    * [.password](#vscp.ws.Client+password) : <code>string</code>
    * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
    * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
    * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
    * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
    * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
    * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
    * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
    * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
    * [.state](#vscp.ws.Client+state) : <code>number</code>
    * [.substate](#vscp.ws.Client+substate) : <code>number</code>
    * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
    * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
    * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
    * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
    * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
    * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
    * [.signalConnError()](#vscp.ws.Client+signalConnError)
    * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
    * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
    * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
    * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
    * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
    * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
    * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
    * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
    * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
    * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
    * [.connect(options)](#vscp.ws.Client+connect)
    * [.disconnect()](#vscp.ws.Client+disconnect)
    * [.start(options)](#vscp.ws.Client+start)
    * [.stop(options)](#vscp.ws.Client+stop)
    * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
    * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
    * [.setFilter(options)](#vscp.ws.Client+setFilter)
    * [.createVar(options)](#vscp.ws.Client+createVar)
    * [.readVar(options)](#vscp.ws.Client+readVar)
    * [.writeVar(options)](#vscp.ws.Client+writeVar)
    * [.resetVar(options)](#vscp.ws.Client+resetVar)
    * [.removeVar(options)](#vscp.ws.Client+removeVar)
    * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
    * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
    * [.listVar(options)](#vscp.ws.Client+listVar)
    * [.readTable(options)](#vscp.ws.Client+readTable)
  * _inner_
    * [~Command](#vscp.ws.Client..Command)
      * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
      * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
      * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
      * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
    * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
    * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>

<a id="new_vscp.ws.Client_new"></a>
##### new vscp.ws.Client()
VSCP websocket client, used for connection establishment to a VSCP server.

<a id="vscp.ws.Client+states"></a>
##### client.states : <code>enum</code>
States of the VSCP websocket

**Kind**: instance enum property of <code>[Client](#vscp.ws.Client)</code>  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| DISCONNECTED | <code>number</code> | <code>0</code> | Not connected |
| CONNECTED | <code>number</code> | <code>1</code> | Standard websocket connection established |
| AUTHENTICATED | <code>number</code> | <code>2</code> | Authentication with VSCP server successful |

<a id="vscp.ws.Client+substates"></a>
##### client.substates : <code>enum</code>
Substates of the VSCP websocket

**Kind**: instance enum property of <code>[Client](#vscp.ws.Client)</code>  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| CLOSED | <code>number</code> | <code>0</code> | No events sent from server |
| OPEN | <code>number</code> | <code>1</code> | Events sent from server |

<a id="vscp.ws.Client+socket"></a>
##### client.socket : <code>object</code>
Websocket

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+url"></a>
##### client.url : <code>string</code>
url used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userName"></a>
##### client.userName : <code>string</code>
User name used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userId"></a>
##### client.userId : <code>number</code>
User id from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userFullname"></a>
##### client.userFullname : <code>string</code>
User full name from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userRights"></a>
##### client.userRights : <code>array</code>
User rights from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userRemotes"></a>
##### client.userRemotes : <code>array</code>
User allowed remotes from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userEvents"></a>
##### client.userEvents : <code>array</code>
User allowed events from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userNote"></a>
##### client.userNote : <code>string</code>
User note from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+password"></a>
##### client.password : <code>string</code>
Password used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+vscpkey"></a>
##### client.vscpkey : <code>string</code>
Secret key used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+authdomain"></a>
##### client.authdomain : <code>string</code>
authdomain used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+passwordHash"></a>
##### client.passwordHash : <code>string</code>
Password hash used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onConnError"></a>
##### client.onConnError : <code>function</code>
Callback called on any connection error

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onMessage"></a>
##### client.onMessage : <code>function</code>
Callback called on any received VSCP response message

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onEvent"></a>
##### client.onEvent : <code>Array.&lt;function()&gt;</code>
Callbacks called on any received VSCP event message

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onVariable"></a>
##### client.onVariable : <code>function</code>
Callback called on any received variable (see LSTVAR command)

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onTableRow"></a>
##### client.onTableRow : <code>function</code>
Callback called on any received table row (see GT command)

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+state"></a>
##### client.state : <code>number</code>
VSCP websocket is not connected right now

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+substate"></a>
##### client.substate : <code>number</code>
VSCP event traffic is closed

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+webSocketMessages"></a>
##### client.webSocketMessages : <code>object</code>
VSCP websocket command responses and unsolicited messages

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+getPendingCommand"></a>
##### client.getPendingCommand(command) ⇒ <code>Command</code>
Get command from queue with pending commands.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>Command</code> - Command object  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |

<a id="vscp.ws.Client+_sendCommand"></a>
##### client._sendCommand(options)
Send command to VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.command | <code>string</code> | Command string |
| options.data | <code>string</code> | Data string |
| options.simulate | <code>boolean</code> | Simulate the command (true/false) |
| options.onSuccess | <code>function</code> | Callback on success |
| options.onError | <code>function</code> | Callback on error |

<a id="vscp.ws.Client+_sendEvent"></a>
##### client._sendEvent(options)
Send event to VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.data | <code>string</code> | Data string |
| options.onSuccess | <code>function</code> | Callback on success |
| options.onError | <code>function</code> | Callback on error |

<a id="vscp.ws.Client+signalSuccess"></a>
##### client.signalSuccess(command, [obj])
Signal success of the current asynchronous operation.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| [obj] | <code>object</code> | Options for on success callback |

<a id="vscp.ws.Client+signalError"></a>
##### client.signalError(command, [obj])
Signal failed of the current asynchronous operation.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| [obj] | <code>object</code> | Options for on error callback |

<a id="vscp.ws.Client+signalConnError"></a>
##### client.signalConnError()
Signal a connection error.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+signalMessage"></a>
##### client.signalMessage(msg) ⇒ <code>boolean</code>
Signal a received VSCP response message.
If the message is handled by the application, the application will return
true, which means no further actions shall take place in this object.
Otherwise the message is handled by the standard onMessage handler here.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>boolean</code> - Message is handled (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp.ws.Client+signalEvent"></a>
##### client.signalEvent(vscpEvent)
Signal a received VSCP event.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| vscpEvent | <code>[Event](#vscp.Event)</code> | VSCP event |

<a id="vscp.ws.Client+signalVariable"></a>
##### client.signalVariable(variable)
Signal a received variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| variable | <code>object</code> | Variable object |
| variable.id | <code>number</code> | Consecutive number |
| variable.name | <code>string</code> | Variable name |
| variable.type | <code>string</code> | Variable type |
| variable.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| variable.value | <code>string</code> | Variable value |

<a id="vscp.ws.Client+signalTableRow"></a>
##### client.signalTableRow(row)
Signal a received table row.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| row | <code>object</code> | Table row object |
| row.date | <code>string</code> | Date and time |
| row.value | <code>string</code> | Value |

<a id="vscp.ws.Client+addEventListener"></a>
##### client.addEventListener(eventListener)
Add a event listener.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp.ws.Client+removeEventListener"></a>
##### client.removeEventListener(eventListener)
Remove a event listener.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp.ws.Client+getAuthHash"></a>
##### client.getAuthHash(userName, password, str_iv) ⇒ <code>string</code>
Calculates the VSCP server websocket authentication hash.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>string</code> - Authentication ("encrypted user:password")  

| Param | Type | Description |
| --- | --- | --- |
| userName | <code>string</code> | User name |
| password | <code>string</code> | Password |
| str_iv | <code>string</code> | 16 random byte iv in hex form |

<a id="vscp.ws.Client+onWebSocketOpen"></a>
##### client.onWebSocketOpen()
This function is called by the websocket in case the connection is established.
It will initiate the authentication with the VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onWebSocketClose"></a>
##### client.onWebSocketClose()
This function is called by the websocket in case that the connection is closed.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onWebSocketMessage"></a>
##### client.onWebSocketMessage(msg)
This function is called for any websocket message (VSCP server response message).

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp.ws.Client+connect"></a>
##### client.connect(options)
Connect to a VSCP server with the given URL.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.url | <code>string</code> | URL to the VSCP server, e.g. ws:// |
| options.userName | <code>string</code> | User name used for authentication |
| options.password | <code>string</code> | Password used for authentication |
| options.vscpkey | <code>string</code> | Secret key used for authentication |
| [options.onMessage] | <code>function</code> | Function which is called on any received VSCP response message. |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful connection establishment. |
| [options.onError] | <code>function</code> | Function which is called on a failed connection establishment or in case the connection is lost during the session. |

<a id="vscp.ws.Client+disconnect"></a>
##### client.disconnect()
Disconnect from a VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+start"></a>
##### client.start(options)
Start receiving events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+stop"></a>
##### client.stop(options)
Stop receiving events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+clearQueue"></a>
##### client.clearQueue(options)
Clear the VSCP event queue on the server side.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+sendEvent"></a>
##### client.sendEvent(options)
Send a VSCP event to the VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>[Event](#vscp.Event)</code> | VSCP event to send |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+setFilter"></a>
##### client.setFilter(options)
Set a filter in the VSCP server for VSCP events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+createVar"></a>
##### client.createVar(options)
Create a a VSCP remote variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.type] | <code>number</code> | Variable type (default: string) |
| [options.accessrights] | <code>number</code> | Variable value (default: 744) |
| options.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| options.value | <code>string</code> | Variable Value |
| [options.note] | <code>string</code> | Variable note (optional) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+readVar"></a>
##### client.readVar(options)
Read a value from a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+writeVar"></a>
##### client.writeVar(options)
Write a value to a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+resetVar"></a>
##### client.resetVar(options)
Reset a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+removeVar"></a>
##### client.removeVar(options)
Remove a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+lengthVar"></a>
##### client.lengthVar(options)
Get a VSCP server variable length.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+lastChangeVar"></a>
##### client.lastChangeVar(options)
Get last change of a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+listVar"></a>
##### client.listVar(options)
List all VSCP server variables.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| options.onVariable | <code>function</code> | Function which is called per variable |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+readTable"></a>
##### client.readTable(options)
Get data from a table.
If "begin" and "end" are omitted, the whole table is returned.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Table name |
| options.begin | <code>string</code> | Date when to begin ( ISO form YY-MM-DD HH:MM:SS ) |
| options.end | <code>string</code> | Date when to end ( ISO form YY-MM-DD HH:MM:SS ) |
| options.onTableRow | <code>function</code> | Function which is called on every received table row |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client..Command"></a>
##### Client~Command
**Kind**: inner class of <code>[Client](#vscp.ws.Client)</code>  

  * [~Command](#vscp.ws.Client..Command)
    * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
    * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
    * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
    * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>

<a id="new_vscp.ws.Client..Command_new"></a>
###### new Command(command, onSuccess, onerror)
VSCP server command


| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| onSuccess | <code>function</code> | Function which is called on successful operation |
| onerror | <code>function</code> | Function which is called on failed operation |

<a id="vscp.ws.Client..Command+command"></a>
###### command.command : <code>string</code>
Server command string

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..Command+onSuccess"></a>
###### command.onSuccess : <code>function</code>
Function which is called on successful operation

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..Command+onError"></a>
###### command.onError : <code>function</code>
Function which is called on failed operation

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..cmdQueue"></a>
##### Client~cmdQueue : <code>Array.&lt;Command&gt;</code>
Queue contains all pending VSCP server commands

**Kind**: inner property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client..getPendingCommandIndex"></a>
##### Client~getPendingCommandIndex(command) ⇒ <code>number</code>
Get the index of a command in the queue.

**Kind**: inner method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>number</code> - Index of command in the queue. If index is < 0, the command was not found.  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |

<a id="vscp._createNS"></a>
### vscp._createNS(namespace)
Create a general purpose namespace method. This will allow us to create
namespace a bit easier.

**Kind**: static method of <code>[vscp](#vscp)</code>  

| Param | Type | Description |
| --- | --- | --- |
| namespace | <code>string</code> | Complete namespace, e.g. "a.b.c.d" |

<a id="vscp.getVarTypeName"></a>
### vscp.getVarTypeName(n) ⇒ <code>string</code>
Get variable type name as string by numerical code.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Variable type name  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Numerical code |

<a id="vscp.getVarTypeNumerical"></a>
### vscp.getVarTypeNumerical(str) ⇒ <code>number</code>
Get numerical code of variable type from string.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>number</code> - Variable type numerical code  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Variable type name |

<a id="vscp.getEditorModeFromType"></a>
### vscp.getEditorModeFromType(n) ⇒ <code>string</code>
Get ace editor formation mode string from numerical variable type code.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Ace editro formation mode string  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Variable type numerical code |

<a id="vscp.b64EncodeUnicode"></a>
### vscp.b64EncodeUnicode(str) ⇒ <code>string</code>
Encode base64 unicode safe.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Base64  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Unicode string |

<a id="vscp.b64DecodeUnicode"></a>
### vscp.b64DecodeUnicode(str) ⇒ <code>string</code>
Decode base64 unicode safe.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Unicode string  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Base64 |

<a id="vscp.isBase64Type"></a>
### vscp.isBase64Type(type) ⇒ <code>bool</code>
Determine whether the given variable type is a type stored base64 encoded or not.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>bool</code> - Stored base64 encoded (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |

<a id="vscp.decodeValueIfBase64"></a>
### vscp.decodeValueIfBase64(type, value) ⇒ <code>string</code>
Decode the value if its base64 encoded.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Decoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |

<a id="vscp.encodeValueIfBase64"></a>
### vscp.encodeValueIfBase64(type, value) ⇒ <code>string</code>
Encode the value if its stored in base64.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Encoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |

<a id="vscp"></a>
## vscp : <code>object</code>
Namespace for all functionality of the VSCP provided libraries.

**Kind**: global namespace  

* [vscp](#vscp) : <code>object</code>
  * [.Event](#vscp.Event)
    * [new vscp.Event(options)](#new_vscp.Event_new)
    * [.vscpHead](#vscp.Event+vscpHead) : <code>number</code>
    * [.vscpClass](#vscp.Event+vscpClass) : <code>number</code>
    * [.vscpType](#vscp.Event+vscpType) : <code>number</code>
    * [.vscpObId](#vscp.Event+vscpObId) : <code>number</code>
    * [.vscpTimeStamp](#vscp.Event+vscpTimeStamp) : <code>number</code>
    * [.vscpDateTime](#vscp.Event+vscpDateTime) : <code>date</code>
    * [.vscpGuid](#vscp.Event+vscpGuid) : <code>string</code>
    * [.vscpData](#vscp.Event+vscpData) : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
    * [.setIPV6Addr()](#vscp.Event+setIPV6Addr)
    * [.isIPV6Addr()](#vscp.Event+isIPV6Addr) ⇒ <code>boolean</code>
    * [.setDumbNode()](#vscp.Event+setDumbNode)
    * [.isDumbNode()](#vscp.Event+isDumbNode) ⇒ <code>boolean</code>
    * [.setPriority(priority)](#vscp.Event+setPriority)
    * [.getPriority()](#vscp.Event+getPriority) ⇒ <code>number</code>
    * [.setHardCodedAddr()](#vscp.Event+setHardCodedAddr)
    * [.isHardCodedAddr()](#vscp.Event+isHardCodedAddr) ⇒ <code>boolean</code>
    * [.setDoNotCalcCRC()](#vscp.Event+setDoNotCalcCRC)
    * [.isDoNotCalcCRC()](#vscp.Event+isDoNotCalcCRC) ⇒ <code>boolean</code>
    * [.getText()](#vscp.Event+getText) ⇒ <code>string</code>
  * [.version](#vscp.version)
  * [.constants](#vscp.constants) : <code>object</code>
    * [.classes](#vscp.constants.classes) : <code>enum</code>
    * [.types](#vscp.constants.types) : <code>enum</code>
    * [.priorities](#vscp.constants.priorities) : <code>enum</code>
    * [.varTypes](#vscp.constants.varTypes) : <code>enum</code>
    * [.varTypeNames](#vscp.constants.varTypeNames)
  * [.utility](#vscp.utility) : <code>object</code>
    * [.readValue(input)](#vscp.utility.readValue) ⇒ <code>number</code>
    * [.getTime()](#vscp.utility.getTime) ⇒ <code>string</code>
    * [.guidToStr(guid)](#vscp.utility.guidToStr) ⇒ <code>string</code>
    * [.strToGuid(guid)](#vscp.utility.strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
    * [.getNodeId(guid)](#vscp.utility.getNodeId) ⇒ <code>number</code>
  * [.rest](#vscp.rest) : <code>object</code>
    * [.Client](#vscp.rest.Client)
      * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
      * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
      * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
      * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
      * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
      * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
      * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
      * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
      * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
      * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
      * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
      * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
      * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
      * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
      * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
      * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
      * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
      * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
      * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
      * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>
  * [.ws](#vscp.ws) : <code>object</code>
    * [.Client](#vscp.ws.Client)
      * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
      * _instance_
        * [.states](#vscp.ws.Client+states) : <code>enum</code>
        * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
        * [.socket](#vscp.ws.Client+socket) : <code>object</code>
        * [.url](#vscp.ws.Client+url) : <code>string</code>
        * [.userName](#vscp.ws.Client+userName) : <code>string</code>
        * [.userId](#vscp.ws.Client+userId) : <code>number</code>
        * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
        * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
        * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
        * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
        * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
        * [.password](#vscp.ws.Client+password) : <code>string</code>
        * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
        * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
        * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
        * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
        * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
        * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
        * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
        * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
        * [.state](#vscp.ws.Client+state) : <code>number</code>
        * [.substate](#vscp.ws.Client+substate) : <code>number</code>
        * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
        * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
        * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
        * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
        * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
        * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
        * [.signalConnError()](#vscp.ws.Client+signalConnError)
        * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
        * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
        * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
        * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
        * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
        * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
        * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
        * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
        * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
        * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
        * [.connect(options)](#vscp.ws.Client+connect)
        * [.disconnect()](#vscp.ws.Client+disconnect)
        * [.start(options)](#vscp.ws.Client+start)
        * [.stop(options)](#vscp.ws.Client+stop)
        * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
        * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
        * [.setFilter(options)](#vscp.ws.Client+setFilter)
        * [.createVar(options)](#vscp.ws.Client+createVar)
        * [.readVar(options)](#vscp.ws.Client+readVar)
        * [.writeVar(options)](#vscp.ws.Client+writeVar)
        * [.resetVar(options)](#vscp.ws.Client+resetVar)
        * [.removeVar(options)](#vscp.ws.Client+removeVar)
        * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
        * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
        * [.listVar(options)](#vscp.ws.Client+listVar)
        * [.readTable(options)](#vscp.ws.Client+readTable)
      * _inner_
        * [~Command](#vscp.ws.Client..Command)
          * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
          * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
          * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
          * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
        * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
        * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>
  * [._createNS(namespace)](#vscp._createNS)
  * [.getVarTypeName(n)](#vscp.getVarTypeName) ⇒ <code>string</code>
  * [.getVarTypeNumerical(str)](#vscp.getVarTypeNumerical) ⇒ <code>number</code>
  * [.getEditorModeFromType(n)](#vscp.getEditorModeFromType) ⇒ <code>string</code>
  * [.b64EncodeUnicode(str)](#vscp.b64EncodeUnicode) ⇒ <code>string</code>
  * [.b64DecodeUnicode(str)](#vscp.b64DecodeUnicode) ⇒ <code>string</code>
  * [.isBase64Type(type)](#vscp.isBase64Type) ⇒ <code>bool</code>
  * [.decodeValueIfBase64(type, value)](#vscp.decodeValueIfBase64) ⇒ <code>string</code>
  * [.encodeValueIfBase64(type, value)](#vscp.encodeValueIfBase64) ⇒ <code>string</code>

<a id="vscp.Event"></a>
### vscp.Event
**Kind**: static class of <code>[vscp](#vscp)</code>  

* [.Event](#vscp.Event)
  * [new vscp.Event(options)](#new_vscp.Event_new)
  * [.vscpHead](#vscp.Event+vscpHead) : <code>number</code>
  * [.vscpClass](#vscp.Event+vscpClass) : <code>number</code>
  * [.vscpType](#vscp.Event+vscpType) : <code>number</code>
  * [.vscpObId](#vscp.Event+vscpObId) : <code>number</code>
  * [.vscpTimeStamp](#vscp.Event+vscpTimeStamp) : <code>number</code>
  * [.vscpDateTime](#vscp.Event+vscpDateTime) : <code>date</code>
  * [.vscpGuid](#vscp.Event+vscpGuid) : <code>string</code>
  * [.vscpData](#vscp.Event+vscpData) : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
  * [.setIPV6Addr()](#vscp.Event+setIPV6Addr)
  * [.isIPV6Addr()](#vscp.Event+isIPV6Addr) ⇒ <code>boolean</code>
  * [.setDumbNode()](#vscp.Event+setDumbNode)
  * [.isDumbNode()](#vscp.Event+isDumbNode) ⇒ <code>boolean</code>
  * [.setPriority(priority)](#vscp.Event+setPriority)
  * [.getPriority()](#vscp.Event+getPriority) ⇒ <code>number</code>
  * [.setHardCodedAddr()](#vscp.Event+setHardCodedAddr)
  * [.isHardCodedAddr()](#vscp.Event+isHardCodedAddr) ⇒ <code>boolean</code>
  * [.setDoNotCalcCRC()](#vscp.Event+setDoNotCalcCRC)
  * [.isDoNotCalcCRC()](#vscp.Event+isDoNotCalcCRC) ⇒ <code>boolean</code>
  * [.getText()](#vscp.Event+getText) ⇒ <code>string</code>

<a id="new_vscp.Event_new"></a>
#### new vscp.Event(options)
VSCP event.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.vscpHead | <code>number</code> | Event head |
| options.guidIsIpV6Addr | <code>boolean</code> | GUID is a IPv6 address |
| options.dumpNode | <code>boolean</code> | Node is a dump node |
| options.vscpPriority | <code>number</code> | Priority |
| options.vscpHardCoded | <code>boolean</code> | Hard coded node id |
| options.vscpCalcCRC | <code>boolean</code> | Calculate CRC |
| options.vscpClass | <code>number</code> | VSCP class |
| options.vscpType | <code>number</code> | VSCP type |
| options.vscpObId | <code>number</code> | Object id |
| options.vscpTimeStamp | <code>number</code> | Timestamp |
| options.vscpGuid | <code>string</code> | GUID string |
| options.vscpData | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | Event data |

<a id="vscp.Event+vscpHead"></a>
#### event.vscpHead : <code>number</code>
VSCP event head

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpClass"></a>
#### event.vscpClass : <code>number</code>
VSCP class

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpType"></a>
#### event.vscpType : <code>number</code>
VSCP type

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpObId"></a>
#### event.vscpObId : <code>number</code>
VSCP object id used by driver for channel info and etc.

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpTimeStamp"></a>
#### event.vscpTimeStamp : <code>number</code>
Relative timestamp for package in us

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpDateTime"></a>
#### event.vscpDateTime : <code>date</code>
Date/Time for package

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpGuid"></a>
#### event.vscpGuid : <code>string</code>
Node global unique id LSB(15) -> MSB(0)

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+vscpData"></a>
#### event.vscpData : <code>Array.&lt;number&gt;</code> &#124; <code>string</code>
Data array or string

**Kind**: instance property of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+setIPV6Addr"></a>
#### event.setIPV6Addr()
Set GUID as IP v6 address

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isIPV6Addr"></a>
#### event.isIPV6Addr() ⇒ <code>boolean</code>
Is GUID a IP v6 address or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the GUID is a IP v6 address, it will return true, otherwise false.  
<a id="vscp.Event+setDumbNode"></a>
#### event.setDumbNode()
Set dumb node. No MDF, registers, nothing.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isDumbNode"></a>
#### event.isDumbNode() ⇒ <code>boolean</code>
Is node a dump node or not?
Dumb node means no MDF, registers, nothing.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the node is a dumb node, it will return true, otherwise false.  
<a id="vscp.Event+setPriority"></a>
#### event.setPriority(priority)
Set the VSCP event priority.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  

| Param | Type | Description |
| --- | --- | --- |
| priority | <code>number</code> | Priority |

<a id="vscp.Event+getPriority"></a>
#### event.getPriority() ⇒ <code>number</code>
Get the VSCP event priority.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>number</code> - Priority of the event.  
<a id="vscp.Event+setHardCodedAddr"></a>
#### event.setHardCodedAddr()
Set the node id of the event sender as hard coded?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isHardCodedAddr"></a>
#### event.isHardCodedAddr() ⇒ <code>boolean</code>
Is the node id of the event sender hard coded or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If the node id is hard coded, it will return true, otherwise false.  
<a id="vscp.Event+setDoNotCalcCRC"></a>
#### event.setDoNotCalcCRC()
Set flag for no CRC calculation?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
<a id="vscp.Event+isDoNotCalcCRC"></a>
#### event.isDoNotCalcCRC() ⇒ <code>boolean</code>
Is CRC calculated or not?

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>boolean</code> - If nor CRC should be calculated true is returned.  
<a id="vscp.Event+getText"></a>
#### event.getText() ⇒ <code>string</code>
Get event as string.

**Kind**: instance method of <code>[Event](#vscp.Event)</code>  
**Returns**: <code>string</code> - Event as string  
<a id="vscp.version"></a>
### vscp.version
VSCP websocket library version

**Kind**: static property of <code>[vscp](#vscp)</code>  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| major | <code>number</code> | Major version number |
| minor | <code>number</code> | Minor version number |
| patch | <code>number</code> | Sub-minor version number |

<a id="vscp.constants"></a>
### vscp.constants : <code>object</code>
VSCP constants

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.constants](#vscp.constants) : <code>object</code>
  * [.classes](#vscp.constants.classes) : <code>enum</code>
  * [.types](#vscp.constants.types) : <code>enum</code>
  * [.priorities](#vscp.constants.priorities) : <code>enum</code>
  * [.varTypes](#vscp.constants.varTypes) : <code>enum</code>
  * [.varTypeNames](#vscp.constants.varTypeNames)

<a id="vscp.constants.classes"></a>
#### constants.classes : <code>enum</code>
VSCP classes

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| VSCP_CLASS1_PROTOCOL | <code>number</code> | <code>0</code> | 
| VSCP_CLASS1_ALARM | <code>number</code> | <code>1</code> | 
| VSCP_CLASS1_SECURITY | <code>number</code> | <code>2</code> | 
| VSCP_CLASS1_MEASUREMENT | <code>number</code> | <code>10</code> | 
| VSCP_CLASS1_DATA | <code>number</code> | <code>15</code> | 
| VSCP_CLASS1_INFORMATION | <code>number</code> | <code>20</code> | 
| VSCP_CLASS1_CONTROL | <code>number</code> | <code>30</code> | 
| VSCP_CLASS1_MULTIMEDIA | <code>number</code> | <code>40</code> | 
| VSCP_CLASS1_AOL | <code>number</code> | <code>50</code> | 
| VSCP_CLASS1_MEASUREMENT64 | <code>number</code> | <code>60</code> | 
| VSCP_CLASS1_MEASUREZONE | <code>number</code> | <code>65</code> | 
| VSCP_CLASS1_MEASUREMENT32 | <code>number</code> | <code>70</code> | 
| VSCP_CLASS1_SETVALUEZONE | <code>number</code> | <code>85</code> | 
| VSCP_CLASS1_WEATHER | <code>number</code> | <code>90</code> | 
| VSCP_CLASS1_WEATHER_FORECAST | <code>number</code> | <code>95</code> | 
| VSCP_CLASS1_PHONE | <code>number</code> | <code>100</code> | 
| VSCP_CLASS1_LIN | <code>number</code> | <code>101</code> | 
| VSCP_CLASS1_DISPLAY | <code>number</code> | <code>102</code> | 
| VSCP_CLASS1_REMOTE | <code>number</code> | <code>110</code> | 
| VSCP_CLASS1_GPS | <code>number</code> | <code>206</code> | 
| VSCP_CLASS1_WIRELESS | <code>number</code> | <code>212</code> | 
| VSCP_CLASS1_DIAGNOSTIC | <code>number</code> | <code>506</code> | 
| VSCP_CLASS1_ERROR | <code>number</code> | <code>508</code> | 
| VSCP_CLASS1_LOG | <code>number</code> | <code>509</code> | 
| VSCP_CLASS1_LAB | <code>number</code> | <code>510</code> | 
| VSCP_CLASS1_LOCAL | <code>number</code> | <code>511</code> | 
| VSCP_CLASS2_LEVEL1_PROTOCOL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_ALARM | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_SECURITY | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_DATA | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_INFORMATION | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_CONTROL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MULTIMEDIA | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_AOL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT64 | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREZONE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_MEASUREMENT32 | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_SETVALUEZONE | <code>number</code> | <code></code> | 
| VSCP_CLASS1_LEVEL1_WEATHER | <code>number</code> | <code>90</code> | 
| VSCP_CLASS1_LEVEL1_WEATHER_FORECAST | <code>number</code> | <code>95</code> | 
| VSCP_CLASS2_LEVEL1_PHONE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_REMOTE | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_GPS | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_WIRELESS | <code>number</code> | <code></code> | 
| VSCP_CLASS1_LEVEL1_DIAGNOSTIC | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LOG | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LAB | <code>number</code> | <code></code> | 
| VSCP_CLASS2_LEVEL1_LOCAL | <code>number</code> | <code></code> | 
| VSCP_CLASS2_PROTOCOL | <code>number</code> | <code>1024</code> | 
| VSCP_CLASS2_CONTROL | <code>number</code> | <code>1025</code> | 
| VSCP_CLASS2_INFORMATION | <code>number</code> | <code>1026</code> | 
| VSCP_CLASS2_TEXT2SPEECH | <code>number</code> | <code>1028</code> | 
| VSCP_CLASS2_CUSTOM | <code>number</code> | <code>1029</code> | 
| VSCP_CLASS2_DISPLAY | <code>number</code> | <code>1030</code> | 
| VSCP_CLASS2_MEASUREMENT_STR | <code>number</code> | <code>1040</code> | 
| VSCP_CLASS2_MEASUREMENT_FLOAT | <code>number</code> | <code>1060</code> | 
| VSCP_CLASS2_VSCPD | <code>number</code> | <code>65535</code> | 

<a id="vscp.constants.types"></a>
#### constants.types : <code>enum</code>
VSCP class types

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| VSCP_TYPE_UNDEFINED | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_PROTOCOL_SEGCTRL_HEARTBEAT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_PROTOCOL_NEW_NODE_ONLINE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_PROTOCOL_PROBE_ACK | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_PROTOCOL_SET_NICKNAME | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_PROTOCOL_NICKNAME_ACCEPTED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_PROTOCOL_DROP_NICKNAME | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_PROTOCOL_READ_REGISTER | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_PROTOCOL_RW_RESPONSE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_PROTOCOL_WRITE_REGISTER | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_PROTOCOL_ENTER_BOOT_LOADER | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_PROTOCOL_ACK_BOOT_LOADER | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_PROTOCOL_NACK_BOOT_LOADER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA_ACK | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_PROTOCOL_BLOCK_DATA_NACK | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA_ACK | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_PROTOCOL_PROGRAM_BLOCK_DATA_NACK | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_PROTOCOL_RESET_DEVICE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_PROTOCOL_PAGE_READ | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_PROTOCOL_PAGE_WRITE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_PROTOCOL_RW_PAGE_RESPONSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_PROTOCOL_HIGH_END_SERVER_PROBE | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_PROTOCOL_HIGH_END_SERVER_RESPONSE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_PROTOCOL_INCREMENT_REGISTER | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_PROTOCOL_DECREMENT_REGISTER | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_PROTOCOL_WHO_IS_THERE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_PROTOCOL_WHO_IS_THERE_RESPONSE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_PROTOCOL_GET_MATRIX_INFO | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_PROTOCOL_GET_MATRIX_INFO_RESPONSE | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_PROTOCOL_GET_EMBEDDED_MDF | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_PROTOCOL_GET_EMBEDDED_MDF_RESPONSE | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_READ | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_WRITE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_PROTOCOL_EXTENDED_PAGE_RESPONSE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_PROTOCOL_GET_EVENT_INTEREST | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_PROTOCOL_GET_EVENT_INTEREST_RESPONSE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE_ACK | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_PROTOCOL_ACTIVATE_NEW_IMAGE_NACK | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK_ACK | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_PROTOCOL_START_BLOCK_NACK | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_ALARM_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_ALARM_WARNING | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_ALARM_ALARM | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_ALARM_SOUND | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_ALARM_LIGHT | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_ALARM_POWER | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_STOP | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_PAUSE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_RESET | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_ALARM_EMERGENCY_RESUME | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_ALARM_ARM | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_ALARM_DISARM | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SECURITY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_SECURITY_MOTION | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_SECURITY_GLASS_BREAK | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_SECURITY_BEAM_BREAK | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_SECURITY_SENSOR_TAMPER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_SECURITY_SHOCK_SENSOR | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_SECURITY_SMOKE_SENSOR | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_SECURITY_HEAT_SENSOR | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_SECURITY_PANIC_SWITCH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_SECURITY_DOOR_OPEN | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_SECURITY_WINDOW_OPEN | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_SECURITY_CO_SENSOR | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SECURITY_FROST_DETECTED | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_SECURITY_FLAME_DETECTED | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_SECURITY_OXYGEN_LOW | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_SECURITY_WEIGHT_DETECTED | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_SECURITY_WATER_DETECTED | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_SECURITY_CONDENSATION_DETECTED | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_SECURITY_SOUND_DETECTED | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_SECURITY_HARMFUL_SOUND_LEVEL | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_SECURITY_TAMPER | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_RESISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_DATA_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DATA_IO | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DATA_AD | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DATA_DA | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DATA_RELATIVE_STRENGTH | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DATA_SIGNAL_LEVEL | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DATA_SIGNAL_QUALITY | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_INFORMATION_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_INFORMATION_BUTTON | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_INFORMATION_MOUSE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_INFORMATION_ON | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_INFORMATION_OFF | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_INFORMATION_ALIVE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_INFORMATION_TERMINATING | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_INFORMATION_OPENED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_INFORMATION_CLOSED | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_INFORMATION_NODE_HEARTBEAT | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_INFORMATION_BELOW_LIMIT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_INFORMATION_ABOVE_LIMIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_INFORMATION_PULSE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_INFORMATION_ERROR | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_INFORMATION_RESUMED | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_INFORMATION_PAUSED | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_INFORMATION_SLEEP | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_INFORMATION_GOOD_MORNING | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_INFORMATION_GOOD_DAY | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_INFORMATION_GOOD_AFTERNOON | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_INFORMATION_GOOD_EVENING | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_INFORMATION_GOOD_NIGHT | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_INFORMATION_SEE_YOU_SOON | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_INFORMATION_GOODBYE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_INFORMATION_STOP | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_INFORMATION_START | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_INFORMATION_RESET_COMPLETED | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_INFORMATION_INTERRUPTED | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_INFORMATION_PREPARING_TO_SLEEP | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_INFORMATION_WOKEN_UP | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_INFORMATION_DUSK | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_INFORMATION_DAWN | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_INFORMATION_ACTIVE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_INFORMATION_INACTIVE | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_INFORMATION_BUSY | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_INFORMATION_IDLE | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_INFORMATION_STREAM_DATA | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_INFORMATION_TOKEN_ACTIVITY | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_INFORMATION_STREAM_DATA_WITH_ZONE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_INFORMATION_CONFIRM | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_INFORMATION_LEVEL_CHANGED | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_INFORMATION_WARNING | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_INFORMATION_STATE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_INFORMATION_ACTION_TRIGGER | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_INFORMATION_SUNRISE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_INFORMATION_SUNSET | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_INFORMATION_START_OF_RECORD | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_INFORMATION_END_OF_RECORD | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_INFORMATION_PRESET_ACTIVE | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_INFORMATION_DETECT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_INFORMATION_OVERFLOW | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_INFORMATION_BIG_LEVEL_CHANGED | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_INFORMATION_SUNRISE_TWILIGHT_START | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_INFORMATION_SUNSET_TWILIGHT_START | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_INFORMATION_NAUTICAL_SUNRISE_TWILIGHT_START | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_INFORMATION_NAUTICAL_SUNSET_TWILIGHT_START | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_INFORMATION_ASTRONOMICAL_SUNRISE_TWILIGHT_START | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_INFORMATION_ASTRONOMICAL_SUNSET_TWILIGHT_START | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_INFORMATION_CALCULATED_NOON | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_UP | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_DOWN | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_LEFT | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_RIGHT | <code>number</code> | <code>62</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_TOP | <code>number</code> | <code>63</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_BOTTOM | <code>number</code> | <code>64</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_MIDDLE | <code>number</code> | <code>65</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_PRESET | <code>number</code> | <code>66</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_LEFT | <code>number</code> | <code>67</code> | 
| VSCP_TYPE_INFORMATION_SHUTTER_END_RIGHT | <code>number</code> | <code>68</code> | 
| VSCP_TYPE_INFORMATION_LONG_CLICK | <code>number</code> | <code>69</code> | 
| VSCP_TYPE_INFORMATION_SINGLE_CLICK | <code>number</code> | <code>70</code> | 
| VSCP_TYPE_INFORMATION_DOUBLE_CLICK | <code>number</code> | <code>71</code> | 
| VSCP_TYPE_INFORMATION_DATE | <code>number</code> | <code>72</code> | 
| VSCP_TYPE_INFORMATION_TIME | <code>number</code> | <code>73</code> | 
| VSCP_TYPE_INFORMATION_WEEKDAY | <code>number</code> | <code>74</code> | 
| VSCP_TYPE_INFORMATION_LOCK | <code>number</code> | <code>75</code> | 
| VSCP_TYPE_INFORMATION_UNLOCK | <code>number</code> | <code>76</code> | 
| VSCP_TYPE_CONTROL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_CONTROL_MUTE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_CONTROL_OPEN | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_CONTROL_CLOSE | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_CONTROL_TURNON | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_CONTROL_TURNOFF | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_CONTROL_START | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_CONTROL_STOP | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_CONTROL_RESET | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_CONTROL_INTERRUPT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_CONTROL_SLEEP | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_CONTROL_WAKEUP | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_CONTROL_RESUME | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_CONTROL_PAUSE | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_CONTROL_ACTIVATE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_CONTROL_DEACTIVATE | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_CONTROL_DIM_LAMPS | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_CONTROL_CHANGE_CHANNEL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_CONTROL_CHANGE_LEVEL | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_CONTROL_RELATIVE_CHANGE_LEVEL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_CONTROL_MEASUREMENT_REQUEST | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_CONTROL_STREAM_DATA | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_CONTROL_SYNC | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_CONTROL_ZONED_STREAM_DATA | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_CONTROL_SET_PRESET | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_CONTROL_TOGGLE_STATE | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_CONTROL_TIMED_PULSE_ON | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_CONTROL_TIMED_PULSE_OFF | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_CONTROL_SET_COUNTRY_LANGUAGE | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_CONTROL_BIG_CHANGE_LEVEL | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_UP | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_DOWN | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_LEFT | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_RIGHT | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_MIDDLE | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_CONTROL_SHUTTER_PRESET | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS_ON | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_CONTROL_ALL_LAMPS_OFF | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_CONTROL_LOCK | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_CONTROL_UNLOCK | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MULTIMEDIA_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MULTIMEDIA_PLAYBACK | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MULTIMEDIA_NAVIGATOR_KEY_ENG | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_CONTRAST | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_FOCUS | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_TINT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_COLOUR_BALANCE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_BRIGHTNESS | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_HUE | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_BASS | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_TREBLE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_MASTER_VOLUME | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_FRONT_VOLUME | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_CENTRE_VOLUME | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_REAR_VOLUME | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SIDE_VOLUME | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_DISK | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_TRACK | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_ALBUM | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_CHANNEL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_PAGE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_CHAPTER | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_SCREEN_FORMAT | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_INPUT_SOURCE | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MULTIMEDIA_ADJUST_SELECT_OUTPUT | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MULTIMEDIA_RECORD | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MULTIMEDIA_SET_RECORDING_VOLUME | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MULTIMEDIA_TIVO_FUNCTION | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MULTIMEDIA_GET_CURRENT_TITLE | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MULTIMEDIA_SET_POSITION | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MULTIMEDIA_GET_MEDIA_INFO | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MULTIMEDIA_REMOVE_ITEM | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MULTIMEDIA_REMOVE_ALL_ITEMS | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MULTIMEDIA_SAVE_ALBUM | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MULTIMEDIA_CONTROL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MULTIMEDIA_CONTROL_RESPONSE | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_AOL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_AOL_UNPLUGGED_POWER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_AOL_UNPLUGGED_LAN | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_AOL_CHASSIS_INTRUSION | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_AOL_PROCESSOR_REMOVAL | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_AOL_ENVIRONMENT_ERROR | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_AOL_HIGH_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_AOL_FAN_SPEED | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_AOL_VOLTAGE_FLUCTUATIONS | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_AOL_OS_ERROR | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_AOL_POWER_ON_ERROR | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_AOL_SYSTEM_HUNG | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_AOL_COMPONENT_FAILURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_AOL_REBOOT_UPON_FAILURE | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_AOL_REPAIR_OPERATING_SYSTEM | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_AOL_UPDATE_BIOS_IMAGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_AOL_UPDATE_DIAGNOSTIC_PROCEDURE | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT64_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT64_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT64_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT64_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT64_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT64_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT64_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT64_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT64_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT64_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT64_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT64_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT64_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT64_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT64_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT64_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT64_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT64_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT64_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT64_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT64_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT64_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT64_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT64_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT64_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT64_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT64_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT64_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT64_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT64_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT64_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT64_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT64_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT64_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT64_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT64_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT64_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT64_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT64_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT64_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT64_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT64_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT64_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT64_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MEASUREZONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREZONE_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREZONE_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREZONE_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREZONE_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREZONE_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREZONE_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREZONE_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREZONE_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREZONE_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREZONE_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREZONE_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREZONE_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREZONE_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREZONE_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREZONE_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREZONE_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREZONE_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREZONE_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREZONE_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREZONE_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREZONE_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREZONE_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREZONE_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREZONE_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREZONE_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREZONE_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREZONE_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREZONE_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREZONE_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREZONE_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREZONE_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREZONE_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREZONE_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREZONE_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREZONE_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREZONE_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREZONE_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREZONE_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREZONE_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREZONE_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREZONE_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREZONE_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREZONE_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREZONE_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREZONE_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREZONE_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_MEASUREMENT32_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_MEASUREMENT32_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_MEASUREMENT32_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_MEASUREMENT32_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_MEASUREMENT32_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_MEASUREMENT32_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_MEASUREMENT32_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_MEASUREMENT32_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_MEASUREMENT32_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_MEASUREMENT32_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_MEASUREMENT32_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_MEASUREMENT32_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_MEASUREMENT32_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_MEASUREMENT32_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_MEASUREMENT32_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_MEASUREMENT32_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_MEASUREMENT32_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_MEASUREMENT32_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_MEASUREMENT32_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_MEASUREMENT32_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_MEASUREMENT32_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_MEASUREMENT32_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_MEASUREMENT32_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_MEASUREMENT32_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_MEASUREMENT32_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_MEASUREMENT32_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_MEASUREMENT32_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_MEASUREMENT32_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_MEASUREMENT32_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_MEASUREMENT32_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_MEASUREMENT32_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_MEASUREMENT32_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_MEASUREMENT32_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_MEASUREMENT32_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_MEASUREMENT32_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_MEASUREMENT32_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_MEASUREMENT32_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_MEASUREMENT32_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_MEASUREMENT32_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_MEASUREMENT32_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_MEASUREMENT32_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_MEASUREMENT32_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_MEASUREMENT32_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_MEASUREMENT32_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_SETVALUEZONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_SETVALUEZONE_COUNT | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_SETVALUEZONE_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_SETVALUEZONE_MASS | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_SETVALUEZONE_TIME | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_SETVALUEZONE_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_SETVALUEZONE_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_SETVALUEZONE_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_SETVALUEZONE_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_SETVALUEZONE_FORCE | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_SETVALUEZONE_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_SETVALUEZONE_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_SETVALUEZONE_POWER | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_SETVALUEZONE_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_SETVALUEZONE_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_SETVALUEZONE_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_SETVALUEZONE_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_SETVALUEZONE_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_SETVALUEZONE_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_SETVALUEZONE_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_SETVALUEZONE_POSITION | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_SETVALUEZONE_SPEED | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_SETVALUEZONE_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_SETVALUEZONE_TENSION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_SETVALUEZONE_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_SETVALUEZONE_FLOW | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_SETVALUEZONE_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_SETVALUEZONE_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_SETVALUEZONE_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_SETVALUEZONE_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_SETVALUEZONE_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_SETVALUEZONE_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_SETVALUEZONE_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_SETVALUEZONE_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_SETVALUEZONE_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_SETVALUEZONE_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_SETVALUEZONE_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_SETVALUEZONE_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_SETVALUEZONE_AREA | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_SETVALUEZONE_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_SETVALUEZONE_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_SETVALUEZONE_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_SETVALUEZONE_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_SETVALUEZONE_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_WEATHER_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WEATHER_SEASONS_WINTER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_WEATHER_SEASONS_SPRING | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WEATHER_SEASONS_SUMMER | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_WEATHER_SEASONS_AUTUMN | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_WEATHER_WIND_NONE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_WEATHER_WIND_LOW | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_WEATHER_WIND_MEDIUM | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_WEATHER_WIND_HIGH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_WEATHER_WIND_VERY_HIGH | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_WEATHER_AIR_FOGGY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_WEATHER_AIR_FREEZING | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_WEATHER_AIR_VERY_COLD | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_WEATHER_AIR_COLD | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_WEATHER_AIR_NORMAL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_WEATHER_AIR_HOT | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_WEATHER_AIR_VERY_HOT | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_LOW | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_MEDIUM | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_WEATHER_AIR_POLLUTION_HIGH | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_WEATHER_AIR_HUMID | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_WEATHER_AIR_DRY | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_WEATHER_SOIL_HUMID | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_WEATHER_SOIL_DRY | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_WEATHER_RAIN_NONE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_WEATHER_RAIN_LIGHT | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_WEATHER_RAIN_HEAVY | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_WEATHER_RAIN_VERY_HEAVY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_WEATHER_SUN_NONE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_WEATHER_SUN_LIGHT | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_WEATHER_SUN_HEAVY | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_WEATHER_SNOW_NONE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_WEATHER_SNOW_LIGHT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_WEATHER_SNOW_HEAVY | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_WEATHER_DEW_POINT | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_WEATHER_STORM | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_WEATHER_FLOOD | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_WEATHER_EARTHQUAKE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_WEATHER_NUCLEAR_DISASTER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_WEATHER_FIRE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_WEATHER_LIGHTNING | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_LOW | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_MEDIUM | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_NORMAL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_HIGH | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_WEATHER_UV_RADIATION_VERY_HIGH | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL1 | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL2 | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL3 | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL4 | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_WEATHER_WARNING_LEVEL5 | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_WEATHER_ARMAGEDON | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_WEATHER_FORECAST_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_WINTER | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_SPRING | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_SUMMER | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SEASONS_AUTUMN | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_NONE | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_LOW | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_MEDIUM | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_HIGH | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WIND_VERY_HIGH | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_FOGGY | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_FREEZING | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_VERY_COLD | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_COLD | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_NORMAL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_HOT | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_VERY_HOT | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_LOW | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_MEDIUM | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_POLLUTION_HIGH | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_HUMID | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_WEATHER_FORECAST_AIR_DRY | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SOIL_HUMID | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SOIL_DRY | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_NONE | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_LIGHT | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_HEAVY | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_WEATHER_FORECAST_RAIN_VERY_HEAVY | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_NONE | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_LIGHT | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SUN_HEAVY | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_NONE | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_LIGHT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_WEATHER_FORECAST_SNOW_HEAVY | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_WEATHER_FORECAST_DEW_POINT | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_WEATHER_FORECAST_STORM | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_WEATHER_FORECAST_FLOOD | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_WEATHER_FORECAST_EARTHQUAKE | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_WEATHER_FORECAST_NUCLEAR_DISASTER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_WEATHER_FORECAST_FIRE | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_WEATHER_FORECAST_LIGHTNING | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_LOW | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_MEDIUM | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_NORMAL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_HIGH | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_WEATHER_FORECAST_UV_RADIATION_VERY_HIGH | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL1 | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL2 | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL3 | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL4 | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_WEATHER_FORECAST_WARNING_LEVEL5 | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_WEATHER_FORECAST_ARMAGEDDON | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_PHONE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_PHONE_INCOMING_CALL | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_PHONE_OUTGOING_CALL | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_PHONE_RING | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_PHONE_ANSWER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_PHONE_HANGUP | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_PHONE_GIVEUP | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_PHONE_TRANSFER | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_PHONE_DATABASE_INFO | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_DISPLAY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DISPLAY_CLEAR_DISPLAY | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DISPLAY_POSITION_CURSOR | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DISPLAY_WRITE_DISPLAY | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DISPLAY_WRITE_DISPLAY_BUFFER | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DISPLAY_SHOW_DISPLAY_BUFFER | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DISPLAY_SET_DISPLAY_BUFFER_PARAM | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_DISPLAY_SHOW_TEXT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_DISPLAY_SHOW_LED | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_DISPLAY_SHOW_LED_COLOR | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_REMOTE_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_REMOTE_RC5 | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_REMOTE_SONY12 | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_REMOTE_LIRC | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_REMOTE_VSCP | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_GPS_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_GPS_POSITION | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_GPS_SATELLITES | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_WIRELESS_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_WIRELESS_GSM_CELL | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DIAGNOSTIC_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERVOLTAGE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_DIAGNOSTIC_UNDERVOLTAGE | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_DIAGNOSTIC_VBUS_LOW | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_LOW | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_FULL | <code>number</code> | <code>5</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_ERROR | <code>number</code> | <code>6</code> | 
| VSCP_TYPE_DIAGNOSTIC_BATTERY_OK | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERCURRENT | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_DIAGNOSTIC_CIRCUIT_ERROR | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_DIAGNOSTIC_SHORT_CIRCUIT | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_DIAGNOSTIC_OPEN_CIRCUIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_DIAGNOSTIC_MOIST | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIRE_FAIL | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIRELESS_FAIL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_DIAGNOSTIC_IR_FAIL | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_DIAGNOSTIC_1WIRE_FAIL | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS222_FAIL | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS232_FAIL | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS423_FAIL | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_DIAGNOSTIC_RS485_FAIL | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_DIAGNOSTIC_CAN_FAIL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_DIAGNOSTIC_LAN_FAIL | <code>number</code> | <code>22</code> | 
| VSCP_TYPE_DIAGNOSTIC_USB_FAIL | <code>number</code> | <code>23</code> | 
| VSCP_TYPE_DIAGNOSTIC_WIFI_FAIL | <code>number</code> | <code>24</code> | 
| VSCP_TYPE_DIAGNOSTIC_NFC_RFID_FAIL | <code>number</code> | <code>25</code> | 
| VSCP_TYPE_DIAGNOSTIC_LOW_SIGNAL | <code>number</code> | <code>26</code> | 
| VSCP_TYPE_DIAGNOSTIC_HIGH_SIGNAL | <code>number</code> | <code>27</code> | 
| VSCP_TYPE_DIAGNOSTIC_ADC_FAIL | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_DIAGNOSTIC_ALU_FAIL | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_DIAGNOSTIC_ASSERT | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_DIAGNOSTIC_DAC_FAIL | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_DIAGNOSTIC_DMA_FAIL | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_DIAGNOSTIC_ETH_FAIL | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_DIAGNOSTIC_EXCEPTION | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_DIAGNOSTIC_FPU_FAIL | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_DIAGNOSTIC_GPIO_FAIL | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_DIAGNOSTIC_I2C_FAIL | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_DIAGNOSTIC_I2S_FAIL | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_DIAGNOSTIC_INVALID_CONFIG | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_DIAGNOSTIC_MMU_FAIL | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_DIAGNOSTIC_NMI | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_DIAGNOSTIC_OVERHEAT | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_DIAGNOSTIC_PLL_FAIL | <code>number</code> | <code>43</code> | 
| VSCP_TYPE_DIAGNOSTIC_POR_FAIL | <code>number</code> | <code>44</code> | 
| VSCP_TYPE_DIAGNOSTIC_PWM_FAIL | <code>number</code> | <code>45</code> | 
| VSCP_TYPE_DIAGNOSTIC_RAM_FAIL | <code>number</code> | <code>46</code> | 
| VSCP_TYPE_DIAGNOSTIC_ROM_FAIL | <code>number</code> | <code>47</code> | 
| VSCP_TYPE_DIAGNOSTIC_SPI_FAIL | <code>number</code> | <code>48</code> | 
| VSCP_TYPE_DIAGNOSTIC_STACK_FAIL | <code>number</code> | <code>49</code> | 
| VSCP_TYPE_DIAGNOSTIC_LIN_FAIL | <code>number</code> | <code>50</code> | 
| VSCP_TYPE_DIAGNOSTIC_UART_FAIL | <code>number</code> | <code>51</code> | 
| VSCP_TYPE_DIAGNOSTIC_UNHANDLED_INT | <code>number</code> | <code>52</code> | 
| VSCP_TYPE_DIAGNOSTIC_MEMORY_FAIL | <code>number</code> | <code>53</code> | 
| VSCP_TYPE_DIAGNOSTIC_VARIABLE_RANGE | <code>number</code> | <code>54</code> | 
| VSCP_TYPE_DIAGNOSTIC_WDT | <code>number</code> | <code>55</code> | 
| VSCP_TYPE_DIAGNOSTIC_EEPROM_FAIL | <code>number</code> | <code>56</code> | 
| VSCP_TYPE_DIAGNOSTIC_ENCRYPTION_FAIL | <code>number</code> | <code>57</code> | 
| VSCP_TYPE_DIAGNOSTIC_BAD_USER_INPUT | <code>number</code> | <code>58</code> | 
| VSCP_TYPE_DIAGNOSTIC_DECRYPTION_FAIL | <code>number</code> | <code>59</code> | 
| VSCP_TYPE_DIAGNOSTIC_NOISE | <code>number</code> | <code>60</code> | 
| VSCP_TYPE_DIAGNOSTIC_BOOTLOADER_FAIL | <code>number</code> | <code>61</code> | 
| VSCP_TYPE_DIAGNOSTIC_PROGRAMFLOW_FAIL | <code>number</code> | <code>62</code> | 
| VSCP_TYPE_DIAGNOSTIC_RTC_FAIL | <code>number</code> | <code>63</code> | 
| VSCP_TYPE_DIAGNOSTIC_SYSTEM_TEST_FAIL | <code>number</code> | <code>64</code> | 
| VSCP_TYPE_DIAGNOSTIC_SENSOR_FAIL | <code>number</code> | <code>65</code> | 
| VSCP_TYPE_DIAGNOSTIC_SAFESTATE | <code>number</code> | <code>66</code> | 
| VSCP_TYPE_DIAGNOSTIC_SIGNAL_IMPLAUSIBLE | <code>number</code> | <code>67</code> | 
| VSCP_TYPE_DIAGNOSTIC_STORAGE_FAIL | <code>number</code> | <code>68</code> | 
| VSCP_TYPE_DIAGNOSTIC_SELFTEST_FAIL | <code>number</code> | <code>69</code> | 
| VSCP_TYPE_DIAGNOSTIC_ESD_EMC_EMI | <code>number</code> | <code>70</code> | 
| VSCP_TYPE_DIAGNOSTIC_TIMEOUT | <code>number</code> | <code>71</code> | 
| VSCP_TYPE_DIAGNOSTIC_LCD_FAIL | <code>number</code> | <code>72</code> | 
| VSCP_TYPE_DIAGNOSTIC_TOUCHPANEL_FAIL | <code>number</code> | <code>73</code> | 
| VSCP_TYPE_DIAGNOSTIC_NOLOAD | <code>number</code> | <code>74</code> | 
| VSCP_TYPE_DIAGNOSTIC_COOLING_FAIL | <code>number</code> | <code>75</code> | 
| VSCP_TYPE_DIAGNOSTIC_HEATING_FAIL | <code>number</code> | <code>76</code> | 
| VSCP_TYPE_DIAGNOSTIC_TX_FAIL | <code>number</code> | <code>77</code> | 
| VSCP_TYPE_DIAGNOSTIC_RX_FAIL | <code>number</code> | <code>78</code> | 
| VSCP_TYPE_DIAGNOSTIC_EXT_IC_FAIL | <code>number</code> | <code>79</code> | 
| VSCP_TYPE_ERROR_SUCCESS | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_ERROR_ERROR | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_ERROR_CHANNEL | <code>number</code> | <code>7</code> | 
| VSCP_TYPE_ERROR_FIFO_EMPTY | <code>number</code> | <code>8</code> | 
| VSCP_TYPE_ERROR_FIFO_FULL | <code>number</code> | <code>9</code> | 
| VSCP_TYPE_ERROR_FIFO_SIZE | <code>number</code> | <code>10</code> | 
| VSCP_TYPE_ERROR_FIFO_WAIT | <code>number</code> | <code>11</code> | 
| VSCP_TYPE_ERROR_GENERIC | <code>number</code> | <code>12</code> | 
| VSCP_TYPE_ERROR_HARDWARE | <code>number</code> | <code>13</code> | 
| VSCP_TYPE_ERROR_INIT_FAIL | <code>number</code> | <code>14</code> | 
| VSCP_TYPE_ERROR_INIT_MISSING | <code>number</code> | <code>15</code> | 
| VSCP_TYPE_ERROR_INIT_READY | <code>number</code> | <code>16</code> | 
| VSCP_TYPE_ERROR_NOT_SUPPORTED | <code>number</code> | <code>17</code> | 
| VSCP_TYPE_ERROR_OVERRUN | <code>number</code> | <code>18</code> | 
| VSCP_TYPE_ERROR_RCV_EMPTY | <code>number</code> | <code>19</code> | 
| VSCP_TYPE_ERROR_REGISTER | <code>number</code> | <code>20</code> | 
| VSCP_TYPE_ERROR_TRM_FULL | <code>number</code> | <code>21</code> | 
| VSCP_TYPE_ERROR_LIBRARY | <code>number</code> | <code>28</code> | 
| VSCP_TYPE_ERROR_PROCADDRESS | <code>number</code> | <code>29</code> | 
| VSCP_TYPE_ERROR_ONLY_ONE_INSTANCE | <code>number</code> | <code>30</code> | 
| VSCP_TYPE_ERROR_SUB_DRIVER | <code>number</code> | <code>31</code> | 
| VSCP_TYPE_ERROR_TIMEOUT | <code>number</code> | <code>32</code> | 
| VSCP_TYPE_ERROR_NOT_OPEN | <code>number</code> | <code>33</code> | 
| VSCP_TYPE_ERROR_PARAMETER | <code>number</code> | <code>34</code> | 
| VSCP_TYPE_ERROR_MEMORY | <code>number</code> | <code>35</code> | 
| VSCP_TYPE_ERROR_INTERNAL | <code>number</code> | <code>36</code> | 
| VSCP_TYPE_ERROR_COMMUNICATION | <code>number</code> | <code>37</code> | 
| VSCP_TYPE_ERROR_USER | <code>number</code> | <code>38</code> | 
| VSCP_TYPE_ERROR_PASSWORD | <code>number</code> | <code>39</code> | 
| VSCP_TYPE_ERROR_CONNECTION | <code>number</code> | <code>40</code> | 
| VSCP_TYPE_ERROR_INVALID_HANDLE | <code>number</code> | <code>41</code> | 
| VSCP_TYPE_ERROR_OPERATION_FAILED | <code>number</code> | <code>42</code> | 
| VSCP_TYPE_LOG_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_LOG_MESSAGE | <code>number</code> | <code>1</code> | 
| VSCP_TYPE_LOG_START | <code>number</code> | <code>2</code> | 
| VSCP_TYPE_LOG_STOP | <code>number</code> | <code>3</code> | 
| VSCP_TYPE_LOG_LEVEL | <code>number</code> | <code>4</code> | 
| VSCP_TYPE_LABORATORY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP_TYPE_LOCAL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_PROTOCOL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_PROTOCOL_READ_REGISTER | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_PROTOCOL_WRITE_REGISTER | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_PROTOCOL_READ_WRITE_RESPONSE | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_PROTOCOL_HIGH_END_SERVER_CAPS | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_PROTOCOL_WHO_IS_THERE_RESPONE | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_CONTROL_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_INFORMATION_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_INFORMATION_TOKEN_ACTIVITY | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_INFORMATION_HEART_BEAT | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_TEXT2SPEECH_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_TEXT2SPEECH_TALK | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_CUSTOM_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_DISPLAY_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_COUNT | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MASS | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TIME | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FORCE | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_POWER | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_POSITION | <code>number</code> | <code>31</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPEED | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_TENSION | <code>number</code> | <code>34</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_FLOW | <code>number</code> | <code>36</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_AREA | <code>number</code> | <code>52</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP2_TYPE_MEASUREMENT_STR_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_COUNT | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LENGTH | <code>number</code> | <code>2</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MASS | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TIME | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRIC_CURRENT | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TEMPERATURE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_AMOUNT_OF_SUBSTANCE | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_INTENSITY_OF_LIGHT | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FREQUENCY | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIOACTIVITY | <code>number</code> | <code>10</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FORCE | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_PRESSURE | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ENERGY | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_POWER | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CHARGE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_POTENTIAL | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CAPACITANCE | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_RECISTANCE | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRICAL_CONDUCTANCE | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FIELD_STRENGTH | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FLUX | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_MAGNETIC_FLUX_DENSITY | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_INDUCTANCE | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FLUX_OF_LIGHT | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ILLUMINANCE | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIATION_DOSE | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_CATALYTIC_ACTIVITY | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_VOLUME | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_INTENSITY | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ANGLE | <code>number</code> | <code>30</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_POSITION | <code>number</code> | <code>31</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPEED | <code>number</code> | <code>32</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ACCELERATION | <code>number</code> | <code>33</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_TENSION | <code>number</code> | <code>34</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_HUMIDITY | <code>number</code> | <code>35</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_FLOW | <code>number</code> | <code>36</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_THERMAL_RESISTANCE | <code>number</code> | <code>37</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_REFRACTIVE_POWER | <code>number</code> | <code>38</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DYNAMIC_VISCOSITY | <code>number</code> | <code>39</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_IMPEDANCE | <code>number</code> | <code>40</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_RESISTANCE | <code>number</code> | <code>41</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ELECTRIC_ELASTANCE | <code>number</code> | <code>42</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LUMINOUS_ENERGY | <code>number</code> | <code>43</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_LUMINANCE | <code>number</code> | <code>44</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_CHEMICAL_CONCENTRATION | <code>number</code> | <code>45</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RESERVED | <code>number</code> | <code>46</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DOSE_EQUIVALENT | <code>number</code> | <code>47</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_DEWPOINT | <code>number</code> | <code>49</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RELATIVE_LEVEL | <code>number</code> | <code>50</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_ALTITUDE | <code>number</code> | <code>51</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_AREA | <code>number</code> | <code>52</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIANT_INTENSITY | <code>number</code> | <code>53</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_RADIANCE | <code>number</code> | <code>54</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_IRRADIANCE | <code>number</code> | <code>55</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPECTRAL_RADIANCE | <code>number</code> | <code>56</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SPECTRAL_IRRADIANCE | <code>number</code> | <code>57</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_PRESSURE | <code>number</code> | <code>58</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_DENSITY | <code>number</code> | <code>59</code> | 
| VSCP2_TYPE_MEASUREMENT_FLOAT_SOUND_LEVEL | <code>number</code> | <code>60</code> | 
| VSCP2_TYPE_VSCPD_GENERAL | <code>number</code> | <code>0</code> | 
| VSCP2_TYPE_VSCPD_LOOP | <code>number</code> | <code>1</code> | 
| VSCP2_TYPE_VSCPD_PAUSE | <code>number</code> | <code>3</code> | 
| VSCP2_TYPE_VSCPD_ACTIVATE | <code>number</code> | <code>4</code> | 
| VSCP2_TYPE_VSCPD_SECOND | <code>number</code> | <code>5</code> | 
| VSCP2_TYPE_VSCPD_MINUTE | <code>number</code> | <code>6</code> | 
| VSCP2_TYPE_VSCPD_HOUR | <code>number</code> | <code>7</code> | 
| VSCP2_TYPE_VSCPD_NOON | <code>number</code> | <code>8</code> | 
| VSCP2_TYPE_VSCPD_MIDNIGHT | <code>number</code> | <code>9</code> | 
| VSCP2_TYPE_VSCPD_WEEK | <code>number</code> | <code>11</code> | 
| VSCP2_TYPE_VSCPD_MONTH | <code>number</code> | <code>12</code> | 
| VSCP2_TYPE_VSCPD_QUARTER | <code>number</code> | <code>13</code> | 
| VSCP2_TYPE_VSCPD_YEAR | <code>number</code> | <code>14</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_MINUTE | <code>number</code> | <code>15</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_HOUR | <code>number</code> | <code>16</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_DAY | <code>number</code> | <code>17</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_WEEK | <code>number</code> | <code>18</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_MONTH | <code>number</code> | <code>19</code> | 
| VSCP2_TYPE_VSCPD_RANDOM_YEAR | <code>number</code> | <code>20</code> | 
| VSCP2_TYPE_VSCPD_DUSK | <code>number</code> | <code>21</code> | 
| VSCP2_TYPE_VSCPD_DAWN | <code>number</code> | <code>22</code> | 
| VSCP2_TYPE_VSCPD_STARTING_UP | <code>number</code> | <code>23</code> | 
| VSCP2_TYPE_VSCPD_SHUTTING_DOWN | <code>number</code> | <code>24</code> | 
| VSCP2_TYPE_VSCPD_TIMER_STARTED | <code>number</code> | <code>25</code> | 
| VSCP2_TYPE_VSCPD_TIMER_PAUSED | <code>number</code> | <code>26</code> | 
| VSCP2_TYPE_VSCPD_TIMER_RESUMED | <code>number</code> | <code>27</code> | 
| VSCP2_TYPE_VSCPD_TIMER_STOPPED | <code>number</code> | <code>28</code> | 
| VSCP2_TYPE_VSCPD_TIMER_ELLAPSED | <code>number</code> | <code>29</code> | 
| VSCP2_TYPE_VSCPD_NEW_CALCULATION | <code>number</code> | <code>30</code> | 

<a id="vscp.constants.priorities"></a>
#### constants.priorities : <code>enum</code>
VSCP class priorities

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| PRIORITY_0_HIGH | <code>number</code> | <code>0</code> | 
| PRIORITY_1 | <code>number</code> | <code>1</code> | 
| PRIORITY_2 | <code>number</code> | <code>2</code> | 
| PRIORITY_3_NORMAL | <code>number</code> | <code>3</code> | 
| PRIORITY_4 | <code>number</code> | <code>4</code> | 
| PRIORITY_5 | <code>number</code> | <code>5</code> | 
| PRIORITY_6 | <code>number</code> | <code>6</code> | 
| PRIORITY_7_LOW | <code>number</code> | <code>7</code> | 

<a id="vscp.constants.varTypes"></a>
#### constants.varTypes : <code>enum</code>
VSCP variable types

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| UNASSIGNED | <code>number</code> | <code>0</code> | 
| STRING | <code>number</code> | <code>1</code> | 
| BOOLEAN | <code>number</code> | <code>2</code> | 
| INTEGER | <code>number</code> | <code>3</code> | 
| LONG | <code>number</code> | <code>4</code> | 
| DOUBLE | <code>number</code> | <code>5</code> | 
| MEASUREMENT | <code>number</code> | <code>6</code> | 
| EVENT | <code>number</code> | <code>7</code> | 
| GUID | <code>number</code> | <code>8</code> | 
| EVENT_DATA | <code>number</code> | <code>9</code> | 
| EVENT_CLASS | <code>number</code> | <code>10</code> | 
| EVENT_TYPE | <code>number</code> | <code>11</code> | 
| EVENT_TIMESTAMP | <code>number</code> | <code>12</code> | 
| DATE_TIME | <code>number</code> | <code>13</code> | 
| DATE | <code>number</code> | <code>14</code> | 
| TIME | <code>number</code> | <code>15</code> | 
| BLOB | <code>number</code> | <code>16</code> | 
| MIME | <code>number</code> | <code>100</code> | 
| HTML | <code>number</code> | <code>101</code> | 
| JAVASCIPT | <code>number</code> | <code>102</code> | 
| JSON | <code>number</code> | <code>103</code> | 
| XML | <code>number</code> | <code>104</code> | 
| SQL | <code>number</code> | <code>105</code> | 
| LUA | <code>number</code> | <code>201</code> | 
| LUARES | <code>number</code> | <code>202</code> | 
| UXTYPE1 | <code>number</code> | <code>300</code> | 
| DMROW | <code>number</code> | <code>500</code> | 
| DRIVER | <code>number</code> | <code>501</code> | 
| USER | <code>number</code> | <code>502</code> | 
| FILTER | <code>number</code> | <code>503</code> | 

<a id="vscp.constants.varTypeNames"></a>
#### constants.varTypeNames
VSCP variable type names as string. Use to fill drop down boxes and similar.

**Kind**: static constant of <code>[constants](#vscp.constants)</code>  
<a id="vscp.utility"></a>
### vscp.utility : <code>object</code>
Utility functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.utility](#vscp.utility) : <code>object</code>
  * [.readValue(input)](#vscp.utility.readValue) ⇒ <code>number</code>
  * [.getTime()](#vscp.utility.getTime) ⇒ <code>string</code>
  * [.guidToStr(guid)](#vscp.utility.guidToStr) ⇒ <code>string</code>
  * [.strToGuid(guid)](#vscp.utility.strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
  * [.getNodeId(guid)](#vscp.utility.getNodeId) ⇒ <code>number</code>

<a id="vscp.utility.readValue"></a>
#### utility.readValue(input) ⇒ <code>number</code>
Read a hex or decimal value and return as an integer.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>number</code> - Value  

| Param | Type | Description |
| --- | --- | --- |
| input | <code>string</code> | Hex or decimal value as string |

<a id="vscp.utility.getTime"></a>
#### utility.getTime() ⇒ <code>string</code>
Utility function which returns the current time in the following format: hh:mm:ss.us

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>string</code> - Current time in the format hh:mm:ss.us  
<a id="vscp.utility.guidToStr"></a>
#### utility.guidToStr(guid) ⇒ <code>string</code>
Converts a GUID number array to a GUID string.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>string</code> - GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>Array.&lt;number&gt;</code> | GUID number array |

<a id="vscp.utility.strToGuid"></a>
#### utility.strToGuid(guid) ⇒ <code>Array.&lt;number&gt;</code>
Converts a GUID string to a GUID number array.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>Array.&lt;number&gt;</code> - GUID number array  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp.utility.getNodeId"></a>
#### utility.getNodeId(guid) ⇒ <code>number</code>
Get node id from a node GUID string.

**Kind**: static method of <code>[utility](#vscp.utility)</code>  
**Returns**: <code>number</code> - Node id  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp.rest"></a>
### vscp.rest : <code>object</code>
VSCP REST api functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.rest](#vscp.rest) : <code>object</code>
  * [.Client](#vscp.rest.Client)
    * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
    * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
    * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
    * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
    * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
    * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
    * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
    * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
    * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
    * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
    * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
    * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
    * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
    * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>

<a id="vscp.rest.Client"></a>
#### rest.Client
**Kind**: static class of <code>[rest](#vscp.rest)</code>  

* [.Client](#vscp.rest.Client)
  * [new vscp.rest.Client(config)](#new_vscp.rest.Client_new)
  * [.baseUrl](#vscp.rest.Client+baseUrl) : <code>string</code>
  * [.pathPrefix](#vscp.rest.Client+pathPrefix) : <code>string</code>
  * [.apiVersion](#vscp.rest.Client+apiVersion) : <code>string</code>
  * [.sessionKey](#vscp.rest.Client+sessionKey) : <code>string</code>
  * [._buildUrl(path)](#vscp.rest.Client+_buildUrl) ⇒
  * [._makeRequest(options)](#vscp.rest.Client+_makeRequest) ⇒ <code>object</code>
  * [._abort(error, [onError])](#vscp.rest.Client+_abort) ⇒ <code>object</code>
  * [.openSession(options)](#vscp.rest.Client+openSession) ⇒ <code>object</code>
  * [.closeSession([options])](#vscp.rest.Client+closeSession) ⇒ <code>object</code>
  * [.getStatus([options])](#vscp.rest.Client+getStatus) ⇒ <code>object</code>
  * [.sendEvent(options)](#vscp.rest.Client+sendEvent) ⇒ <code>object</code>
  * [.readEvent([options])](#vscp.rest.Client+readEvent) ⇒ <code>object</code>
  * [.setFilter(options)](#vscp.rest.Client+setFilter) ⇒ <code>object</code>
  * [.clearQueue([options])](#vscp.rest.Client+clearQueue) ⇒ <code>object</code>
  * [.createVar(options)](#vscp.rest.Client+createVar) ⇒ <code>object</code>
  * [.readVar(options)](#vscp.rest.Client+readVar) ⇒ <code>object</code>
  * [.writeVar(options)](#vscp.rest.Client+writeVar) ⇒ <code>object</code>
  * [.removeVar(options)](#vscp.rest.Client+removeVar) ⇒ <code>object</code>
  * [.listVar(options)](#vscp.rest.Client+listVar) ⇒ <code>object</code>

<a id="new_vscp.rest.Client_new"></a>
##### new vscp.rest.Client(config)
The VSCP client class handles the basic REST api of the VSCP daemon.
The function interface uses jquery ajax call in the background and will
return object with the jquery promise interface.


| Param | Type | Description |
| --- | --- | --- |
| config | <code>string</code> | Configuration |
| [config.baseUrl] | <code>string</code> | VSCP daemon URL (protocol + hostname + port) |
| [options.pathPrefix] | <code>string</code> | Path prefix (default: '/vscp'), which comes right after the base url. |
| [options.apiVersion] | <code>string</code> | API version (for future use) |

<a id="vscp.rest.Client+baseUrl"></a>
##### client.baseUrl : <code>string</code>
Base URL

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+pathPrefix"></a>
##### client.pathPrefix : <code>string</code>
Path prefix

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+apiVersion"></a>
##### client.apiVersion : <code>string</code>
REST API version (future use)

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+sessionKey"></a>
##### client.sessionKey : <code>string</code>
Session key

**Kind**: instance property of <code>[Client](#vscp.rest.Client)</code>  
<a id="vscp.rest.Client+_buildUrl"></a>
##### client._buildUrl(path) ⇒
Build complete URL, including command path.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: URL  

| Param | Type | Description |
| --- | --- | --- |
| path | <code>string</code> | Relative command path, after REST API version. |

<a id="vscp.rest.Client+_makeRequest"></a>
##### client._makeRequest(options) ⇒ <code>object</code>
Make a request to VSCP daemon via REST api.
The onSuccess and onError function parameter are harmonized here.
This makes it easier to process them further.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.path | <code>string</code> | Relative path |
| options.parameter | <code>Array.&lt;string&gt;</code> | Array of URL parameter |
| options.type | <code>string</code> | 'GET', 'POST', or etc. |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+_abort"></a>
##### client._abort(error, [onError]) ⇒ <code>object</code>
Prepare error object, call error callback and return rejected promise.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - Rejected jquery promise  

| Param | Type | Description |
| --- | --- | --- |
| error | <code>string</code> | Error description |
| [onError] | <code>function</code> | Callback |

<a id="vscp.rest.Client+openSession"></a>
##### client.openSession(options) ⇒ <code>object</code>
Open a session.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.user | <code>string</code> | User name |
| options.password | <code>string</code> | Password |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+closeSession"></a>
##### client.closeSession([options]) ⇒ <code>object</code>
Close a session.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+getStatus"></a>
##### client.getStatus([options]) ⇒ <code>object</code>
Get status and how many events are in the queue.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+sendEvent"></a>
##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>object</code> | VSCP event |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+readEvent"></a>
##### client.readEvent([options]) ⇒ <code>object</code>
Read one or more VSCP events.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.count] | <code>object</code> | Number of events to read |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+setFilter"></a>
##### client.setFilter(options) ⇒ <code>object</code>
Set filter.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+clearQueue"></a>
##### client.clearQueue([options]) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp.rest.Client+createVar"></a>
##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.type] | <code>number</code> | Variable type (default: string) |
| [options.accessrights] | <code>number</code> | Variable value (default: 744) |
| options.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| options.value | <code>string</code> | Variable Value |
| [options.note] | <code>string</code> | Variable note (optional) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+readVar"></a>
##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+writeVar"></a>
##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+removeVar"></a>
##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.rest.Client+listVar"></a>
##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of <code>[Client](#vscp.rest.Client)</code>  
**Returns**: <code>object</code> - jquery promise (deferred object)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.listLong | <code>boolean</code> | When false the variable list dos not include value and note. If set to true value and note is included. |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws"></a>
### vscp.ws : <code>object</code>
VSCP websocket api functions

**Kind**: static namespace of <code>[vscp](#vscp)</code>  

* [.ws](#vscp.ws) : <code>object</code>
  * [.Client](#vscp.ws.Client)
    * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
    * _instance_
      * [.states](#vscp.ws.Client+states) : <code>enum</code>
      * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
      * [.socket](#vscp.ws.Client+socket) : <code>object</code>
      * [.url](#vscp.ws.Client+url) : <code>string</code>
      * [.userName](#vscp.ws.Client+userName) : <code>string</code>
      * [.userId](#vscp.ws.Client+userId) : <code>number</code>
      * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
      * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
      * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
      * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
      * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
      * [.password](#vscp.ws.Client+password) : <code>string</code>
      * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
      * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
      * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
      * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
      * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
      * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
      * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
      * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
      * [.state](#vscp.ws.Client+state) : <code>number</code>
      * [.substate](#vscp.ws.Client+substate) : <code>number</code>
      * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
      * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
      * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
      * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
      * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
      * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
      * [.signalConnError()](#vscp.ws.Client+signalConnError)
      * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
      * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
      * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
      * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
      * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
      * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
      * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
      * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
      * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
      * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
      * [.connect(options)](#vscp.ws.Client+connect)
      * [.disconnect()](#vscp.ws.Client+disconnect)
      * [.start(options)](#vscp.ws.Client+start)
      * [.stop(options)](#vscp.ws.Client+stop)
      * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
      * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
      * [.setFilter(options)](#vscp.ws.Client+setFilter)
      * [.createVar(options)](#vscp.ws.Client+createVar)
      * [.readVar(options)](#vscp.ws.Client+readVar)
      * [.writeVar(options)](#vscp.ws.Client+writeVar)
      * [.resetVar(options)](#vscp.ws.Client+resetVar)
      * [.removeVar(options)](#vscp.ws.Client+removeVar)
      * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
      * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
      * [.listVar(options)](#vscp.ws.Client+listVar)
      * [.readTable(options)](#vscp.ws.Client+readTable)
    * _inner_
      * [~Command](#vscp.ws.Client..Command)
        * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
        * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
        * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
        * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
      * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
      * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>

<a id="vscp.ws.Client"></a>
#### ws.Client
**Kind**: static class of <code>[ws](#vscp.ws)</code>  

* [.Client](#vscp.ws.Client)
  * [new vscp.ws.Client()](#new_vscp.ws.Client_new)
  * _instance_
    * [.states](#vscp.ws.Client+states) : <code>enum</code>
    * [.substates](#vscp.ws.Client+substates) : <code>enum</code>
    * [.socket](#vscp.ws.Client+socket) : <code>object</code>
    * [.url](#vscp.ws.Client+url) : <code>string</code>
    * [.userName](#vscp.ws.Client+userName) : <code>string</code>
    * [.userId](#vscp.ws.Client+userId) : <code>number</code>
    * [.userFullname](#vscp.ws.Client+userFullname) : <code>string</code>
    * [.userRights](#vscp.ws.Client+userRights) : <code>array</code>
    * [.userRemotes](#vscp.ws.Client+userRemotes) : <code>array</code>
    * [.userEvents](#vscp.ws.Client+userEvents) : <code>array</code>
    * [.userNote](#vscp.ws.Client+userNote) : <code>string</code>
    * [.password](#vscp.ws.Client+password) : <code>string</code>
    * [.vscpkey](#vscp.ws.Client+vscpkey) : <code>string</code>
    * [.authdomain](#vscp.ws.Client+authdomain) : <code>string</code>
    * [.passwordHash](#vscp.ws.Client+passwordHash) : <code>string</code>
    * [.onConnError](#vscp.ws.Client+onConnError) : <code>function</code>
    * [.onMessage](#vscp.ws.Client+onMessage) : <code>function</code>
    * [.onEvent](#vscp.ws.Client+onEvent) : <code>Array.&lt;function()&gt;</code>
    * [.onVariable](#vscp.ws.Client+onVariable) : <code>function</code>
    * [.onTableRow](#vscp.ws.Client+onTableRow) : <code>function</code>
    * [.state](#vscp.ws.Client+state) : <code>number</code>
    * [.substate](#vscp.ws.Client+substate) : <code>number</code>
    * [.webSocketMessages](#vscp.ws.Client+webSocketMessages) : <code>object</code>
    * [.getPendingCommand(command)](#vscp.ws.Client+getPendingCommand) ⇒ <code>Command</code>
    * [._sendCommand(options)](#vscp.ws.Client+_sendCommand)
    * [._sendEvent(options)](#vscp.ws.Client+_sendEvent)
    * [.signalSuccess(command, [obj])](#vscp.ws.Client+signalSuccess)
    * [.signalError(command, [obj])](#vscp.ws.Client+signalError)
    * [.signalConnError()](#vscp.ws.Client+signalConnError)
    * [.signalMessage(msg)](#vscp.ws.Client+signalMessage) ⇒ <code>boolean</code>
    * [.signalEvent(vscpEvent)](#vscp.ws.Client+signalEvent)
    * [.signalVariable(variable)](#vscp.ws.Client+signalVariable)
    * [.signalTableRow(row)](#vscp.ws.Client+signalTableRow)
    * [.addEventListener(eventListener)](#vscp.ws.Client+addEventListener)
    * [.removeEventListener(eventListener)](#vscp.ws.Client+removeEventListener)
    * [.getAuthHash(userName, password, str_iv)](#vscp.ws.Client+getAuthHash) ⇒ <code>string</code>
    * [.onWebSocketOpen()](#vscp.ws.Client+onWebSocketOpen)
    * [.onWebSocketClose()](#vscp.ws.Client+onWebSocketClose)
    * [.onWebSocketMessage(msg)](#vscp.ws.Client+onWebSocketMessage)
    * [.connect(options)](#vscp.ws.Client+connect)
    * [.disconnect()](#vscp.ws.Client+disconnect)
    * [.start(options)](#vscp.ws.Client+start)
    * [.stop(options)](#vscp.ws.Client+stop)
    * [.clearQueue(options)](#vscp.ws.Client+clearQueue)
    * [.sendEvent(options)](#vscp.ws.Client+sendEvent)
    * [.setFilter(options)](#vscp.ws.Client+setFilter)
    * [.createVar(options)](#vscp.ws.Client+createVar)
    * [.readVar(options)](#vscp.ws.Client+readVar)
    * [.writeVar(options)](#vscp.ws.Client+writeVar)
    * [.resetVar(options)](#vscp.ws.Client+resetVar)
    * [.removeVar(options)](#vscp.ws.Client+removeVar)
    * [.lengthVar(options)](#vscp.ws.Client+lengthVar)
    * [.lastChangeVar(options)](#vscp.ws.Client+lastChangeVar)
    * [.listVar(options)](#vscp.ws.Client+listVar)
    * [.readTable(options)](#vscp.ws.Client+readTable)
  * _inner_
    * [~Command](#vscp.ws.Client..Command)
      * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
      * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
      * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
      * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>
    * [~cmdQueue](#vscp.ws.Client..cmdQueue) : <code>Array.&lt;Command&gt;</code>
    * [~getPendingCommandIndex(command)](#vscp.ws.Client..getPendingCommandIndex) ⇒ <code>number</code>

<a id="new_vscp.ws.Client_new"></a>
##### new vscp.ws.Client()
VSCP websocket client, used for connection establishment to a VSCP server.

<a id="vscp.ws.Client+states"></a>
##### client.states : <code>enum</code>
States of the VSCP websocket

**Kind**: instance enum property of <code>[Client](#vscp.ws.Client)</code>  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| DISCONNECTED | <code>number</code> | <code>0</code> | Not connected |
| CONNECTED | <code>number</code> | <code>1</code> | Standard websocket connection established |
| AUTHENTICATED | <code>number</code> | <code>2</code> | Authentication with VSCP server successful |

<a id="vscp.ws.Client+substates"></a>
##### client.substates : <code>enum</code>
Substates of the VSCP websocket

**Kind**: instance enum property of <code>[Client](#vscp.ws.Client)</code>  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| CLOSED | <code>number</code> | <code>0</code> | No events sent from server |
| OPEN | <code>number</code> | <code>1</code> | Events sent from server |

<a id="vscp.ws.Client+socket"></a>
##### client.socket : <code>object</code>
Websocket

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+url"></a>
##### client.url : <code>string</code>
url used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userName"></a>
##### client.userName : <code>string</code>
User name used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userId"></a>
##### client.userId : <code>number</code>
User id from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userFullname"></a>
##### client.userFullname : <code>string</code>
User full name from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userRights"></a>
##### client.userRights : <code>array</code>
User rights from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userRemotes"></a>
##### client.userRemotes : <code>array</code>
User allowed remotes from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userEvents"></a>
##### client.userEvents : <code>array</code>
User allowed events from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+userNote"></a>
##### client.userNote : <code>string</code>
User note from authentication AUTH1

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+password"></a>
##### client.password : <code>string</code>
Password used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+vscpkey"></a>
##### client.vscpkey : <code>string</code>
Secret key used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+authdomain"></a>
##### client.authdomain : <code>string</code>
authdomain used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+passwordHash"></a>
##### client.passwordHash : <code>string</code>
Password hash used for connection establishment

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onConnError"></a>
##### client.onConnError : <code>function</code>
Callback called on any connection error

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onMessage"></a>
##### client.onMessage : <code>function</code>
Callback called on any received VSCP response message

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onEvent"></a>
##### client.onEvent : <code>Array.&lt;function()&gt;</code>
Callbacks called on any received VSCP event message

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onVariable"></a>
##### client.onVariable : <code>function</code>
Callback called on any received variable (see LSTVAR command)

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onTableRow"></a>
##### client.onTableRow : <code>function</code>
Callback called on any received table row (see GT command)

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+state"></a>
##### client.state : <code>number</code>
VSCP websocket is not connected right now

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+substate"></a>
##### client.substate : <code>number</code>
VSCP event traffic is closed

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+webSocketMessages"></a>
##### client.webSocketMessages : <code>object</code>
VSCP websocket command responses and unsolicited messages

**Kind**: instance property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+getPendingCommand"></a>
##### client.getPendingCommand(command) ⇒ <code>Command</code>
Get command from queue with pending commands.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>Command</code> - Command object  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |

<a id="vscp.ws.Client+_sendCommand"></a>
##### client._sendCommand(options)
Send command to VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.command | <code>string</code> | Command string |
| options.data | <code>string</code> | Data string |
| options.simulate | <code>boolean</code> | Simulate the command (true/false) |
| options.onSuccess | <code>function</code> | Callback on success |
| options.onError | <code>function</code> | Callback on error |

<a id="vscp.ws.Client+_sendEvent"></a>
##### client._sendEvent(options)
Send event to VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.data | <code>string</code> | Data string |
| options.onSuccess | <code>function</code> | Callback on success |
| options.onError | <code>function</code> | Callback on error |

<a id="vscp.ws.Client+signalSuccess"></a>
##### client.signalSuccess(command, [obj])
Signal success of the current asynchronous operation.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| [obj] | <code>object</code> | Options for on success callback |

<a id="vscp.ws.Client+signalError"></a>
##### client.signalError(command, [obj])
Signal failed of the current asynchronous operation.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| [obj] | <code>object</code> | Options for on error callback |

<a id="vscp.ws.Client+signalConnError"></a>
##### client.signalConnError()
Signal a connection error.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+signalMessage"></a>
##### client.signalMessage(msg) ⇒ <code>boolean</code>
Signal a received VSCP response message.
If the message is handled by the application, the application will return
true, which means no further actions shall take place in this object.
Otherwise the message is handled by the standard onMessage handler here.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>boolean</code> - Message is handled (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp.ws.Client+signalEvent"></a>
##### client.signalEvent(vscpEvent)
Signal a received VSCP event.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| vscpEvent | <code>[Event](#vscp.Event)</code> | VSCP event |

<a id="vscp.ws.Client+signalVariable"></a>
##### client.signalVariable(variable)
Signal a received variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| variable | <code>object</code> | Variable object |
| variable.id | <code>number</code> | Consecutive number |
| variable.name | <code>string</code> | Variable name |
| variable.type | <code>string</code> | Variable type |
| variable.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| variable.value | <code>string</code> | Variable value |

<a id="vscp.ws.Client+signalTableRow"></a>
##### client.signalTableRow(row)
Signal a received table row.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| row | <code>object</code> | Table row object |
| row.date | <code>string</code> | Date and time |
| row.value | <code>string</code> | Value |

<a id="vscp.ws.Client+addEventListener"></a>
##### client.addEventListener(eventListener)
Add a event listener.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp.ws.Client+removeEventListener"></a>
##### client.removeEventListener(eventListener)
Remove a event listener.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp.ws.Client+getAuthHash"></a>
##### client.getAuthHash(userName, password, str_iv) ⇒ <code>string</code>
Calculates the VSCP server websocket authentication hash.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>string</code> - Authentication ("encrypted user:password")  

| Param | Type | Description |
| --- | --- | --- |
| userName | <code>string</code> | User name |
| password | <code>string</code> | Password |
| str_iv | <code>string</code> | 16 random byte iv in hex form |

<a id="vscp.ws.Client+onWebSocketOpen"></a>
##### client.onWebSocketOpen()
This function is called by the websocket in case the connection is established.
It will initiate the authentication with the VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onWebSocketClose"></a>
##### client.onWebSocketClose()
This function is called by the websocket in case that the connection is closed.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+onWebSocketMessage"></a>
##### client.onWebSocketMessage(msg)
This function is called for any websocket message (VSCP server response message).

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp.ws.Client+connect"></a>
##### client.connect(options)
Connect to a VSCP server with the given URL.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.url | <code>string</code> | URL to the VSCP server, e.g. ws:// |
| options.userName | <code>string</code> | User name used for authentication |
| options.password | <code>string</code> | Password used for authentication |
| options.vscpkey | <code>string</code> | Secret key used for authentication |
| [options.onMessage] | <code>function</code> | Function which is called on any received VSCP response message. |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful connection establishment. |
| [options.onError] | <code>function</code> | Function which is called on a failed connection establishment or in case the connection is lost during the session. |

<a id="vscp.ws.Client+disconnect"></a>
##### client.disconnect()
Disconnect from a VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client+start"></a>
##### client.start(options)
Start receiving events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+stop"></a>
##### client.stop(options)
Stop receiving events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+clearQueue"></a>
##### client.clearQueue(options)
Clear the VSCP event queue on the server side.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+sendEvent"></a>
##### client.sendEvent(options)
Send a VSCP event to the VSCP server.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>[Event](#vscp.Event)</code> | VSCP event to send |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+setFilter"></a>
##### client.setFilter(options)
Set a filter in the VSCP server for VSCP events.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> &#124; <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+createVar"></a>
##### client.createVar(options)
Create a a VSCP remote variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.type] | <code>number</code> | Variable type (default: string) |
| [options.accessrights] | <code>number</code> | Variable value (default: 744) |
| options.persistency | <code>boolean</code> | Variable is persistent (true) or not (false) |
| options.value | <code>string</code> | Variable Value |
| [options.note] | <code>string</code> | Variable note (optional) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+readVar"></a>
##### client.readVar(options)
Read a value from a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+writeVar"></a>
##### client.writeVar(options)
Write a value to a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+resetVar"></a>
##### client.resetVar(options)
Reset a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+removeVar"></a>
##### client.removeVar(options)
Remove a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+lengthVar"></a>
##### client.lengthVar(options)
Get a VSCP server variable length.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+lastChangeVar"></a>
##### client.lastChangeVar(options)
Get last change of a VSCP server variable.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+listVar"></a>
##### client.listVar(options)
List all VSCP server variables.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| options.onVariable | <code>function</code> | Function which is called per variable |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client+readTable"></a>
##### client.readTable(options)
Get data from a table.
If "begin" and "end" are omitted, the whole table is returned.

**Kind**: instance method of <code>[Client](#vscp.ws.Client)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Table name |
| options.begin | <code>string</code> | Date when to begin ( ISO form YY-MM-DD HH:MM:SS ) |
| options.end | <code>string</code> | Date when to end ( ISO form YY-MM-DD HH:MM:SS ) |
| options.onTableRow | <code>function</code> | Function which is called on every received table row |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp.ws.Client..Command"></a>
##### Client~Command
**Kind**: inner class of <code>[Client](#vscp.ws.Client)</code>  

  * [~Command](#vscp.ws.Client..Command)
    * [new Command(command, onSuccess, onerror)](#new_vscp.ws.Client..Command_new)
    * [.command](#vscp.ws.Client..Command+command) : <code>string</code>
    * [.onSuccess](#vscp.ws.Client..Command+onSuccess) : <code>function</code>
    * [.onError](#vscp.ws.Client..Command+onError) : <code>function</code>

<a id="new_vscp.ws.Client..Command_new"></a>
###### new Command(command, onSuccess, onerror)
VSCP server command


| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |
| onSuccess | <code>function</code> | Function which is called on successful operation |
| onerror | <code>function</code> | Function which is called on failed operation |

<a id="vscp.ws.Client..Command+command"></a>
###### command.command : <code>string</code>
Server command string

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..Command+onSuccess"></a>
###### command.onSuccess : <code>function</code>
Function which is called on successful operation

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..Command+onError"></a>
###### command.onError : <code>function</code>
Function which is called on failed operation

**Kind**: instance property of <code>[Command](#vscp.ws.Client..Command)</code>  
<a id="vscp.ws.Client..cmdQueue"></a>
##### Client~cmdQueue : <code>Array.&lt;Command&gt;</code>
Queue contains all pending VSCP server commands

**Kind**: inner property of <code>[Client](#vscp.ws.Client)</code>  
<a id="vscp.ws.Client..getPendingCommandIndex"></a>
##### Client~getPendingCommandIndex(command) ⇒ <code>number</code>
Get the index of a command in the queue.

**Kind**: inner method of <code>[Client](#vscp.ws.Client)</code>  
**Returns**: <code>number</code> - Index of command in the queue. If index is < 0, the command was not found.  

| Param | Type | Description |
| --- | --- | --- |
| command | <code>string</code> | Server command string |

<a id="vscp._createNS"></a>
### vscp._createNS(namespace)
Create a general purpose namespace method. This will allow us to create
namespace a bit easier.

**Kind**: static method of <code>[vscp](#vscp)</code>  

| Param | Type | Description |
| --- | --- | --- |
| namespace | <code>string</code> | Complete namespace, e.g. "a.b.c.d" |

<a id="vscp.getVarTypeName"></a>
### vscp.getVarTypeName(n) ⇒ <code>string</code>
Get variable type name as string by numerical code.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Variable type name  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Numerical code |

<a id="vscp.getVarTypeNumerical"></a>
### vscp.getVarTypeNumerical(str) ⇒ <code>number</code>
Get numerical code of variable type from string.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>number</code> - Variable type numerical code  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Variable type name |

<a id="vscp.getEditorModeFromType"></a>
### vscp.getEditorModeFromType(n) ⇒ <code>string</code>
Get ace editor formation mode string from numerical variable type code.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Ace editro formation mode string  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Variable type numerical code |

<a id="vscp.b64EncodeUnicode"></a>
### vscp.b64EncodeUnicode(str) ⇒ <code>string</code>
Encode base64 unicode safe.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Base64  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Unicode string |

<a id="vscp.b64DecodeUnicode"></a>
### vscp.b64DecodeUnicode(str) ⇒ <code>string</code>
Decode base64 unicode safe.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Unicode string  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Base64 |

<a id="vscp.isBase64Type"></a>
### vscp.isBase64Type(type) ⇒ <code>bool</code>
Determine whether the given variable type is a type stored base64 encoded or not.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>bool</code> - Stored base64 encoded (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |

<a id="vscp.decodeValueIfBase64"></a>
### vscp.decodeValueIfBase64(type, value) ⇒ <code>string</code>
Decode the value if its base64 encoded.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Decoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |

<a id="vscp.encodeValueIfBase64"></a>
### vscp.encodeValueIfBase64(type, value) ⇒ <code>string</code>
Encode the value if its stored in base64.

**Kind**: static method of <code>[vscp](#vscp)</code>  
**Returns**: <code>string</code> - Encoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |


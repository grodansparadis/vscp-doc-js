<a id="vscp"></a>

## vscp : <code>object</code>
Namespace for all functionality of the VSCP provided libraries.

**Kind**: global namespace  

* [vscp](#vscp) : <code>object</code>
    * [.Event](#vscp_dot_Event)
        * [new vscp.Event(options)](#new_vscp_dot_Event_new)
        * [.vscpHead](#vscp_dot_Event_and_vscpHead) : <code>number</code>
        * [.vscpClass](#vscp_dot_Event_and_vscpClass) : <code>number</code>
        * [.vscpType](#vscp_dot_Event_and_vscpType) : <code>number</code>
        * [.vscpObId](#vscp_dot_Event_and_vscpObId) : <code>number</code>
        * [.vscpTimeStamp](#vscp_dot_Event_and_vscpTimeStamp) : <code>number</code>
        * [.vscpDateTime](#vscp_dot_Event_and_vscpDateTime) : <code>date</code>
        * [.vscpGuid](#vscp_dot_Event_and_vscpGuid) : <code>string</code>
        * [.vscpData](#vscp_dot_Event_and_vscpData) : <code>Array.&lt;number&gt;</code> \| <code>string</code>
        * [.setIPV6Addr()](#vscp_dot_Event_and_setIPV6Addr)
        * [.isIPV6Addr()](#vscp_dot_Event_and_isIPV6Addr) ⇒ <code>boolean</code>
        * [.setDumbNode()](#vscp_dot_Event_and_setDumbNode)
        * [.isDumbNode()](#vscp_dot_Event_and_isDumbNode) ⇒ <code>boolean</code>
        * [.setPriority(priority)](#vscp_dot_Event_and_setPriority)
        * [.getPriority()](#vscp_dot_Event_and_getPriority) ⇒ <code>number</code>
        * [.setHardCodedAddr()](#vscp_dot_Event_and_setHardCodedAddr)
        * [.isHardCodedAddr()](#vscp_dot_Event_and_isHardCodedAddr) ⇒ <code>boolean</code>
        * [.setDoNotCalcCRC()](#vscp_dot_Event_and_setDoNotCalcCRC)
        * [.isDoNotCalcCRC()](#vscp_dot_Event_and_isDoNotCalcCRC) ⇒ <code>boolean</code>
        * [.getText()](#vscp_dot_Event_and_getText) ⇒ <code>string</code>
    * [.version](#vscp_dot_version)
    * [.constants](#vscp_dot_constants) : <code>object</code>
        * [.classes](#vscp_dot_constants_dot_classes) : <code>enum</code>
        * [.types](#vscp_dot_constants_dot_types) : <code>enum</code>
        * [.priorities](#vscp_dot_constants_dot_priorities) : <code>enum</code>
        * [.varTypes](#vscp_dot_constants_dot_varTypes) : <code>enum</code>
        * [.varTypeNames](#vscp_dot_constants_dot_varTypeNames)
    * [.utility](#vscp_dot_utility) : <code>object</code>
        * [.readValue(input)](#vscp_dot_utility_dot_readValue) ⇒ <code>number</code>
        * [.getTime()](#vscp_dot_utility_dot_getTime) ⇒ <code>string</code>
        * [.guidToStr(guid)](#vscp_dot_utility_dot_guidToStr) ⇒ <code>string</code>
        * [.strToGuid(guid)](#vscp_dot_utility_dot_strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
        * [.getNodeId(guid)](#vscp_dot_utility_dot_getNodeId) ⇒ <code>number</code>
    * [.mdf](#vscp_dot_mdf) : <code>object</code>
        * [.Register](#vscp_dot_mdf_dot_Register)
            * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
            * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
            * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
            * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
            * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
            * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
            * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
            * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
            * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
            * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
            * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)
        * [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
            * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
            * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
            * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
            * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
            * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
            * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
            * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
            * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
            * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
            * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
            * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
            * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
            * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
            * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)
        * [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
            * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
            * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
            * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
            * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)
        * [.timeout](#vscp_dot_mdf_dot_timeout) : <code>number</code>
        * [.load(options)](#vscp_dot_mdf_dot_load)
        * [.loadLocal(options)](#vscp_dot_mdf_dot_loadLocal)
        * [.readAbstractValue(options)](#vscp_dot_mdf_dot_readAbstractValue)
        * [.writeAbstractValue(options)](#vscp_dot_mdf_dot_writeAbstractValue)
        * [.writeAbstractBits(options)](#vscp_dot_mdf_dot_writeAbstractBits)
        * [.getRegisters(options)](#vscp_dot_mdf_dot_getRegisters) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
        * [.getAbstractions(options)](#vscp_dot_mdf_dot_getAbstractions) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)
    * [.measurement](#vscp_dot_measurement) : <code>object</code>
        * [.Decoder](#vscp_dot_measurement_dot_Decoder)
            * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
            * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
            * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
            * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>
        * [.constants](#vscp_dot_measurement_dot_constants) : <code>object</code>
            * [.units](#vscp_dot_measurement_dot_constants_dot_units) : <code>Array.&lt;string&gt;</code>
        * [.timeout](#vscp_dot_measurement_dot_timeout) : <code>number</code>
        * [.toFixed(value, precision)](#vscp_dot_measurement_dot_toFixed) ⇒ <code>number</code>
        * [.varInteger2Float(data)](#vscp_dot_measurement_dot_varInteger2Float) ⇒ <code>number</code>
        * [.getDataCoding(data)](#vscp_dot_measurement_dot_getDataCoding) ⇒ <code>number</code>
        * [.getUnitFromDataCoding(data)](#vscp_dot_measurement_dot_getUnitFromDataCoding) ⇒ <code>number</code>
        * [.getSensorIndexFromDataCoding(data)](#vscp_dot_measurement_dot_getSensorIndexFromDataCoding) ⇒ <code>number</code>
        * [.decodeClass10(data)](#vscp_dot_measurement_dot_decodeClass10) ⇒ <code>number</code>
        * [.decodeClass60Number(data)](#vscp_dot_measurement_dot_decodeClass60Number) ⇒ <code>number</code>
        * [.decodeClass65Number(data)](#vscp_dot_measurement_dot_decodeClass65Number) ⇒ <code>number</code>
        * [.convertFahrenheitToKelvin(value)](#vscp_dot_measurement_dot_convertFahrenheitToKelvin) ⇒ <code>number</code>
        * [.convertFahrenheitToCelsius(value)](#vscp_dot_measurement_dot_convertFahrenheitToCelsius) ⇒ <code>number</code>
        * [.convertCelsiusToFahrenheit(value)](#vscp_dot_measurement_dot_convertCelsiusToFahrenheit) ⇒ <code>number</code>
        * [.convertKelvinToCelsius(value)](#vscp_dot_measurement_dot_convertKelvinToCelsius) ⇒ <code>number</code>
        * [.convertCelsiusToKelvin(value)](#vscp_dot_measurement_dot_convertCelsiusToKelvin) ⇒ <code>number</code>
        * [.convertKelvinToFahrenheit(value)](#vscp_dot_measurement_dot_convertKelvinToFahrenheit) ⇒ <code>number</code>
        * [.convertMeterToFeet(value)](#vscp_dot_measurement_dot_convertMeterToFeet) ⇒ <code>number</code>
        * [.convertFeetToMeter(value)](#vscp_dot_measurement_dot_convertFeetToMeter) ⇒ <code>number</code>
        * [.convertMeterToInch(value)](#vscp_dot_measurement_dot_convertMeterToInch) ⇒ <code>number</code>
        * [.convertInchToMeter(value)](#vscp_dot_measurement_dot_convertInchToMeter) ⇒ <code>number</code>
    * [.register](#vscp_dot_register) : <code>object</code>
        * [.constants](#vscp_dot_register_dot_constants) : <code>enum</code>
        * [.timeout](#vscp_dot_register_dot_timeout) : <code>number</code>
        * [.read(options)](#vscp_dot_register_dot_read)
        * [.write(options)](#vscp_dot_register_dot_write)
        * [.writeBits(options)](#vscp_dot_register_dot_writeBits)
        * [.readAlarmStatus(options)](#vscp_dot_register_dot_readAlarmStatus)
        * [.readVscpVersion(options)](#vscp_dot_register_dot_readVscpVersion)
        * [.readNodeControlFlags(options)](#vscp_dot_register_dot_readNodeControlFlags)
        * [.readUserId(options)](#vscp_dot_register_dot_readUserId)
        * [.readManufacturerDevId(options)](#vscp_dot_register_dot_readManufacturerDevId)
        * [.readManufacturerSubDevId(options)](#vscp_dot_register_dot_readManufacturerSubDevId)
        * [.readNicknameId(options)](#vscp_dot_register_dot_readNicknameId)
        * [.readSelectedPage(options)](#vscp_dot_register_dot_readSelectedPage)
        * [.readFirmwareVersion(options)](#vscp_dot_register_dot_readFirmwareVersion)
        * [.readBootloaderAlgorithm(options)](#vscp_dot_register_dot_readBootloaderAlgorithm)
        * [.readUsedPages(options)](#vscp_dot_register_dot_readUsedPages)
        * [.readStdDevFamCode(options)](#vscp_dot_register_dot_readStdDevFamCode)
        * [.readStdDevType(options)](#vscp_dot_register_dot_readStdDevType)
        * [.readGUID(options)](#vscp_dot_register_dot_readGUID)
        * [.readMdfUrl(options)](#vscp_dot_register_dot_readMdfUrl)
    * [.rest](#vscp_dot_rest) : <code>object</code>
        * [.Client](#vscp_dot_rest_dot_Client)
            * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
            * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
            * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
            * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
            * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
            * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
            * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
            * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
            * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
            * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
            * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
            * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
            * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
            * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
            * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
            * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
            * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>
    * [.service](#vscp_dot_service) : <code>object</code>
        * [.Container](#vscp_dot_service_dot_Container)
            * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
            * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
            * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
            * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
            * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
            * [.create(options)](#vscp_dot_service_dot_Container_and_create)
            * [.write(options)](#vscp_dot_service_dot_Container_and_write)
            * [.read(options)](#vscp_dot_service_dot_Container_and_read)
        * [.timeout](#vscp_dot_service_dot_timeout) : <code>number</code>
        * [.whoIsThere(options)](#vscp_dot_service_dot_whoIsThere)
        * [.scan(options)](#vscp_dot_service_dot_scan)
    * [.widget](#vscp_dot_widget) : <code>object</code>
        * [.Button](#vscp_dot_widget_dot_Button)
            * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
            * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
            * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)
        * [.Thermometer](#vscp_dot_widget_dot_Thermometer)
            * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
            * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
            * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)
        * [.generateUUID()](#vscp_dot_widget_dot_generateUUID) ⇒ <code>string</code>
        * [.Image(options)](#vscp_dot_widget_dot_Image)
    * [.wizard](#vscp_dot_wizard) : <code>object</code>
        * [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
            * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
            * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
            * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
            * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
            * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
            * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
            * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
            * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)
        * [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
            * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
            * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
            * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
            * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
            * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
            * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)
        * [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
            * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
            * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
            * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
            * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
            * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)
        * [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
            * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
            * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
            * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
            * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)
        * [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
            * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
            * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
            * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
            * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)
        * [.Recipe](#vscp_dot_wizard_dot_Recipe)
            * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
            * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
            * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
            * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
            * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
            * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
            * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
            * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
            * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
            * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
            * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)
        * [.getRecipes(options)](#vscp_dot_wizard_dot_getRecipes) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)
    * [.ws](#vscp_dot_ws) : <code>object</code>
        * [.Client](#vscp_dot_ws_dot_Client)
            * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
            * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
            * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
            * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
            * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
            * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
            * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
            * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
            * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
            * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
            * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
            * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
            * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
            * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
            * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
            * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
            * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
            * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
            * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
            * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
            * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
            * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
            * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
            * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
            * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
            * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
            * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
            * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
            * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
            * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
            * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
            * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
            * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
            * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
            * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
            * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
            * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
            * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
            * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
            * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
            * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
            * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
            * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
            * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
            * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>
    * [.getVarTypeName(n)](#vscp_dot_getVarTypeName) ⇒ <code>string</code>
    * [.getVarTypeNumerical(str)](#vscp_dot_getVarTypeNumerical) ⇒ <code>number</code>
    * [.getEditorModeFromType(n)](#vscp_dot_getEditorModeFromType) ⇒ <code>string</code>
    * [.b64EncodeUnicode(str)](#vscp_dot_b64EncodeUnicode) ⇒ <code>string</code>
    * [.b64DecodeUnicode(str)](#vscp_dot_b64DecodeUnicode) ⇒ <code>string</code>
    * [.isBase64Type(type)](#vscp_dot_isBase64Type) ⇒ <code>bool</code>
    * [.decodeValueIfBase64(type, value)](#vscp_dot_decodeValueIfBase64) ⇒ <code>string</code>
    * [.encodeValueIfBase64(type, value)](#vscp_dot_encodeValueIfBase64) ⇒ <code>string</code>

<a id="vscp_dot_Event"></a>

### vscp.Event
**Kind**: static class of [<code>vscp</code>](#vscp)  

* [.Event](#vscp_dot_Event)
    * [new vscp.Event(options)](#new_vscp_dot_Event_new)
    * [.vscpHead](#vscp_dot_Event_and_vscpHead) : <code>number</code>
    * [.vscpClass](#vscp_dot_Event_and_vscpClass) : <code>number</code>
    * [.vscpType](#vscp_dot_Event_and_vscpType) : <code>number</code>
    * [.vscpObId](#vscp_dot_Event_and_vscpObId) : <code>number</code>
    * [.vscpTimeStamp](#vscp_dot_Event_and_vscpTimeStamp) : <code>number</code>
    * [.vscpDateTime](#vscp_dot_Event_and_vscpDateTime) : <code>date</code>
    * [.vscpGuid](#vscp_dot_Event_and_vscpGuid) : <code>string</code>
    * [.vscpData](#vscp_dot_Event_and_vscpData) : <code>Array.&lt;number&gt;</code> \| <code>string</code>
    * [.setIPV6Addr()](#vscp_dot_Event_and_setIPV6Addr)
    * [.isIPV6Addr()](#vscp_dot_Event_and_isIPV6Addr) ⇒ <code>boolean</code>
    * [.setDumbNode()](#vscp_dot_Event_and_setDumbNode)
    * [.isDumbNode()](#vscp_dot_Event_and_isDumbNode) ⇒ <code>boolean</code>
    * [.setPriority(priority)](#vscp_dot_Event_and_setPriority)
    * [.getPriority()](#vscp_dot_Event_and_getPriority) ⇒ <code>number</code>
    * [.setHardCodedAddr()](#vscp_dot_Event_and_setHardCodedAddr)
    * [.isHardCodedAddr()](#vscp_dot_Event_and_isHardCodedAddr) ⇒ <code>boolean</code>
    * [.setDoNotCalcCRC()](#vscp_dot_Event_and_setDoNotCalcCRC)
    * [.isDoNotCalcCRC()](#vscp_dot_Event_and_isDoNotCalcCRC) ⇒ <code>boolean</code>
    * [.getText()](#vscp_dot_Event_and_getText) ⇒ <code>string</code>

<a id="new_vscp_dot_Event_new"></a>

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
| options.vscpData | <code>Array.&lt;number&gt;</code> \| <code>string</code> | Event data |

<a id="vscp_dot_Event_and_vscpHead"></a>

#### event.vscpHead : <code>number</code>
VSCP event head

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpClass"></a>

#### event.vscpClass : <code>number</code>
VSCP class

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpType"></a>

#### event.vscpType : <code>number</code>
VSCP type

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpObId"></a>

#### event.vscpObId : <code>number</code>
VSCP object id used by driver for channel info and etc.

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpTimeStamp"></a>

#### event.vscpTimeStamp : <code>number</code>
Relative timestamp for package in us

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpDateTime"></a>

#### event.vscpDateTime : <code>date</code>
Date/Time for package

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpGuid"></a>

#### event.vscpGuid : <code>string</code>
Node global unique id LSB(15) -> MSB(0)

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpData"></a>

#### event.vscpData : <code>Array.&lt;number&gt;</code> \| <code>string</code>
Data array or string

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_setIPV6Addr"></a>

#### event.setIPV6Addr()
Set GUID as IP v6 address

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isIPV6Addr"></a>

#### event.isIPV6Addr() ⇒ <code>boolean</code>
Is GUID a IP v6 address or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the GUID is a IP v6 address, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setDumbNode"></a>

#### event.setDumbNode()
Set dumb node. No MDF, registers, nothing.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isDumbNode"></a>

#### event.isDumbNode() ⇒ <code>boolean</code>
Is node a dump node or not?
Dumb node means no MDF, registers, nothing.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the node is a dumb node, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setPriority"></a>

#### event.setPriority(priority)
Set the VSCP event priority.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  

| Param | Type | Description |
| --- | --- | --- |
| priority | <code>number</code> | Priority |

<a id="vscp_dot_Event_and_getPriority"></a>

#### event.getPriority() ⇒ <code>number</code>
Get the VSCP event priority.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>number</code> - Priority of the event.  
<a id="vscp_dot_Event_and_setHardCodedAddr"></a>

#### event.setHardCodedAddr()
Set the node id of the event sender as hard coded?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isHardCodedAddr"></a>

#### event.isHardCodedAddr() ⇒ <code>boolean</code>
Is the node id of the event sender hard coded or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the node id is hard coded, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setDoNotCalcCRC"></a>

#### event.setDoNotCalcCRC()
Set flag for no CRC calculation?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isDoNotCalcCRC"></a>

#### event.isDoNotCalcCRC() ⇒ <code>boolean</code>
Is CRC calculated or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If nor CRC should be calculated true is returned.  
<a id="vscp_dot_Event_and_getText"></a>

#### event.getText() ⇒ <code>string</code>
Get event as string.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>string</code> - Event as string  
<a id="vscp_dot_version"></a>

### vscp.version
VSCP websocket library version

**Kind**: static property of [<code>vscp</code>](#vscp)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| major | <code>number</code> | Major version number |
| minor | <code>number</code> | Minor version number |
| patch | <code>number</code> | Sub-minor version number |

<a id="vscp_dot_constants"></a>

### vscp.constants : <code>object</code>
VSCP constants

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.constants](#vscp_dot_constants) : <code>object</code>
    * [.classes](#vscp_dot_constants_dot_classes) : <code>enum</code>
    * [.types](#vscp_dot_constants_dot_types) : <code>enum</code>
    * [.priorities](#vscp_dot_constants_dot_priorities) : <code>enum</code>
    * [.varTypes](#vscp_dot_constants_dot_varTypes) : <code>enum</code>
    * [.varTypeNames](#vscp_dot_constants_dot_varTypeNames)

<a id="vscp_dot_constants_dot_classes"></a>

#### constants.classes : <code>enum</code>
VSCP classes

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_types"></a>

#### constants.types : <code>enum</code>
VSCP class types

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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
| VSCP_TYPE_INFORMATION_DATETIME | <code>number</code> | <code>77</code> | 
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

<a id="vscp_dot_constants_dot_priorities"></a>

#### constants.priorities : <code>enum</code>
VSCP class priorities

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_varTypes"></a>

#### constants.varTypes : <code>enum</code>
VSCP variable types

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_varTypeNames"></a>

#### constants.varTypeNames
VSCP variable type names as string. Use to fill drop down boxes and similar.

**Kind**: static constant of [<code>constants</code>](#vscp_dot_constants)  
<a id="vscp_dot_utility"></a>

### vscp.utility : <code>object</code>
Utility functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.utility](#vscp_dot_utility) : <code>object</code>
    * [.readValue(input)](#vscp_dot_utility_dot_readValue) ⇒ <code>number</code>
    * [.getTime()](#vscp_dot_utility_dot_getTime) ⇒ <code>string</code>
    * [.guidToStr(guid)](#vscp_dot_utility_dot_guidToStr) ⇒ <code>string</code>
    * [.strToGuid(guid)](#vscp_dot_utility_dot_strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
    * [.getNodeId(guid)](#vscp_dot_utility_dot_getNodeId) ⇒ <code>number</code>

<a id="vscp_dot_utility_dot_readValue"></a>

#### utility.readValue(input) ⇒ <code>number</code>
Read a hex or decimal value and return as an integer.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>number</code> - Value  

| Param | Type | Description |
| --- | --- | --- |
| input | <code>string</code> | Hex or decimal value as string |

<a id="vscp_dot_utility_dot_getTime"></a>

#### utility.getTime() ⇒ <code>string</code>
Utility function which returns the current time in the following format: hh:mm:ss.us

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>string</code> - Current time in the format hh:mm:ss.us  
<a id="vscp_dot_utility_dot_guidToStr"></a>

#### utility.guidToStr(guid) ⇒ <code>string</code>
Converts a GUID number array to a GUID string.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>string</code> - GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>Array.&lt;number&gt;</code> | GUID number array |

<a id="vscp_dot_utility_dot_strToGuid"></a>

#### utility.strToGuid(guid) ⇒ <code>Array.&lt;number&gt;</code>
Converts a GUID string to a GUID number array.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>Array.&lt;number&gt;</code> - GUID number array  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp_dot_utility_dot_getNodeId"></a>

#### utility.getNodeId(guid) ⇒ <code>number</code>
Get node id from a node GUID string.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>number</code> - Node id  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp_dot_mdf"></a>

### vscp.mdf : <code>object</code>
VSCP module description file handling functionality

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.mdf](#vscp_dot_mdf) : <code>object</code>
    * [.Register](#vscp_dot_mdf_dot_Register)
        * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
        * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
        * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
        * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
        * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
        * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
        * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
        * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
        * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
        * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
        * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)
    * [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
        * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
        * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
        * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
        * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
        * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
        * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
        * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
        * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
        * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
        * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
        * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
        * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
        * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
        * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)
    * [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
        * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
        * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
        * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
        * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)
    * [.timeout](#vscp_dot_mdf_dot_timeout) : <code>number</code>
    * [.load(options)](#vscp_dot_mdf_dot_load)
    * [.loadLocal(options)](#vscp_dot_mdf_dot_loadLocal)
    * [.readAbstractValue(options)](#vscp_dot_mdf_dot_readAbstractValue)
    * [.writeAbstractValue(options)](#vscp_dot_mdf_dot_writeAbstractValue)
    * [.writeAbstractBits(options)](#vscp_dot_mdf_dot_writeAbstractBits)
    * [.getRegisters(options)](#vscp_dot_mdf_dot_getRegisters) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
    * [.getAbstractions(options)](#vscp_dot_mdf_dot_getAbstractions) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)

<a id="vscp_dot_mdf_dot_Register"></a>

#### mdf.Register
**Kind**: static class of [<code>mdf</code>](#vscp_dot_mdf)  

* [.Register](#vscp_dot_mdf_dot_Register)
    * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
    * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
    * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
    * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
    * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
    * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
    * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
    * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
    * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
    * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
    * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)

<a id="new_vscp_dot_mdf_dot_Register_new"></a>

##### new vscp.mdf.Register()
MDF register with all parameters.

<a id="vscp_dot_mdf_dot_Register_and_name"></a>

##### register.name : <code>string</code>
Register name

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_description"></a>

##### register.description : <code>string</code>
Register description

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_readAccess"></a>

##### register.readAccess : <code>boolean</code>
Read access to the register allowed or not

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_writeAccess"></a>

##### register.writeAccess : <code>boolean</code>
Write access to the register allowed or not

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_page"></a>

##### register.page : <code>number</code>
Page where the register is located

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_offset"></a>

##### register.offset : <code>number</code>
Offset where the register is located on the page

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_value"></a>

##### register.value : <code>number</code>
Register value

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_dirty"></a>

##### register.dirty : <code>number</code>
Marks the register value dirty, which means the user changed it.It can be used to detect which registers have to be written to the node.

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_userData"></a>

##### register.userData : <code>object</code>
User specific data

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_setValue"></a>

##### register.setValue(value)
This function set a register value and marks it dirty.

**Kind**: instance method of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | New value |

<a id="vscp_dot_mdf_dot_Abstraction"></a>

#### mdf.Abstraction
**Kind**: static class of [<code>mdf</code>](#vscp_dot_mdf)  

* [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
    * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
    * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
    * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
    * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
    * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
    * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
    * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
    * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
    * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
    * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
    * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
    * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
    * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
    * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)

<a id="new_vscp_dot_mdf_dot_Abstraction_new"></a>

##### new vscp.mdf.Abstraction()
MDF abstraction with all parameters.

<a id="vscp_dot_mdf_dot_Abstraction_and_name"></a>

##### abstraction.name : <code>string</code>
Abstraction name

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_description"></a>

##### abstraction.description : <code>string</code>
Abstraction description

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_readAccess"></a>

##### abstraction.readAccess : <code>boolean</code>
Read access to the abstraction allowed or not

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_writeAccess"></a>

##### abstraction.writeAccess : <code>boolean</code>
Write access to the abstraction allowed or not

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_id"></a>

##### abstraction.id : <code>string</code>
Abstraction id

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_page"></a>

##### abstraction.page : <code>number</code>
Page where the abstraction is located

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_offset"></a>

##### abstraction.offset : <code>number</code>
Offset where the abstraction is located

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_value"></a>

##### abstraction.value : <code>number</code>
Abstraction value

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_type"></a>

##### abstraction.type : <code>string</code>
Abstraction type

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_defValue"></a>

##### abstraction.defValue : <code>number</code>
Abstraction default value

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_dirty"></a>

##### abstraction.dirty : <code>number</code>
Marks the abstraction value dirty, which means the user changed it.It can be used to detect which abstractions have to be written to the node.

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_userData"></a>

##### abstraction.userData : <code>object</code>
User specific data

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_setValue"></a>

##### abstraction.setValue(value)
This function set a abstraction value and marks it dirty.

**Kind**: instance method of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | New value |

<a id="vscp_dot_mdf_dot_constants"></a>

#### mdf.constants : <code>object</code>
MDF specific constants

**Kind**: static namespace of [<code>mdf</code>](#vscp_dot_mdf)  

* [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
    * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
    * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
    * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
    * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)

<a id="vscp_dot_mdf_dot_constants_dot_TYPE_SIZES"></a>

##### constants.TYPE_SIZES : <code>enum</code>
MDF type sizes in bytes

**Kind**: static enum of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| string | <code>number</code> | <code>0</code> | 
| bitfield | <code>number</code> | <code>1</code> | 
| bool | <code>number</code> | <code>1</code> | 
| int8_t | <code>number</code> | <code>1</code> | 
| uint8_t | <code>number</code> | <code>1</code> | 
| int16_t | <code>number</code> | <code>2</code> | 
| uint16_t | <code>number</code> | <code>2</code> | 
| int32_t | <code>number</code> | <code>4</code> | 
| uint32_t | <code>number</code> | <code>4</code> | 
| int64_t | <code>number</code> | <code>8</code> | 
| uint64_t | <code>number</code> | <code>8</code> | 
| float | <code>number</code> | <code>4</code> | 
| double | <code>number</code> | <code>8</code> | 
| date | <code>number</code> | <code>4</code> | 
| time | <code>number</code> | <code>4</code> | 
| guid | <code>number</code> | <code>16</code> | 
| char | <code>number</code> | <code>1</code> | 
| byte | <code>number</code> | <code>1</code> | 
| short | <code>number</code> | <code>2</code> | 
| integer | <code>number</code> | <code>2</code> | 
| long | <code>number</code> | <code>4</code> | 

<a id="vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL"></a>

##### constants.CONVERSION_FROM_DECIMAL
Conversion functions from decimal

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL"></a>

##### constants.CONVERSION_TO_DECIMAL
Conversion functions to decimal

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_constants_dot_RANGE"></a>

##### constants.RANGE
Type ranges

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_timeout"></a>

#### mdf.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>mdf</code>](#vscp_dot_mdf)  
<a id="vscp_dot_mdf_dot_load"></a>

#### mdf.load(options)
Get the MDF as xml document from a URL.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.url | <code>function</code> | URL to MDF file |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_loadLocal"></a>

#### mdf.loadLocal(options)
Get the MDF as xml document from local file system.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.fileRef | <code>function</code> | File reference to MDF file |
| options.onSuccess | <code>function</code> | If the xml file is successful loaded, this function will be called. |
| [options.onError] | <code>function</code> | If loading the xml file failed, this function will be called. |

<a id="vscp_dot_mdf_dot_readAbstractValue"></a>

#### mdf.readAbstractValue(options)
Read a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_writeAbstractValue"></a>

#### mdf.writeAbstractValue(options)
Write a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.value | <code>string</code> | Abstract value |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_writeAbstractBits"></a>

#### mdf.writeAbstractBits(options)
Change some bits in a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.pos | <code>number</code> | Bit position |
| options.width | <code>number</code> | Bit width |
| options.value | <code>string</code> | Abstract value |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_getRegisters"></a>

#### mdf.getRegisters(options) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
This function retrieves all register informations from a mdf.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  
**Returns**: [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register) - Array of MDF registers  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | MDF as jquery object |

<a id="vscp_dot_mdf_dot_getAbstractions"></a>

#### mdf.getAbstractions(options) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)
This function retrieves all abstraction informations from a mdf.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  
**Returns**: [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction) - Array of MDF abstractions  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | MDF as jquery object |

<a id="vscp_dot_measurement"></a>

### vscp.measurement : <code>object</code>
VSCP measurement stuff

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.measurement](#vscp_dot_measurement) : <code>object</code>
    * [.Decoder](#vscp_dot_measurement_dot_Decoder)
        * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
        * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
        * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
        * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>
    * [.constants](#vscp_dot_measurement_dot_constants) : <code>object</code>
        * [.units](#vscp_dot_measurement_dot_constants_dot_units) : <code>Array.&lt;string&gt;</code>
    * [.timeout](#vscp_dot_measurement_dot_timeout) : <code>number</code>
    * [.toFixed(value, precision)](#vscp_dot_measurement_dot_toFixed) ⇒ <code>number</code>
    * [.varInteger2Float(data)](#vscp_dot_measurement_dot_varInteger2Float) ⇒ <code>number</code>
    * [.getDataCoding(data)](#vscp_dot_measurement_dot_getDataCoding) ⇒ <code>number</code>
    * [.getUnitFromDataCoding(data)](#vscp_dot_measurement_dot_getUnitFromDataCoding) ⇒ <code>number</code>
    * [.getSensorIndexFromDataCoding(data)](#vscp_dot_measurement_dot_getSensorIndexFromDataCoding) ⇒ <code>number</code>
    * [.decodeClass10(data)](#vscp_dot_measurement_dot_decodeClass10) ⇒ <code>number</code>
    * [.decodeClass60Number(data)](#vscp_dot_measurement_dot_decodeClass60Number) ⇒ <code>number</code>
    * [.decodeClass65Number(data)](#vscp_dot_measurement_dot_decodeClass65Number) ⇒ <code>number</code>
    * [.convertFahrenheitToKelvin(value)](#vscp_dot_measurement_dot_convertFahrenheitToKelvin) ⇒ <code>number</code>
    * [.convertFahrenheitToCelsius(value)](#vscp_dot_measurement_dot_convertFahrenheitToCelsius) ⇒ <code>number</code>
    * [.convertCelsiusToFahrenheit(value)](#vscp_dot_measurement_dot_convertCelsiusToFahrenheit) ⇒ <code>number</code>
    * [.convertKelvinToCelsius(value)](#vscp_dot_measurement_dot_convertKelvinToCelsius) ⇒ <code>number</code>
    * [.convertCelsiusToKelvin(value)](#vscp_dot_measurement_dot_convertCelsiusToKelvin) ⇒ <code>number</code>
    * [.convertKelvinToFahrenheit(value)](#vscp_dot_measurement_dot_convertKelvinToFahrenheit) ⇒ <code>number</code>
    * [.convertMeterToFeet(value)](#vscp_dot_measurement_dot_convertMeterToFeet) ⇒ <code>number</code>
    * [.convertFeetToMeter(value)](#vscp_dot_measurement_dot_convertFeetToMeter) ⇒ <code>number</code>
    * [.convertMeterToInch(value)](#vscp_dot_measurement_dot_convertMeterToInch) ⇒ <code>number</code>
    * [.convertInchToMeter(value)](#vscp_dot_measurement_dot_convertInchToMeter) ⇒ <code>number</code>

<a id="vscp_dot_measurement_dot_Decoder"></a>

#### measurement.Decoder
**Kind**: static class of [<code>measurement</code>](#vscp_dot_measurement)  

* [.Decoder](#vscp_dot_measurement_dot_Decoder)
    * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
    * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
    * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
    * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>

<a id="new_vscp_dot_measurement_dot_Decoder_new"></a>

##### new vscp.measurement.Decoder(options)
Measurement decoder


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.onValue | <code>function</code> | Function which will be called for every received measurement value. |
| options.filter | <code>object</code> | Filter |
| options.filter.vscpGuid | <code>string</code> | Node GUID string |
| options.filter.vscpClass | <code>number</code> | VSCP class |
| options.filter.vscpType | <code>number</code> | VSCP type |
| options.filter.sensorIndex | <code>number</code> | Sensor index |
| options.filter.zone | <code>number</code> | Zone |
| options.filter.subZone | <code>number</code> | Sub-zone |

<a id="vscp_dot_measurement_dot_Decoder_and_client"></a>

##### decoder.client : [<code>Client</code>](#vscp_dot_ws_dot_Client)
VSCP websocket client

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
<a id="vscp_dot_measurement_dot_Decoder_and_onValue"></a>

##### decoder.onValue : <code>function</code>
Callback which will be called for every received value.

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
<a id="vscp_dot_measurement_dot_Decoder_and_filter"></a>

##### decoder.filter : <code>object</code>
Filter

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| vscpGuid | <code>string</code> | Node GUID string |
| vscpClass | <code>number</code> | VSCP class |
| vscpType | <code>number</code> | VSCP type |
| datetime | <code>date</code> | datetime |
| sensorIndex | <code>number</code> | Sensor index |
| zone | <code>number</code> | Zone |
| subZone | <code>number</code> | Sub-zone |

<a id="vscp_dot_measurement_dot_constants"></a>

#### measurement.constants : <code>object</code>
Measurement specific constants

**Kind**: static namespace of [<code>measurement</code>](#vscp_dot_measurement)  
<a id="vscp_dot_measurement_dot_constants_dot_units"></a>

##### constants.units : <code>Array.&lt;string&gt;</code>
VSCP units

**Kind**: static property of [<code>constants</code>](#vscp_dot_measurement_dot_constants)  
<a id="vscp_dot_measurement_dot_timeout"></a>

#### measurement.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>measurement</code>](#vscp_dot_measurement)  
<a id="vscp_dot_measurement_dot_toFixed"></a>

#### measurement.toFixed(value, precision) ⇒ <code>number</code>
Round value to a fixed precision.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Rounded value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | Value |
| precision | <code>number</code> | Precision |

<a id="vscp_dot_measurement_dot_varInteger2Float"></a>

#### measurement.varInteger2Float(data) ⇒ <code>number</code>
Convert a integer value to float

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Float value  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>Array.&lt;number&gt;</code> | Byte array |

<a id="vscp_dot_measurement_dot_getDataCoding"></a>

#### measurement.getDataCoding(data) ⇒ <code>number</code>
Get data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Coding  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_getUnitFromDataCoding"></a>

#### measurement.getUnitFromDataCoding(data) ⇒ <code>number</code>
Get unit from data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Unit  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data coding |

<a id="vscp_dot_measurement_dot_getSensorIndexFromDataCoding"></a>

#### measurement.getSensorIndexFromDataCoding(data) ⇒ <code>number</code>
Get sensor index from data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Sensor index  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data coding |

<a id="vscp_dot_measurement_dot_decodeClass10"></a>

#### measurement.decodeClass10(data) ⇒ <code>number</code>
Decode a class 10 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>Array.&lt;number&gt;</code> | Data (event data array where first data byte is the data coding) |

<a id="vscp_dot_measurement_dot_decodeClass60Number"></a>

#### measurement.decodeClass60Number(data) ⇒ <code>number</code>
Decode a class 60 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_decodeClass65Number"></a>

#### measurement.decodeClass65Number(data) ⇒ <code>number</code>
Decode a class 65 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_convertFahrenheitToKelvin"></a>

#### measurement.convertFahrenheitToKelvin(value) ⇒ <code>number</code>
Convert from unit fahrenheit to unit kelvin.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertFahrenheitToCelsius"></a>

#### measurement.convertFahrenheitToCelsius(value) ⇒ <code>number</code>
Convert from unit fahrenheit to unit celsius.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertCelsiusToFahrenheit"></a>

#### measurement.convertCelsiusToFahrenheit(value) ⇒ <code>number</code>
Convert from unit celsius to unit fahrenheit.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertKelvinToCelsius"></a>

#### measurement.convertKelvinToCelsius(value) ⇒ <code>number</code>
Convert from unit kelvin to unit celsius.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertCelsiusToKelvin"></a>

#### measurement.convertCelsiusToKelvin(value) ⇒ <code>number</code>
Convert from unit celsius to unit kelvin.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertKelvinToFahrenheit"></a>

#### measurement.convertKelvinToFahrenheit(value) ⇒ <code>number</code>
Convert from unit kelvin to unit fahrenheit.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertMeterToFeet"></a>

#### measurement.convertMeterToFeet(value) ⇒ <code>number</code>
Convert from unit meter to unit feet.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertFeetToMeter"></a>

#### measurement.convertFeetToMeter(value) ⇒ <code>number</code>
Convert from unit feet to unit meter.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertMeterToInch"></a>

#### measurement.convertMeterToInch(value) ⇒ <code>number</code>
Convert from unit meter to unit inch.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertInchToMeter"></a>

#### measurement.convertInchToMeter(value) ⇒ <code>number</code>
Convert from unit inch to unit meter.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_register"></a>

### vscp.register : <code>object</code>
VSCP register access functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.register](#vscp_dot_register) : <code>object</code>
    * [.constants](#vscp_dot_register_dot_constants) : <code>enum</code>
    * [.timeout](#vscp_dot_register_dot_timeout) : <code>number</code>
    * [.read(options)](#vscp_dot_register_dot_read)
    * [.write(options)](#vscp_dot_register_dot_write)
    * [.writeBits(options)](#vscp_dot_register_dot_writeBits)
    * [.readAlarmStatus(options)](#vscp_dot_register_dot_readAlarmStatus)
    * [.readVscpVersion(options)](#vscp_dot_register_dot_readVscpVersion)
    * [.readNodeControlFlags(options)](#vscp_dot_register_dot_readNodeControlFlags)
    * [.readUserId(options)](#vscp_dot_register_dot_readUserId)
    * [.readManufacturerDevId(options)](#vscp_dot_register_dot_readManufacturerDevId)
    * [.readManufacturerSubDevId(options)](#vscp_dot_register_dot_readManufacturerSubDevId)
    * [.readNicknameId(options)](#vscp_dot_register_dot_readNicknameId)
    * [.readSelectedPage(options)](#vscp_dot_register_dot_readSelectedPage)
    * [.readFirmwareVersion(options)](#vscp_dot_register_dot_readFirmwareVersion)
    * [.readBootloaderAlgorithm(options)](#vscp_dot_register_dot_readBootloaderAlgorithm)
    * [.readUsedPages(options)](#vscp_dot_register_dot_readUsedPages)
    * [.readStdDevFamCode(options)](#vscp_dot_register_dot_readStdDevFamCode)
    * [.readStdDevType(options)](#vscp_dot_register_dot_readStdDevType)
    * [.readGUID(options)](#vscp_dot_register_dot_readGUID)
    * [.readMdfUrl(options)](#vscp_dot_register_dot_readMdfUrl)

<a id="vscp_dot_register_dot_constants"></a>

#### register.constants : <code>enum</code>
VSCP registers

**Kind**: static enum of [<code>register</code>](#vscp_dot_register)  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| ALARM_STATUS | <code>number</code> | <code>128</code> | 
| VSCP_VERSION_MAJOR | <code>number</code> | <code>129</code> | 
| VSCP_VERSION_MINOR | <code>number</code> | <code>130</code> | 
| NODE_CONTROL_FLAGS | <code>number</code> | <code>131</code> | 
| USER_ID_0 | <code>number</code> | <code>132</code> | 
| USER_ID_1 | <code>number</code> | <code>133</code> | 
| USER_ID_2 | <code>number</code> | <code>134</code> | 
| USER_ID_3 | <code>number</code> | <code>135</code> | 
| USER_ID_4 | <code>number</code> | <code>136</code> | 
| MANUFACTURER_DEV_ID_0 | <code>number</code> | <code>137</code> | 
| MANUFACTURER_DEV_ID_1 | <code>number</code> | <code>138</code> | 
| MANUFACTURER_DEV_ID_2 | <code>number</code> | <code>139</code> | 
| MANUFACTURER_DEV_ID_3 | <code>number</code> | <code>140</code> | 
| MANUFACTURER_SUB_DEV_ID_0 | <code>number</code> | <code>141</code> | 
| MANUFACTURER_SUB_DEV_ID_1 | <code>number</code> | <code>142</code> | 
| MANUFACTURER_SUB_DEV_ID_2 | <code>number</code> | <code>143</code> | 
| MANUFACTURER_SUB_DEV_ID_3 | <code>number</code> | <code>144</code> | 
| NICKNAME_ID | <code>number</code> | <code>145</code> | 
| PAGE_SELECT_MSB | <code>number</code> | <code>146</code> | 
| PAGE_SELECT_LSB | <code>number</code> | <code>147</code> | 
| FIRMWARE_VERSION_MAJOR | <code>number</code> | <code>148</code> | 
| FIRMWARE_VERSION_MINOR | <code>number</code> | <code>149</code> | 
| FIRMWARE_VERSION_SUB_MINOR | <code>number</code> | <code>150</code> | 
| BOOT_LOADER_ALGORITHM | <code>number</code> | <code>151</code> | 
| BUFFER_SIZE | <code>number</code> | <code>152</code> | 
| PAGES_USED | <code>number</code> | <code>153</code> | 
| STD_DEV_FAMILY_CODE_3 | <code>number</code> | <code>154</code> | 
| STD_DEV_FAMILY_CODE_2 | <code>number</code> | <code>155</code> | 
| STD_DEV_FAMILY_CODE_1 | <code>number</code> | <code>156</code> | 
| STD_DEV_FAMILY_CODE_0 | <code>number</code> | <code>157</code> | 
| STD_DEV_TYPE_3 | <code>number</code> | <code>158</code> | 
| STD_DEV_TYPE_2 | <code>number</code> | <code>159</code> | 
| STD_DEV_TYPE_1 | <code>number</code> | <code>160</code> | 
| STD_DEV_TYPE_0 | <code>number</code> | <code>161</code> | 
| RESTORE_STD_CFG | <code>number</code> | <code>162</code> | 
| GUID | <code>number</code> | <code>208</code> | 
| MDF_URL | <code>number</code> | <code>224</code> | 

<a id="vscp_dot_register_dot_timeout"></a>

#### register.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>register</code>](#vscp_dot_register)  
<a id="vscp_dot_register_dot_read"></a>

#### register.read(options)
Read one or more register values.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| [options.page] | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.count | <code>number</code> | Number of registers to read |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_write"></a>

#### register.write(options)
Write one or more register values.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.page | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.data | <code>Array.&lt;number&gt;</code> | Data array |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_writeBits"></a>

#### register.writeBits(options)
Change some bits of a register.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP connection |
| options.nodeId | <code>number</code> | Node id |
| options.page | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.pos | <code>number</code> | Bit position |
| options.width | <code>number</code> | Bit width |
| options.data | <code>Array.&lt;number&gt;</code> | Data array |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readAlarmStatus"></a>

#### register.readAlarmStatus(options)
Read the alarm status from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readVscpVersion"></a>

#### register.readVscpVersion(options)
Read the supported VSCP version from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readNodeControlFlags"></a>

#### register.readNodeControlFlags(options)
Read the node control flags from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readUserId"></a>

#### register.readUserId(options)
Read the user id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readManufacturerDevId"></a>

#### register.readManufacturerDevId(options)
Read the manufacturer device id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readManufacturerSubDevId"></a>

#### register.readManufacturerSubDevId(options)
Read the manufacturer sub device id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readNicknameId"></a>

#### register.readNicknameId(options)
Read the nickname id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readSelectedPage"></a>

#### register.readSelectedPage(options)
Read the current selected page from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readFirmwareVersion"></a>

#### register.readFirmwareVersion(options)
Read the firmware version from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readBootloaderAlgorithm"></a>

#### register.readBootloaderAlgorithm(options)
Read the bootloader algorithm from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readUsedPages"></a>

#### register.readUsedPages(options)
Read the number of used pages from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readStdDevFamCode"></a>

#### register.readStdDevFamCode(options)
Read the standard device family code from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readStdDevType"></a>

#### register.readStdDevType(options)
Read the standard device type from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readGUID"></a>

#### register.readGUID(options)
Read the GUID from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readMdfUrl"></a>

#### register.readMdfUrl(options)
Read the MDF URL from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_rest"></a>

### vscp.rest : <code>object</code>
VSCP REST api functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.rest](#vscp_dot_rest) : <code>object</code>
    * [.Client](#vscp_dot_rest_dot_Client)
        * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
        * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
        * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
        * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
        * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
        * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
        * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
        * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
        * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
        * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
        * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
        * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
        * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
        * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
        * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
        * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
        * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>

<a id="vscp_dot_rest_dot_Client"></a>

#### rest.Client
**Kind**: static class of [<code>rest</code>](#vscp_dot_rest)  

* [.Client](#vscp_dot_rest_dot_Client)
    * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
    * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
    * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
    * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
    * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
    * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
    * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
    * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
    * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
    * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
    * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>

<a id="new_vscp_dot_rest_dot_Client_new"></a>

##### new vscp.rest.Client(config)
The VSCP client class handles the basic REST api of the VSCP daemon.The function interface uses jquery ajax call in the background and willreturn a Promise.


| Param | Type | Description |
| --- | --- | --- |
| config | <code>string</code> | Configuration |
| [config.baseUrl] | <code>string</code> | VSCP daemon URL (protocol + hostname + port) |
| [options.pathPrefix] | <code>string</code> | Path prefix (default: '/vscp'), which comes right after the base url. |
| [options.apiVersion] | <code>string</code> | API version (for future use) |

<a id="vscp_dot_rest_dot_Client_and_baseUrl"></a>

##### client.baseUrl : <code>string</code>
Base URL

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_pathPrefix"></a>

##### client.pathPrefix : <code>string</code>
Path prefix

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_apiVersion"></a>

##### client.apiVersion : <code>string</code>
REST API version (future use)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_sessionKey"></a>

##### client.sessionKey : <code>string</code>
Session key

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_openSession"></a>

##### client.openSession(options) ⇒ <code>object</code>
Open a session.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.user | <code>string</code> | User name |
| options.password | <code>string</code> | Password |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_closeSession"></a>

##### client.closeSession([options]) ⇒ <code>object</code>
Close a session.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_getStatus"></a>

##### client.getStatus([options]) ⇒ <code>object</code>
Get status and how many events are in the queue.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_sendEvent"></a>

##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>object</code> | VSCP event |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_readEvent"></a>

##### client.readEvent([options]) ⇒ <code>object</code>
Read one or more VSCP events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.count] | <code>object</code> | Number of events to read |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_setFilter"></a>

##### client.setFilter(options) ⇒ <code>object</code>
Set filter.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_clearQueue"></a>

##### client.clearQueue([options]) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_createVar"></a>

##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_rest_dot_Client_and_readVar"></a>

##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_writeVar"></a>

##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_removeVar"></a>

##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_listVar"></a>

##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.listLong | <code>boolean</code> | When false the variable list dos not include value and note. If set to true value and note is included. |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_service"></a>

### vscp.service : <code>object</code>
VSCP service supporting functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.service](#vscp_dot_service) : <code>object</code>
    * [.Container](#vscp_dot_service_dot_Container)
        * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
        * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
        * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
        * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
        * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
        * [.create(options)](#vscp_dot_service_dot_Container_and_create)
        * [.write(options)](#vscp_dot_service_dot_Container_and_write)
        * [.read(options)](#vscp_dot_service_dot_Container_and_read)
    * [.timeout](#vscp_dot_service_dot_timeout) : <code>number</code>
    * [.whoIsThere(options)](#vscp_dot_service_dot_whoIsThere)
    * [.scan(options)](#vscp_dot_service_dot_scan)

<a id="vscp_dot_service_dot_Container"></a>

#### service.Container
**Kind**: static class of [<code>service</code>](#vscp_dot_service)  

* [.Container](#vscp_dot_service_dot_Container)
    * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
    * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
    * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
    * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
    * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
    * [.create(options)](#vscp_dot_service_dot_Container_and_create)
    * [.write(options)](#vscp_dot_service_dot_Container_and_write)
    * [.read(options)](#vscp_dot_service_dot_Container_and_read)

<a id="new_vscp_dot_service_dot_Container_new"></a>

##### new vscp.service.Container(options)
The container is used to store javascript objects in a daemon variable as string.It supports one or more objects in a single variable!


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.name | <code>string</code> | Container name |

<a id="vscp_dot_service_dot_Container_and_client"></a>

##### container.client : [<code>Client</code>](#vscp_dot_ws_dot_Client)
VSCP websocket client

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_name"></a>

##### container.name : <code>string</code>
Complete container name (prefix + user defined name)

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_data"></a>

##### container.data : <code>Array.&lt;object&gt;</code>
Data container itself

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_separator"></a>

##### container.separator : <code>Array.&lt;object&gt;</code>
Data element separator

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_create"></a>

##### container.create(options)
Create a container at the daemon.

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_Container_and_write"></a>

##### container.write(options)
Write the container to a daemon variable.The container must exist at the daemon!

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_Container_and_read"></a>

##### container.read(options)
Read the container from the daemon variable.

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_timeout"></a>

#### service.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>service</code>](#vscp_dot_service)  
<a id="vscp_dot_service_dot_whoIsThere"></a>

#### service.whoIsThere(options)
Request a response from all nodes on the communication bus and returnstheir GUID and MDF URL.

**Kind**: static method of [<code>service</code>](#vscp_dot_service)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_scan"></a>

#### service.scan(options)
Scan for nodes.

**Kind**: static method of [<code>service</code>](#vscp_dot_service)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.begin | <code>number</code> | Node id where to start scanning |
| options.end | <code>number</code> | Node id where to stop scanning |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_widget"></a>

### vscp.widget : <code>object</code>
VSCP widgets

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.widget](#vscp_dot_widget) : <code>object</code>
    * [.Button](#vscp_dot_widget_dot_Button)
        * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
        * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
        * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)
    * [.Thermometer](#vscp_dot_widget_dot_Thermometer)
        * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
        * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
        * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)
    * [.generateUUID()](#vscp_dot_widget_dot_generateUUID) ⇒ <code>string</code>
    * [.Image(options)](#vscp_dot_widget_dot_Image)

<a id="vscp_dot_widget_dot_Button"></a>

#### widget.Button
**Kind**: static class of [<code>widget</code>](#vscp_dot_widget)  

* [.Button](#vscp_dot_widget_dot_Button)
    * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
    * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
    * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)

<a id="new_vscp_dot_widget_dot_Button_new"></a>

##### new vscp.widget.Button(options)
A button widget.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.offImageUrl | <code>number</code> | URL to button which is in off state |
| options.onImageUrl | <code>number</code> | URL to button which is in on state |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |
| [options.scale] | <code>number</code> | Scale factor applied to the button image (default: 1.0) |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client, used for event communication |
| [options.bindToRemoteState] | <code>boolean</code> | Bind the button state to the remote state or not (default: false) |
| [options.receiveZone] | <code>number</code> | Zone where state events will come from (default: 255) |
| [options.receiveSubZone] | <code>number</code> | Sub-zone where state events will come from (default: 255) |
| [options.transmitZone] | <code>number</code> | Zone where button event will be sent to (default: 255) |
| [options.transmitSubZone] | <code>number</code> | Sub-zone where button event will be sent to (default: 255) |
| [options.index] | <code>number</code> | Button index (instance number)  (default: 0) |
| [options.enable] | <code>boolean</code> | Enable or disable button  (default: false) |

<a id="vscp_dot_widget_dot_Button_and_draw"></a>

##### button.draw()
Draw the button depended on its current state.

**Kind**: instance method of [<code>Button</code>](#vscp_dot_widget_dot_Button)  
<a id="vscp_dot_widget_dot_Button_and_setEnabled"></a>

##### button.setEnabled(value)
Enable or disable the button.

**Kind**: instance method of [<code>Button</code>](#vscp_dot_widget_dot_Button)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>boolean</code> | Enable (true) or disable (false) it |

<a id="vscp_dot_widget_dot_Thermometer"></a>

#### widget.Thermometer
**Kind**: static class of [<code>widget</code>](#vscp_dot_widget)  

* [.Thermometer](#vscp_dot_widget_dot_Thermometer)
    * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
    * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
    * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)

<a id="new_vscp_dot_widget_dot_Thermometer_new"></a>

##### new vscp.widget.Thermometer(options)
A thermometer widget.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.imageUrl | <code>number</code> | URL to thermometer image |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |
| options.data | <code>object</code> | Thermometer data |
| options.data.maxT | <code>number</code> | Max. temperature in degree celsius |
| options.data.minT | <code>number</code> | Min. temperature in degree celsius |
| options.data.x | <code>number</code> | x position of the lower left begin of the thermometer column in image |
| options.data.y | <code>number</code> | y position of the lower left begin of the thermometer column in image |
| options.data.height | <code>number</code> | Thermometer column height (only between numbers) |
| options.data.width | <code>number</code> | Thermometer column width |
| options.data.yOffset | <code>number</code> | Thermometer column height offset from the begin to the first number |
| options.data.color | <code>string</code> | HTML color, e.g. '#8A0000' |
| [options.scale] | <code>number</code> | Scale factor applied to the thermometer image (default: 1.0) |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client, used for event communication |
| [options.receiveZone] | <code>number</code> | Zone where state events will come from (default: 255) |
| [options.receiveSubZone] | <code>number</code> | Sub-zone where state events will come from (default: 255) |
| [options.sensorIndex] | <code>number</code> | Sensor index (default: 0) |
| [options.vscpClass] | <code>number</code> | VSCP measurement class (default: CLASS1.MEASUREMENT) |
| [options.vscpType] | <code>number</code> | VSCP measurement type (default: CLASS1.MEASUREMENT.TERMPERATURE) |
| [options.enable] | <code>boolean</code> | Enable or disable thermometer (default: true) |

<a id="vscp_dot_widget_dot_Thermometer_and_draw"></a>

##### thermometer.draw()
Draw the thermometer depended on its current state.

**Kind**: instance method of [<code>Thermometer</code>](#vscp_dot_widget_dot_Thermometer)  
<a id="vscp_dot_widget_dot_Thermometer_and_setEnabled"></a>

##### thermometer.setEnabled(value)
Enable or disable the thermometer.

**Kind**: instance method of [<code>Thermometer</code>](#vscp_dot_widget_dot_Thermometer)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>boolean</code> | Enable (true) or disable (false) it |

<a id="vscp_dot_widget_dot_generateUUID"></a>

#### widget.generateUUID() ⇒ <code>string</code>
Generate a UUID.

**Kind**: static method of [<code>widget</code>](#vscp_dot_widget)  
**Returns**: <code>string</code> - UUID  
<a id="vscp_dot_widget_dot_Image"></a>

#### widget.Image(options)
Add a image to the canvas.

**Kind**: static method of [<code>widget</code>](#vscp_dot_widget)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.url | <code>string</code> | Path to the image |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |

<a id="vscp_dot_wizard"></a>

### vscp.wizard : <code>object</code>
VSCP wizard functionality based on a MDF

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.wizard](#vscp_dot_wizard) : <code>object</code>
    * [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
        * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
        * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
        * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
        * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
        * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
        * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
        * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
        * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)
    * [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
        * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
        * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
        * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
        * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
        * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
        * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)
    * [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
        * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
        * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
        * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
        * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
        * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)
    * [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
        * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
        * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
        * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
        * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)
    * [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
        * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
        * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
        * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
        * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)
    * [.Recipe](#vscp_dot_wizard_dot_Recipe)
        * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
        * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
        * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
        * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
        * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
        * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
        * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
        * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
        * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
        * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
        * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)
    * [.getRecipes(options)](#vscp_dot_wizard_dot_getRecipes) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)

<a id="vscp_dot_wizard_dot_MessageBox"></a>

#### wizard.MessageBox
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
    * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
    * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
    * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
    * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
    * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
    * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
    * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
    * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)

<a id="new_vscp_dot_wizard_dot_MessageBox_new"></a>

##### new vscp.wizard.MessageBox(options)
A message box.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.messageBox | <code>object</code> | Messagebox as jquery xml object |

<a id="vscp_dot_wizard_dot_MessageBox_and_func"></a>

##### messageBox.func : <code>string</code>
Function input or output

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_head"></a>

##### messageBox.head : <code>string</code>
Head

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_description"></a>

##### messageBox.description : <code>string</code>
Description

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableType"></a>

##### messageBox.variableType : <code>string</code>
Variable type

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableName"></a>

##### messageBox.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableValue"></a>

##### messageBox.variableValue : <code>string</code>
Variable value

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_parse"></a>

##### messageBox.parse($messageBox)
Parse a messagebox object.

**Kind**: instance method of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  

| Param | Type | Description |
| --- | --- | --- |
| $messageBox | <code>object</code> | Messagebox as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInReg"></a>

#### wizard.WriteBitInReg
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
    * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
    * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
    * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
    * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
    * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
    * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteBitInReg_new"></a>

##### new vscp.wizard.WriteBitInReg(options)
Bit in register access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeBitInReg | <code>object</code> | write-bit-in-reg as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInReg_and_pos"></a>

##### writeBitInReg.pos : <code>number</code>
Bit position

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_page"></a>

##### writeBitInReg.page : <code>number</code>
Register page

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_offset"></a>

##### writeBitInReg.offset : <code>number</code>
Register offset

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_width"></a>

##### writeBitInReg.width : <code>number</code>
Bit width

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_value"></a>

##### writeBitInReg.value : <code>number</code>
Value of bit width

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_variableName"></a>

##### writeBitInReg.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_parse"></a>

##### writeBitInReg.parse(writeBitInReg)
Parse a bit in register access method object.

**Kind**: instance method of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  

| Param | Type | Description |
| --- | --- | --- |
| writeBitInReg | <code>object</code> | write-bit-in-reg as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInAbstraction"></a>

#### wizard.WriteBitInAbstraction
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
    * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
    * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
    * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
    * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
    * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteBitInAbstraction_new"></a>

##### new vscp.wizard.WriteBitInAbstraction(options)
Bit in abstraction access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeBitInAbstraction | <code>object</code> | write-bit-in-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_id"></a>

##### writeBitInAbstraction.id : <code>string</code>
Abstract value id

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos"></a>

##### writeBitInAbstraction.pos : <code>number</code>
Bit position

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_width"></a>

##### writeBitInAbstraction.width : <code>number</code>
Bit width

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_value"></a>

##### writeBitInAbstraction.value : <code>number</code>
Value of bit width

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName"></a>

##### writeBitInAbstraction.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse"></a>

##### writeBitInAbstraction.parse($writeBitInAbstraction)
Parse a bit in abstraction access method object.

**Kind**: instance method of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  

| Param | Type | Description |
| --- | --- | --- |
| $writeBitInAbstraction | <code>object</code> | write-bit-in-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteRegister"></a>

#### wizard.WriteRegister
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
    * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
    * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
    * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
    * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteRegister_new"></a>

##### new vscp.wizard.WriteRegister(options)
Register access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeRegister | <code>object</code> | write-register as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteRegister_and_page"></a>

##### writeRegister.page : <code>number</code>
Register page

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_offset"></a>

##### writeRegister.offset : <code>number</code>
Register offset

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_value"></a>

##### writeRegister.value : <code>number</code>
Register value

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_variableName"></a>

##### writeRegister.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_parse"></a>

##### writeRegister.parse($writeRegister)
Parse a register access method object.

**Kind**: instance method of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  

| Param | Type | Description |
| --- | --- | --- |
| $writeRegister | <code>object</code> | write-register as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteAbstraction"></a>

#### wizard.WriteAbstraction
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
    * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
    * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
    * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
    * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteAbstraction_new"></a>

##### new vscp.wizard.WriteAbstraction(options)
Abstraction access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeAbstraction | <code>object</code> | write-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteAbstraction_and_id"></a>

##### writeAbstraction.id : <code>string</code>
Abstract value id

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_value"></a>

##### writeAbstraction.value : <code>number</code>
Abstract value

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_variableName"></a>

##### writeAbstraction.variableName : <code>number</code>
Variable name

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_parse"></a>

##### writeAbstraction.parse($writeAbstraction)
Parse a abstraction access method object.

**Kind**: instance method of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  

| Param | Type | Description |
| --- | --- | --- |
| $writeAbstraction | <code>object</code> | write-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe"></a>

#### wizard.Recipe
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.Recipe](#vscp_dot_wizard_dot_Recipe)
    * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
    * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
    * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
    * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
    * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
    * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
    * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
    * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
    * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
    * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
    * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)

<a id="new_vscp_dot_wizard_dot_Recipe_new"></a>

##### new vscp.wizard.Recipe(options)
A recipe.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.recipe | <code>object</code> | Recipe as jquery xml object |
| options.mdf | <code>object</code> | MDF as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe_and_name"></a>

##### recipe.name : <code>string</code>
Recipe name

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_description"></a>

##### recipe.description : <code>string</code>
Recipe description

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeBitInRegs"></a>

##### recipe.writeBitInRegs : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
Bit access methods in registers

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions"></a>

##### recipe.writeBitInAbstractions : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
Bit access methods in abstract value

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeRegisters"></a>

##### recipe.writeRegisters : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
Register access methods

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeAbstractions"></a>

##### recipe.writeAbstractions : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
Abstract access methods

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_messageBoxes"></a>

##### recipe.messageBoxes : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
Messageboxes

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_mdf"></a>

##### recipe.mdf : <code>object</code>
MDF

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_parse"></a>

##### recipe.parse($recipe)
Parse a recipe object.

**Kind**: instance method of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  

| Param | Type | Description |
| --- | --- | --- |
| $recipe | <code>object</code> | Recipe as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe_and_write"></a>

##### recipe.write(options)
Write a recipe.

**Kind**: instance method of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |

<a id="vscp_dot_wizard_dot_getRecipes"></a>

#### wizard.getRecipes(options) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)
Get recipes from a MDF in JSON format.

**Kind**: static method of [<code>wizard</code>](#vscp_dot_wizard)  
**Returns**: [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe) - Recipe array  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | The mdf as jquery xml object |

<a id="vscp_dot_ws"></a>

### vscp.ws : <code>object</code>
VSCP websocket api functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.ws](#vscp_dot_ws) : <code>object</code>
    * [.Client](#vscp_dot_ws_dot_Client)
        * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
        * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
        * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
        * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
        * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
        * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
        * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
        * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
        * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
        * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
        * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
        * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
        * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
        * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
        * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
        * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
        * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
        * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
        * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
        * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
        * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
        * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
        * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
        * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
        * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
        * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
        * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
        * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
        * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
        * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
        * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
        * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
        * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
        * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
        * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
        * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
        * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
        * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
        * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
        * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
        * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
        * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
        * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
        * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
        * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>

<a id="vscp_dot_ws_dot_Client"></a>

#### ws.Client
**Kind**: static class of [<code>ws</code>](#vscp_dot_ws)  

* [.Client](#vscp_dot_ws_dot_Client)
    * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
    * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
    * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
    * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
    * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
    * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
    * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
    * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
    * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
    * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
    * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
    * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
    * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
    * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
    * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
    * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
    * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
    * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
    * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
    * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
    * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
    * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
    * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
    * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
    * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
    * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
    * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
    * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
    * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
    * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
    * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
    * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
    * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
    * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
    * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
    * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
    * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
    * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
    * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>

<a id="new_vscp_dot_ws_dot_Client_new"></a>

##### new vscp.ws.Client()
VSCP websocket client, used for connection establishment to a VSCP server.

<a id="vscp_dot_ws_dot_Client_and_socket"></a>

##### client.socket : <code>object</code>
Websocket

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_url"></a>

##### client.url : <code>string</code>
url used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userName"></a>

##### client.userName : <code>string</code>
User name used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userId"></a>

##### client.userId : <code>number</code>
User id from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userFullname"></a>

##### client.userFullname : <code>string</code>
User full name from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userRights"></a>

##### client.userRights : <code>array</code>
User rights from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userRemotes"></a>

##### client.userRemotes : <code>array</code>
User allowed remotes from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userEvents"></a>

##### client.userEvents : <code>array</code>
User allowed events from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userNote"></a>

##### client.userNote : <code>string</code>
User note from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_password"></a>

##### client.password : <code>string</code>
Password used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_vscpkey"></a>

##### client.vscpkey : <code>string</code>
Secret key used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_authdomain"></a>

##### client.authdomain : <code>string</code>
authdomain used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_passwordHash"></a>

##### client.passwordHash : <code>string</code>
Password hash used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onConnError"></a>

##### client.onConnError : <code>function</code>
Callback called on any connection error

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onMessage"></a>

##### client.onMessage : <code>function</code>
Callback called on any received VSCP response message

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onEvent"></a>

##### client.onEvent : <code>Array.&lt;function()&gt;</code>
Callbacks called on any received VSCP event message

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onVariable"></a>

##### client.onVariable : <code>function</code>
Callback called on any received variable (see LSTVAR command)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onTableRow"></a>

##### client.onTableRow : <code>function</code>
Callback called on any received table row (see GT command)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_state"></a>

##### client.state : <code>number</code>
VSCP websocket is not connected right now

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_substate"></a>

##### client.substate : <code>number</code>
VSCP event traffic is closed

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_states"></a>

##### client.states : <code>enum</code>
States of the VSCP websocket

**Kind**: instance enum of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| DISCONNECTED | <code>number</code> | <code>0</code> | Not connected |
| CONNECTED | <code>number</code> | <code>1</code> | Standard websocket connection established |
| AUTHENTICATED | <code>number</code> | <code>2</code> | Authentication with VSCP server successful |

<a id="vscp_dot_ws_dot_Client_and_substates"></a>

##### client.substates : <code>enum</code>
Substates of the VSCP websocket

**Kind**: instance enum of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| CLOSED | <code>number</code> | <code>0</code> | No events sent from server |
| OPEN | <code>number</code> | <code>1</code> | Events sent from server |

<a id="vscp_dot_ws_dot_Client_and_addEventListener"></a>

##### client.addEventListener(eventListener)
Add a event listener.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp_dot_ws_dot_Client_and_removeEventListener"></a>

##### client.removeEventListener(eventListener)
Remove a event listener.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp_dot_ws_dot_Client_and_getAuthHash"></a>

##### client.getAuthHash(userName, password, str_iv) ⇒ <code>string</code>
Calculates the VSCP server websocket authentication hash.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>string</code> - Authentication ("encrypted user:password")  

| Param | Type | Description |
| --- | --- | --- |
| userName | <code>string</code> | User name |
| password | <code>string</code> | Password |
| str_iv | <code>string</code> | 16 random byte iv in hex form |

<a id="vscp_dot_ws_dot_Client_and_onWebSocketOpen"></a>

##### client.onWebSocketOpen()
This function is called by the websocket in case the connection is established.
It will initiate the authentication with the VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onWebSocketClose"></a>

##### client.onWebSocketClose()
This function is called by the websocket in case that the connection is closed.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onWebSocketMessage"></a>

##### client.onWebSocketMessage(msg)
This function is called for any websocket message (VSCP server response message).

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp_dot_ws_dot_Client_and_connect"></a>

##### client.connect(options) ⇒ <code>object</code>
Connect to a VSCP server with the given URL.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_ws_dot_Client_and_disconnect"></a>

##### client.disconnect(options) ⇒ <code>object</code>
Disconnect from a VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful disconnection. |

<a id="vscp_dot_ws_dot_Client_and_start"></a>

##### client.start(options) ⇒ <code>object</code>
Start receiving events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_stop"></a>

##### client.stop(options) ⇒ <code>object</code>
Stop receiving events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_clearQueue"></a>

##### client.clearQueue(options) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_sendEvent"></a>

##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event to the VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | [<code>Event</code>](#vscp_dot_Event) | VSCP event to send |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_setFilter"></a>

##### client.setFilter(options) ⇒ <code>object</code>
Set a filter in the VSCP server for VSCP events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter (default: 0) |
| [options.filterClass] | <code>number</code> | Class filter (default: 0) |
| [options.filterType] | <code>number</code> | Type filter (default: 0) |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID filter (default: 0) |
| [options.maskPriority] | <code>number</code> | Priority mask (default: 0) |
| [options.maskClass] | <code>number</code> | Class mask (default: 0xffff) |
| [options.maskType] | <code>number</code> | Type mask (default: 0xffff) |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID mask (default: 0) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_createVar"></a>

##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_ws_dot_Client_and_readVar"></a>

##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_writeVar"></a>

##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_resetVar"></a>

##### client.resetVar(options) ⇒ <code>object</code>
Reset a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_removeVar"></a>

##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_lengthVar"></a>

##### client.lengthVar(options) ⇒ <code>object</code>
Get a VSCP server variable length.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_lastChangeVar"></a>

##### client.lastChangeVar(options) ⇒ <code>object</code>
Get last change of a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_listVar"></a>

##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| options.onVariable | <code>function</code> | Function which is called per variable |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_readTable"></a>

##### client.readTable(options) ⇒ <code>object</code>
Get data from a table.
If "begin" and "end" are omitted, the whole table is returned.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Table name |
| options.begin | <code>string</code> | Date when to begin ( ISO form YY-MM-DD HH:MM:SS ) |
| options.end | <code>string</code> | Date when to end ( ISO form YY-MM-DD HH:MM:SS ) |
| options.onTableRow | <code>function</code> | Function which is called on every received table row |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_getVarTypeName"></a>

### vscp.getVarTypeName(n) ⇒ <code>string</code>
Get variable type name as string by numerical code.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Variable type name  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Numerical code |

<a id="vscp_dot_getVarTypeNumerical"></a>

### vscp.getVarTypeNumerical(str) ⇒ <code>number</code>
Get numerical code of variable type from string.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>number</code> - Variable type numerical code  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Variable type name |

<a id="vscp_dot_getEditorModeFromType"></a>

### vscp.getEditorModeFromType(n) ⇒ <code>string</code>
Get ace editor formation mode string from numerical variable type code.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Ace editro formation mode string  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Variable type numerical code |

<a id="vscp_dot_b64EncodeUnicode"></a>

### vscp.b64EncodeUnicode(str) ⇒ <code>string</code>
Encode base64 unicode safe.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Base64  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Unicode string |

<a id="vscp_dot_b64DecodeUnicode"></a>

### vscp.b64DecodeUnicode(str) ⇒ <code>string</code>
Decode base64 unicode safe.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Unicode string  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Base64 |

<a id="vscp_dot_isBase64Type"></a>

### vscp.isBase64Type(type) ⇒ <code>bool</code>
Determine whether the given variable type is a type stored base64 encoded or not.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>bool</code> - Stored base64 encoded (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |

<a id="vscp_dot_decodeValueIfBase64"></a>

### vscp.decodeValueIfBase64(type, value) ⇒ <code>string</code>
Decode the value if its base64 encoded.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Decoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |

<a id="vscp_dot_encodeValueIfBase64"></a>

### vscp.encodeValueIfBase64(type, value) ⇒ <code>string</code>
Encode the value if its stored in base64.

**Kind**: static method of [<code>vscp</code>](#vscp)  
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
    * [.Event](#vscp_dot_Event)
        * [new vscp.Event(options)](#new_vscp_dot_Event_new)
        * [.vscpHead](#vscp_dot_Event_and_vscpHead) : <code>number</code>
        * [.vscpClass](#vscp_dot_Event_and_vscpClass) : <code>number</code>
        * [.vscpType](#vscp_dot_Event_and_vscpType) : <code>number</code>
        * [.vscpObId](#vscp_dot_Event_and_vscpObId) : <code>number</code>
        * [.vscpTimeStamp](#vscp_dot_Event_and_vscpTimeStamp) : <code>number</code>
        * [.vscpDateTime](#vscp_dot_Event_and_vscpDateTime) : <code>date</code>
        * [.vscpGuid](#vscp_dot_Event_and_vscpGuid) : <code>string</code>
        * [.vscpData](#vscp_dot_Event_and_vscpData) : <code>Array.&lt;number&gt;</code> \| <code>string</code>
        * [.setIPV6Addr()](#vscp_dot_Event_and_setIPV6Addr)
        * [.isIPV6Addr()](#vscp_dot_Event_and_isIPV6Addr) ⇒ <code>boolean</code>
        * [.setDumbNode()](#vscp_dot_Event_and_setDumbNode)
        * [.isDumbNode()](#vscp_dot_Event_and_isDumbNode) ⇒ <code>boolean</code>
        * [.setPriority(priority)](#vscp_dot_Event_and_setPriority)
        * [.getPriority()](#vscp_dot_Event_and_getPriority) ⇒ <code>number</code>
        * [.setHardCodedAddr()](#vscp_dot_Event_and_setHardCodedAddr)
        * [.isHardCodedAddr()](#vscp_dot_Event_and_isHardCodedAddr) ⇒ <code>boolean</code>
        * [.setDoNotCalcCRC()](#vscp_dot_Event_and_setDoNotCalcCRC)
        * [.isDoNotCalcCRC()](#vscp_dot_Event_and_isDoNotCalcCRC) ⇒ <code>boolean</code>
        * [.getText()](#vscp_dot_Event_and_getText) ⇒ <code>string</code>
    * [.version](#vscp_dot_version)
    * [.constants](#vscp_dot_constants) : <code>object</code>
        * [.classes](#vscp_dot_constants_dot_classes) : <code>enum</code>
        * [.types](#vscp_dot_constants_dot_types) : <code>enum</code>
        * [.priorities](#vscp_dot_constants_dot_priorities) : <code>enum</code>
        * [.varTypes](#vscp_dot_constants_dot_varTypes) : <code>enum</code>
        * [.varTypeNames](#vscp_dot_constants_dot_varTypeNames)
    * [.utility](#vscp_dot_utility) : <code>object</code>
        * [.readValue(input)](#vscp_dot_utility_dot_readValue) ⇒ <code>number</code>
        * [.getTime()](#vscp_dot_utility_dot_getTime) ⇒ <code>string</code>
        * [.guidToStr(guid)](#vscp_dot_utility_dot_guidToStr) ⇒ <code>string</code>
        * [.strToGuid(guid)](#vscp_dot_utility_dot_strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
        * [.getNodeId(guid)](#vscp_dot_utility_dot_getNodeId) ⇒ <code>number</code>
    * [.mdf](#vscp_dot_mdf) : <code>object</code>
        * [.Register](#vscp_dot_mdf_dot_Register)
            * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
            * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
            * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
            * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
            * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
            * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
            * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
            * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
            * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
            * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
            * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)
        * [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
            * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
            * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
            * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
            * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
            * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
            * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
            * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
            * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
            * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
            * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
            * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
            * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
            * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
            * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)
        * [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
            * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
            * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
            * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
            * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)
        * [.timeout](#vscp_dot_mdf_dot_timeout) : <code>number</code>
        * [.load(options)](#vscp_dot_mdf_dot_load)
        * [.loadLocal(options)](#vscp_dot_mdf_dot_loadLocal)
        * [.readAbstractValue(options)](#vscp_dot_mdf_dot_readAbstractValue)
        * [.writeAbstractValue(options)](#vscp_dot_mdf_dot_writeAbstractValue)
        * [.writeAbstractBits(options)](#vscp_dot_mdf_dot_writeAbstractBits)
        * [.getRegisters(options)](#vscp_dot_mdf_dot_getRegisters) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
        * [.getAbstractions(options)](#vscp_dot_mdf_dot_getAbstractions) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)
    * [.measurement](#vscp_dot_measurement) : <code>object</code>
        * [.Decoder](#vscp_dot_measurement_dot_Decoder)
            * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
            * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
            * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
            * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>
        * [.constants](#vscp_dot_measurement_dot_constants) : <code>object</code>
            * [.units](#vscp_dot_measurement_dot_constants_dot_units) : <code>Array.&lt;string&gt;</code>
        * [.timeout](#vscp_dot_measurement_dot_timeout) : <code>number</code>
        * [.toFixed(value, precision)](#vscp_dot_measurement_dot_toFixed) ⇒ <code>number</code>
        * [.varInteger2Float(data)](#vscp_dot_measurement_dot_varInteger2Float) ⇒ <code>number</code>
        * [.getDataCoding(data)](#vscp_dot_measurement_dot_getDataCoding) ⇒ <code>number</code>
        * [.getUnitFromDataCoding(data)](#vscp_dot_measurement_dot_getUnitFromDataCoding) ⇒ <code>number</code>
        * [.getSensorIndexFromDataCoding(data)](#vscp_dot_measurement_dot_getSensorIndexFromDataCoding) ⇒ <code>number</code>
        * [.decodeClass10(data)](#vscp_dot_measurement_dot_decodeClass10) ⇒ <code>number</code>
        * [.decodeClass60Number(data)](#vscp_dot_measurement_dot_decodeClass60Number) ⇒ <code>number</code>
        * [.decodeClass65Number(data)](#vscp_dot_measurement_dot_decodeClass65Number) ⇒ <code>number</code>
        * [.convertFahrenheitToKelvin(value)](#vscp_dot_measurement_dot_convertFahrenheitToKelvin) ⇒ <code>number</code>
        * [.convertFahrenheitToCelsius(value)](#vscp_dot_measurement_dot_convertFahrenheitToCelsius) ⇒ <code>number</code>
        * [.convertCelsiusToFahrenheit(value)](#vscp_dot_measurement_dot_convertCelsiusToFahrenheit) ⇒ <code>number</code>
        * [.convertKelvinToCelsius(value)](#vscp_dot_measurement_dot_convertKelvinToCelsius) ⇒ <code>number</code>
        * [.convertCelsiusToKelvin(value)](#vscp_dot_measurement_dot_convertCelsiusToKelvin) ⇒ <code>number</code>
        * [.convertKelvinToFahrenheit(value)](#vscp_dot_measurement_dot_convertKelvinToFahrenheit) ⇒ <code>number</code>
        * [.convertMeterToFeet(value)](#vscp_dot_measurement_dot_convertMeterToFeet) ⇒ <code>number</code>
        * [.convertFeetToMeter(value)](#vscp_dot_measurement_dot_convertFeetToMeter) ⇒ <code>number</code>
        * [.convertMeterToInch(value)](#vscp_dot_measurement_dot_convertMeterToInch) ⇒ <code>number</code>
        * [.convertInchToMeter(value)](#vscp_dot_measurement_dot_convertInchToMeter) ⇒ <code>number</code>
    * [.register](#vscp_dot_register) : <code>object</code>
        * [.constants](#vscp_dot_register_dot_constants) : <code>enum</code>
        * [.timeout](#vscp_dot_register_dot_timeout) : <code>number</code>
        * [.read(options)](#vscp_dot_register_dot_read)
        * [.write(options)](#vscp_dot_register_dot_write)
        * [.writeBits(options)](#vscp_dot_register_dot_writeBits)
        * [.readAlarmStatus(options)](#vscp_dot_register_dot_readAlarmStatus)
        * [.readVscpVersion(options)](#vscp_dot_register_dot_readVscpVersion)
        * [.readNodeControlFlags(options)](#vscp_dot_register_dot_readNodeControlFlags)
        * [.readUserId(options)](#vscp_dot_register_dot_readUserId)
        * [.readManufacturerDevId(options)](#vscp_dot_register_dot_readManufacturerDevId)
        * [.readManufacturerSubDevId(options)](#vscp_dot_register_dot_readManufacturerSubDevId)
        * [.readNicknameId(options)](#vscp_dot_register_dot_readNicknameId)
        * [.readSelectedPage(options)](#vscp_dot_register_dot_readSelectedPage)
        * [.readFirmwareVersion(options)](#vscp_dot_register_dot_readFirmwareVersion)
        * [.readBootloaderAlgorithm(options)](#vscp_dot_register_dot_readBootloaderAlgorithm)
        * [.readUsedPages(options)](#vscp_dot_register_dot_readUsedPages)
        * [.readStdDevFamCode(options)](#vscp_dot_register_dot_readStdDevFamCode)
        * [.readStdDevType(options)](#vscp_dot_register_dot_readStdDevType)
        * [.readGUID(options)](#vscp_dot_register_dot_readGUID)
        * [.readMdfUrl(options)](#vscp_dot_register_dot_readMdfUrl)
    * [.rest](#vscp_dot_rest) : <code>object</code>
        * [.Client](#vscp_dot_rest_dot_Client)
            * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
            * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
            * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
            * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
            * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
            * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
            * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
            * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
            * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
            * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
            * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
            * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
            * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
            * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
            * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
            * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
            * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>
    * [.service](#vscp_dot_service) : <code>object</code>
        * [.Container](#vscp_dot_service_dot_Container)
            * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
            * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
            * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
            * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
            * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
            * [.create(options)](#vscp_dot_service_dot_Container_and_create)
            * [.write(options)](#vscp_dot_service_dot_Container_and_write)
            * [.read(options)](#vscp_dot_service_dot_Container_and_read)
        * [.timeout](#vscp_dot_service_dot_timeout) : <code>number</code>
        * [.whoIsThere(options)](#vscp_dot_service_dot_whoIsThere)
        * [.scan(options)](#vscp_dot_service_dot_scan)
    * [.widget](#vscp_dot_widget) : <code>object</code>
        * [.Button](#vscp_dot_widget_dot_Button)
            * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
            * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
            * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)
        * [.Thermometer](#vscp_dot_widget_dot_Thermometer)
            * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
            * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
            * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)
        * [.generateUUID()](#vscp_dot_widget_dot_generateUUID) ⇒ <code>string</code>
        * [.Image(options)](#vscp_dot_widget_dot_Image)
    * [.wizard](#vscp_dot_wizard) : <code>object</code>
        * [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
            * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
            * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
            * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
            * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
            * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
            * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
            * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
            * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)
        * [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
            * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
            * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
            * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
            * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
            * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
            * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)
        * [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
            * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
            * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
            * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
            * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
            * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)
        * [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
            * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
            * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
            * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
            * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
            * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)
        * [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
            * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
            * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
            * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
            * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
            * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)
        * [.Recipe](#vscp_dot_wizard_dot_Recipe)
            * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
            * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
            * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
            * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
            * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
            * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
            * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
            * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
            * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
            * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
            * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)
        * [.getRecipes(options)](#vscp_dot_wizard_dot_getRecipes) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)
    * [.ws](#vscp_dot_ws) : <code>object</code>
        * [.Client](#vscp_dot_ws_dot_Client)
            * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
            * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
            * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
            * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
            * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
            * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
            * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
            * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
            * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
            * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
            * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
            * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
            * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
            * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
            * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
            * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
            * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
            * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
            * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
            * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
            * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
            * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
            * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
            * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
            * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
            * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
            * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
            * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
            * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
            * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
            * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
            * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
            * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
            * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
            * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
            * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
            * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
            * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
            * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
            * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
            * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
            * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
            * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
            * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
            * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>
    * [.getVarTypeName(n)](#vscp_dot_getVarTypeName) ⇒ <code>string</code>
    * [.getVarTypeNumerical(str)](#vscp_dot_getVarTypeNumerical) ⇒ <code>number</code>
    * [.getEditorModeFromType(n)](#vscp_dot_getEditorModeFromType) ⇒ <code>string</code>
    * [.b64EncodeUnicode(str)](#vscp_dot_b64EncodeUnicode) ⇒ <code>string</code>
    * [.b64DecodeUnicode(str)](#vscp_dot_b64DecodeUnicode) ⇒ <code>string</code>
    * [.isBase64Type(type)](#vscp_dot_isBase64Type) ⇒ <code>bool</code>
    * [.decodeValueIfBase64(type, value)](#vscp_dot_decodeValueIfBase64) ⇒ <code>string</code>
    * [.encodeValueIfBase64(type, value)](#vscp_dot_encodeValueIfBase64) ⇒ <code>string</code>

<a id="vscp_dot_Event"></a>

### vscp.Event
**Kind**: static class of [<code>vscp</code>](#vscp)  

* [.Event](#vscp_dot_Event)
    * [new vscp.Event(options)](#new_vscp_dot_Event_new)
    * [.vscpHead](#vscp_dot_Event_and_vscpHead) : <code>number</code>
    * [.vscpClass](#vscp_dot_Event_and_vscpClass) : <code>number</code>
    * [.vscpType](#vscp_dot_Event_and_vscpType) : <code>number</code>
    * [.vscpObId](#vscp_dot_Event_and_vscpObId) : <code>number</code>
    * [.vscpTimeStamp](#vscp_dot_Event_and_vscpTimeStamp) : <code>number</code>
    * [.vscpDateTime](#vscp_dot_Event_and_vscpDateTime) : <code>date</code>
    * [.vscpGuid](#vscp_dot_Event_and_vscpGuid) : <code>string</code>
    * [.vscpData](#vscp_dot_Event_and_vscpData) : <code>Array.&lt;number&gt;</code> \| <code>string</code>
    * [.setIPV6Addr()](#vscp_dot_Event_and_setIPV6Addr)
    * [.isIPV6Addr()](#vscp_dot_Event_and_isIPV6Addr) ⇒ <code>boolean</code>
    * [.setDumbNode()](#vscp_dot_Event_and_setDumbNode)
    * [.isDumbNode()](#vscp_dot_Event_and_isDumbNode) ⇒ <code>boolean</code>
    * [.setPriority(priority)](#vscp_dot_Event_and_setPriority)
    * [.getPriority()](#vscp_dot_Event_and_getPriority) ⇒ <code>number</code>
    * [.setHardCodedAddr()](#vscp_dot_Event_and_setHardCodedAddr)
    * [.isHardCodedAddr()](#vscp_dot_Event_and_isHardCodedAddr) ⇒ <code>boolean</code>
    * [.setDoNotCalcCRC()](#vscp_dot_Event_and_setDoNotCalcCRC)
    * [.isDoNotCalcCRC()](#vscp_dot_Event_and_isDoNotCalcCRC) ⇒ <code>boolean</code>
    * [.getText()](#vscp_dot_Event_and_getText) ⇒ <code>string</code>

<a id="new_vscp_dot_Event_new"></a>

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
| options.vscpData | <code>Array.&lt;number&gt;</code> \| <code>string</code> | Event data |

<a id="vscp_dot_Event_and_vscpHead"></a>

#### event.vscpHead : <code>number</code>
VSCP event head

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpClass"></a>

#### event.vscpClass : <code>number</code>
VSCP class

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpType"></a>

#### event.vscpType : <code>number</code>
VSCP type

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpObId"></a>

#### event.vscpObId : <code>number</code>
VSCP object id used by driver for channel info and etc.

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpTimeStamp"></a>

#### event.vscpTimeStamp : <code>number</code>
Relative timestamp for package in us

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpDateTime"></a>

#### event.vscpDateTime : <code>date</code>
Date/Time for package

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpGuid"></a>

#### event.vscpGuid : <code>string</code>
Node global unique id LSB(15) -> MSB(0)

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_vscpData"></a>

#### event.vscpData : <code>Array.&lt;number&gt;</code> \| <code>string</code>
Data array or string

**Kind**: instance property of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_setIPV6Addr"></a>

#### event.setIPV6Addr()
Set GUID as IP v6 address

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isIPV6Addr"></a>

#### event.isIPV6Addr() ⇒ <code>boolean</code>
Is GUID a IP v6 address or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the GUID is a IP v6 address, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setDumbNode"></a>

#### event.setDumbNode()
Set dumb node. No MDF, registers, nothing.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isDumbNode"></a>

#### event.isDumbNode() ⇒ <code>boolean</code>
Is node a dump node or not?
Dumb node means no MDF, registers, nothing.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the node is a dumb node, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setPriority"></a>

#### event.setPriority(priority)
Set the VSCP event priority.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  

| Param | Type | Description |
| --- | --- | --- |
| priority | <code>number</code> | Priority |

<a id="vscp_dot_Event_and_getPriority"></a>

#### event.getPriority() ⇒ <code>number</code>
Get the VSCP event priority.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>number</code> - Priority of the event.  
<a id="vscp_dot_Event_and_setHardCodedAddr"></a>

#### event.setHardCodedAddr()
Set the node id of the event sender as hard coded?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isHardCodedAddr"></a>

#### event.isHardCodedAddr() ⇒ <code>boolean</code>
Is the node id of the event sender hard coded or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If the node id is hard coded, it will return true, otherwise false.  
<a id="vscp_dot_Event_and_setDoNotCalcCRC"></a>

#### event.setDoNotCalcCRC()
Set flag for no CRC calculation?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
<a id="vscp_dot_Event_and_isDoNotCalcCRC"></a>

#### event.isDoNotCalcCRC() ⇒ <code>boolean</code>
Is CRC calculated or not?

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>boolean</code> - If nor CRC should be calculated true is returned.  
<a id="vscp_dot_Event_and_getText"></a>

#### event.getText() ⇒ <code>string</code>
Get event as string.

**Kind**: instance method of [<code>Event</code>](#vscp_dot_Event)  
**Returns**: <code>string</code> - Event as string  
<a id="vscp_dot_version"></a>

### vscp.version
VSCP websocket library version

**Kind**: static property of [<code>vscp</code>](#vscp)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| major | <code>number</code> | Major version number |
| minor | <code>number</code> | Minor version number |
| patch | <code>number</code> | Sub-minor version number |

<a id="vscp_dot_constants"></a>

### vscp.constants : <code>object</code>
VSCP constants

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.constants](#vscp_dot_constants) : <code>object</code>
    * [.classes](#vscp_dot_constants_dot_classes) : <code>enum</code>
    * [.types](#vscp_dot_constants_dot_types) : <code>enum</code>
    * [.priorities](#vscp_dot_constants_dot_priorities) : <code>enum</code>
    * [.varTypes](#vscp_dot_constants_dot_varTypes) : <code>enum</code>
    * [.varTypeNames](#vscp_dot_constants_dot_varTypeNames)

<a id="vscp_dot_constants_dot_classes"></a>

#### constants.classes : <code>enum</code>
VSCP classes

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_types"></a>

#### constants.types : <code>enum</code>
VSCP class types

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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
| VSCP_TYPE_INFORMATION_DATETIME | <code>number</code> | <code>77</code> | 
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

<a id="vscp_dot_constants_dot_priorities"></a>

#### constants.priorities : <code>enum</code>
VSCP class priorities

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_varTypes"></a>

#### constants.varTypes : <code>enum</code>
VSCP variable types

**Kind**: static enum of [<code>constants</code>](#vscp_dot_constants)  
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

<a id="vscp_dot_constants_dot_varTypeNames"></a>

#### constants.varTypeNames
VSCP variable type names as string. Use to fill drop down boxes and similar.

**Kind**: static constant of [<code>constants</code>](#vscp_dot_constants)  
<a id="vscp_dot_utility"></a>

### vscp.utility : <code>object</code>
Utility functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.utility](#vscp_dot_utility) : <code>object</code>
    * [.readValue(input)](#vscp_dot_utility_dot_readValue) ⇒ <code>number</code>
    * [.getTime()](#vscp_dot_utility_dot_getTime) ⇒ <code>string</code>
    * [.guidToStr(guid)](#vscp_dot_utility_dot_guidToStr) ⇒ <code>string</code>
    * [.strToGuid(guid)](#vscp_dot_utility_dot_strToGuid) ⇒ <code>Array.&lt;number&gt;</code>
    * [.getNodeId(guid)](#vscp_dot_utility_dot_getNodeId) ⇒ <code>number</code>

<a id="vscp_dot_utility_dot_readValue"></a>

#### utility.readValue(input) ⇒ <code>number</code>
Read a hex or decimal value and return as an integer.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>number</code> - Value  

| Param | Type | Description |
| --- | --- | --- |
| input | <code>string</code> | Hex or decimal value as string |

<a id="vscp_dot_utility_dot_getTime"></a>

#### utility.getTime() ⇒ <code>string</code>
Utility function which returns the current time in the following format: hh:mm:ss.us

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>string</code> - Current time in the format hh:mm:ss.us  
<a id="vscp_dot_utility_dot_guidToStr"></a>

#### utility.guidToStr(guid) ⇒ <code>string</code>
Converts a GUID number array to a GUID string.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>string</code> - GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>Array.&lt;number&gt;</code> | GUID number array |

<a id="vscp_dot_utility_dot_strToGuid"></a>

#### utility.strToGuid(guid) ⇒ <code>Array.&lt;number&gt;</code>
Converts a GUID string to a GUID number array.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>Array.&lt;number&gt;</code> - GUID number array  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp_dot_utility_dot_getNodeId"></a>

#### utility.getNodeId(guid) ⇒ <code>number</code>
Get node id from a node GUID string.

**Kind**: static method of [<code>utility</code>](#vscp_dot_utility)  
**Returns**: <code>number</code> - Node id  

| Param | Type | Description |
| --- | --- | --- |
| guid | <code>string</code> | GUID string, e.g. 00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00 |

<a id="vscp_dot_mdf"></a>

### vscp.mdf : <code>object</code>
VSCP module description file handling functionality

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.mdf](#vscp_dot_mdf) : <code>object</code>
    * [.Register](#vscp_dot_mdf_dot_Register)
        * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
        * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
        * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
        * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
        * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
        * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
        * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
        * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
        * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
        * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
        * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)
    * [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
        * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
        * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
        * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
        * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
        * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
        * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
        * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
        * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
        * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
        * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
        * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
        * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
        * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
        * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)
    * [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
        * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
        * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
        * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
        * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)
    * [.timeout](#vscp_dot_mdf_dot_timeout) : <code>number</code>
    * [.load(options)](#vscp_dot_mdf_dot_load)
    * [.loadLocal(options)](#vscp_dot_mdf_dot_loadLocal)
    * [.readAbstractValue(options)](#vscp_dot_mdf_dot_readAbstractValue)
    * [.writeAbstractValue(options)](#vscp_dot_mdf_dot_writeAbstractValue)
    * [.writeAbstractBits(options)](#vscp_dot_mdf_dot_writeAbstractBits)
    * [.getRegisters(options)](#vscp_dot_mdf_dot_getRegisters) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
    * [.getAbstractions(options)](#vscp_dot_mdf_dot_getAbstractions) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)

<a id="vscp_dot_mdf_dot_Register"></a>

#### mdf.Register
**Kind**: static class of [<code>mdf</code>](#vscp_dot_mdf)  

* [.Register](#vscp_dot_mdf_dot_Register)
    * [new vscp.mdf.Register()](#new_vscp_dot_mdf_dot_Register_new)
    * [.name](#vscp_dot_mdf_dot_Register_and_name) : <code>string</code>
    * [.description](#vscp_dot_mdf_dot_Register_and_description) : <code>string</code>
    * [.readAccess](#vscp_dot_mdf_dot_Register_and_readAccess) : <code>boolean</code>
    * [.writeAccess](#vscp_dot_mdf_dot_Register_and_writeAccess) : <code>boolean</code>
    * [.page](#vscp_dot_mdf_dot_Register_and_page) : <code>number</code>
    * [.offset](#vscp_dot_mdf_dot_Register_and_offset) : <code>number</code>
    * [.value](#vscp_dot_mdf_dot_Register_and_value) : <code>number</code>
    * [.dirty](#vscp_dot_mdf_dot_Register_and_dirty) : <code>number</code>
    * [.userData](#vscp_dot_mdf_dot_Register_and_userData) : <code>object</code>
    * [.setValue(value)](#vscp_dot_mdf_dot_Register_and_setValue)

<a id="new_vscp_dot_mdf_dot_Register_new"></a>

##### new vscp.mdf.Register()
MDF register with all parameters.

<a id="vscp_dot_mdf_dot_Register_and_name"></a>

##### register.name : <code>string</code>
Register name

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_description"></a>

##### register.description : <code>string</code>
Register description

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_readAccess"></a>

##### register.readAccess : <code>boolean</code>
Read access to the register allowed or not

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_writeAccess"></a>

##### register.writeAccess : <code>boolean</code>
Write access to the register allowed or not

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_page"></a>

##### register.page : <code>number</code>
Page where the register is located

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_offset"></a>

##### register.offset : <code>number</code>
Offset where the register is located on the page

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_value"></a>

##### register.value : <code>number</code>
Register value

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_dirty"></a>

##### register.dirty : <code>number</code>
Marks the register value dirty, which means the user changed it.It can be used to detect which registers have to be written to the node.

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_userData"></a>

##### register.userData : <code>object</code>
User specific data

**Kind**: instance property of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  
<a id="vscp_dot_mdf_dot_Register_and_setValue"></a>

##### register.setValue(value)
This function set a register value and marks it dirty.

**Kind**: instance method of [<code>Register</code>](#vscp_dot_mdf_dot_Register)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | New value |

<a id="vscp_dot_mdf_dot_Abstraction"></a>

#### mdf.Abstraction
**Kind**: static class of [<code>mdf</code>](#vscp_dot_mdf)  

* [.Abstraction](#vscp_dot_mdf_dot_Abstraction)
    * [new vscp.mdf.Abstraction()](#new_vscp_dot_mdf_dot_Abstraction_new)
    * [.name](#vscp_dot_mdf_dot_Abstraction_and_name) : <code>string</code>
    * [.description](#vscp_dot_mdf_dot_Abstraction_and_description) : <code>string</code>
    * [.readAccess](#vscp_dot_mdf_dot_Abstraction_and_readAccess) : <code>boolean</code>
    * [.writeAccess](#vscp_dot_mdf_dot_Abstraction_and_writeAccess) : <code>boolean</code>
    * [.id](#vscp_dot_mdf_dot_Abstraction_and_id) : <code>string</code>
    * [.page](#vscp_dot_mdf_dot_Abstraction_and_page) : <code>number</code>
    * [.offset](#vscp_dot_mdf_dot_Abstraction_and_offset) : <code>number</code>
    * [.value](#vscp_dot_mdf_dot_Abstraction_and_value) : <code>number</code>
    * [.type](#vscp_dot_mdf_dot_Abstraction_and_type) : <code>string</code>
    * [.defValue](#vscp_dot_mdf_dot_Abstraction_and_defValue) : <code>number</code>
    * [.dirty](#vscp_dot_mdf_dot_Abstraction_and_dirty) : <code>number</code>
    * [.userData](#vscp_dot_mdf_dot_Abstraction_and_userData) : <code>object</code>
    * [.setValue(value)](#vscp_dot_mdf_dot_Abstraction_and_setValue)

<a id="new_vscp_dot_mdf_dot_Abstraction_new"></a>

##### new vscp.mdf.Abstraction()
MDF abstraction with all parameters.

<a id="vscp_dot_mdf_dot_Abstraction_and_name"></a>

##### abstraction.name : <code>string</code>
Abstraction name

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_description"></a>

##### abstraction.description : <code>string</code>
Abstraction description

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_readAccess"></a>

##### abstraction.readAccess : <code>boolean</code>
Read access to the abstraction allowed or not

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_writeAccess"></a>

##### abstraction.writeAccess : <code>boolean</code>
Write access to the abstraction allowed or not

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_id"></a>

##### abstraction.id : <code>string</code>
Abstraction id

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_page"></a>

##### abstraction.page : <code>number</code>
Page where the abstraction is located

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_offset"></a>

##### abstraction.offset : <code>number</code>
Offset where the abstraction is located

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_value"></a>

##### abstraction.value : <code>number</code>
Abstraction value

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_type"></a>

##### abstraction.type : <code>string</code>
Abstraction type

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_defValue"></a>

##### abstraction.defValue : <code>number</code>
Abstraction default value

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_dirty"></a>

##### abstraction.dirty : <code>number</code>
Marks the abstraction value dirty, which means the user changed it.It can be used to detect which abstractions have to be written to the node.

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_userData"></a>

##### abstraction.userData : <code>object</code>
User specific data

**Kind**: instance property of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  
<a id="vscp_dot_mdf_dot_Abstraction_and_setValue"></a>

##### abstraction.setValue(value)
This function set a abstraction value and marks it dirty.

**Kind**: instance method of [<code>Abstraction</code>](#vscp_dot_mdf_dot_Abstraction)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | New value |

<a id="vscp_dot_mdf_dot_constants"></a>

#### mdf.constants : <code>object</code>
MDF specific constants

**Kind**: static namespace of [<code>mdf</code>](#vscp_dot_mdf)  

* [.constants](#vscp_dot_mdf_dot_constants) : <code>object</code>
    * [.TYPE_SIZES](#vscp_dot_mdf_dot_constants_dot_TYPE_SIZES) : <code>enum</code>
    * [.CONVERSION_FROM_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL)
    * [.CONVERSION_TO_DECIMAL](#vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL)
    * [.RANGE](#vscp_dot_mdf_dot_constants_dot_RANGE)

<a id="vscp_dot_mdf_dot_constants_dot_TYPE_SIZES"></a>

##### constants.TYPE_SIZES : <code>enum</code>
MDF type sizes in bytes

**Kind**: static enum of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| string | <code>number</code> | <code>0</code> | 
| bitfield | <code>number</code> | <code>1</code> | 
| bool | <code>number</code> | <code>1</code> | 
| int8_t | <code>number</code> | <code>1</code> | 
| uint8_t | <code>number</code> | <code>1</code> | 
| int16_t | <code>number</code> | <code>2</code> | 
| uint16_t | <code>number</code> | <code>2</code> | 
| int32_t | <code>number</code> | <code>4</code> | 
| uint32_t | <code>number</code> | <code>4</code> | 
| int64_t | <code>number</code> | <code>8</code> | 
| uint64_t | <code>number</code> | <code>8</code> | 
| float | <code>number</code> | <code>4</code> | 
| double | <code>number</code> | <code>8</code> | 
| date | <code>number</code> | <code>4</code> | 
| time | <code>number</code> | <code>4</code> | 
| guid | <code>number</code> | <code>16</code> | 
| char | <code>number</code> | <code>1</code> | 
| byte | <code>number</code> | <code>1</code> | 
| short | <code>number</code> | <code>2</code> | 
| integer | <code>number</code> | <code>2</code> | 
| long | <code>number</code> | <code>4</code> | 

<a id="vscp_dot_mdf_dot_constants_dot_CONVERSION_FROM_DECIMAL"></a>

##### constants.CONVERSION_FROM_DECIMAL
Conversion functions from decimal

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_constants_dot_CONVERSION_TO_DECIMAL"></a>

##### constants.CONVERSION_TO_DECIMAL
Conversion functions to decimal

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_constants_dot_RANGE"></a>

##### constants.RANGE
Type ranges

**Kind**: static constant of [<code>constants</code>](#vscp_dot_mdf_dot_constants)  
<a id="vscp_dot_mdf_dot_timeout"></a>

#### mdf.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>mdf</code>](#vscp_dot_mdf)  
<a id="vscp_dot_mdf_dot_load"></a>

#### mdf.load(options)
Get the MDF as xml document from a URL.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.url | <code>function</code> | URL to MDF file |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_loadLocal"></a>

#### mdf.loadLocal(options)
Get the MDF as xml document from local file system.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.fileRef | <code>function</code> | File reference to MDF file |
| options.onSuccess | <code>function</code> | If the xml file is successful loaded, this function will be called. |
| [options.onError] | <code>function</code> | If loading the xml file failed, this function will be called. |

<a id="vscp_dot_mdf_dot_readAbstractValue"></a>

#### mdf.readAbstractValue(options)
Read a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_writeAbstractValue"></a>

#### mdf.writeAbstractValue(options)
Write a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.value | <code>string</code> | Abstract value |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_writeAbstractBits"></a>

#### mdf.writeAbstractBits(options)
Change some bits in a abstract value.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.mdf | <code>object</code> | MDF as xml jquery object |
| options.id | <code>number</code> | Abstract value id |
| options.pos | <code>number</code> | Bit position |
| options.width | <code>number</code> | Bit width |
| options.value | <code>string</code> | Abstract value |
| options.onSuccess | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_mdf_dot_getRegisters"></a>

#### mdf.getRegisters(options) ⇒ [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register)
This function retrieves all register informations from a mdf.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  
**Returns**: [<code>Array.&lt;Register&gt;</code>](#vscp_dot_mdf_dot_Register) - Array of MDF registers  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | MDF as jquery object |

<a id="vscp_dot_mdf_dot_getAbstractions"></a>

#### mdf.getAbstractions(options) ⇒ [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction)
This function retrieves all abstraction informations from a mdf.

**Kind**: static method of [<code>mdf</code>](#vscp_dot_mdf)  
**Returns**: [<code>Array.&lt;Abstraction&gt;</code>](#vscp_dot_mdf_dot_Abstraction) - Array of MDF abstractions  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | MDF as jquery object |

<a id="vscp_dot_measurement"></a>

### vscp.measurement : <code>object</code>
VSCP measurement stuff

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.measurement](#vscp_dot_measurement) : <code>object</code>
    * [.Decoder](#vscp_dot_measurement_dot_Decoder)
        * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
        * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
        * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
        * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>
    * [.constants](#vscp_dot_measurement_dot_constants) : <code>object</code>
        * [.units](#vscp_dot_measurement_dot_constants_dot_units) : <code>Array.&lt;string&gt;</code>
    * [.timeout](#vscp_dot_measurement_dot_timeout) : <code>number</code>
    * [.toFixed(value, precision)](#vscp_dot_measurement_dot_toFixed) ⇒ <code>number</code>
    * [.varInteger2Float(data)](#vscp_dot_measurement_dot_varInteger2Float) ⇒ <code>number</code>
    * [.getDataCoding(data)](#vscp_dot_measurement_dot_getDataCoding) ⇒ <code>number</code>
    * [.getUnitFromDataCoding(data)](#vscp_dot_measurement_dot_getUnitFromDataCoding) ⇒ <code>number</code>
    * [.getSensorIndexFromDataCoding(data)](#vscp_dot_measurement_dot_getSensorIndexFromDataCoding) ⇒ <code>number</code>
    * [.decodeClass10(data)](#vscp_dot_measurement_dot_decodeClass10) ⇒ <code>number</code>
    * [.decodeClass60Number(data)](#vscp_dot_measurement_dot_decodeClass60Number) ⇒ <code>number</code>
    * [.decodeClass65Number(data)](#vscp_dot_measurement_dot_decodeClass65Number) ⇒ <code>number</code>
    * [.convertFahrenheitToKelvin(value)](#vscp_dot_measurement_dot_convertFahrenheitToKelvin) ⇒ <code>number</code>
    * [.convertFahrenheitToCelsius(value)](#vscp_dot_measurement_dot_convertFahrenheitToCelsius) ⇒ <code>number</code>
    * [.convertCelsiusToFahrenheit(value)](#vscp_dot_measurement_dot_convertCelsiusToFahrenheit) ⇒ <code>number</code>
    * [.convertKelvinToCelsius(value)](#vscp_dot_measurement_dot_convertKelvinToCelsius) ⇒ <code>number</code>
    * [.convertCelsiusToKelvin(value)](#vscp_dot_measurement_dot_convertCelsiusToKelvin) ⇒ <code>number</code>
    * [.convertKelvinToFahrenheit(value)](#vscp_dot_measurement_dot_convertKelvinToFahrenheit) ⇒ <code>number</code>
    * [.convertMeterToFeet(value)](#vscp_dot_measurement_dot_convertMeterToFeet) ⇒ <code>number</code>
    * [.convertFeetToMeter(value)](#vscp_dot_measurement_dot_convertFeetToMeter) ⇒ <code>number</code>
    * [.convertMeterToInch(value)](#vscp_dot_measurement_dot_convertMeterToInch) ⇒ <code>number</code>
    * [.convertInchToMeter(value)](#vscp_dot_measurement_dot_convertInchToMeter) ⇒ <code>number</code>

<a id="vscp_dot_measurement_dot_Decoder"></a>

#### measurement.Decoder
**Kind**: static class of [<code>measurement</code>](#vscp_dot_measurement)  

* [.Decoder](#vscp_dot_measurement_dot_Decoder)
    * [new vscp.measurement.Decoder(options)](#new_vscp_dot_measurement_dot_Decoder_new)
    * [.client](#vscp_dot_measurement_dot_Decoder_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
    * [.onValue](#vscp_dot_measurement_dot_Decoder_and_onValue) : <code>function</code>
    * [.filter](#vscp_dot_measurement_dot_Decoder_and_filter) : <code>object</code>

<a id="new_vscp_dot_measurement_dot_Decoder_new"></a>

##### new vscp.measurement.Decoder(options)
Measurement decoder


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.onValue | <code>function</code> | Function which will be called for every received measurement value. |
| options.filter | <code>object</code> | Filter |
| options.filter.vscpGuid | <code>string</code> | Node GUID string |
| options.filter.vscpClass | <code>number</code> | VSCP class |
| options.filter.vscpType | <code>number</code> | VSCP type |
| options.filter.sensorIndex | <code>number</code> | Sensor index |
| options.filter.zone | <code>number</code> | Zone |
| options.filter.subZone | <code>number</code> | Sub-zone |

<a id="vscp_dot_measurement_dot_Decoder_and_client"></a>

##### decoder.client : [<code>Client</code>](#vscp_dot_ws_dot_Client)
VSCP websocket client

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
<a id="vscp_dot_measurement_dot_Decoder_and_onValue"></a>

##### decoder.onValue : <code>function</code>
Callback which will be called for every received value.

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
<a id="vscp_dot_measurement_dot_Decoder_and_filter"></a>

##### decoder.filter : <code>object</code>
Filter

**Kind**: instance property of [<code>Decoder</code>](#vscp_dot_measurement_dot_Decoder)  
**Properties**

| Name | Type | Description |
| --- | --- | --- |
| vscpGuid | <code>string</code> | Node GUID string |
| vscpClass | <code>number</code> | VSCP class |
| vscpType | <code>number</code> | VSCP type |
| datetime | <code>date</code> | datetime |
| sensorIndex | <code>number</code> | Sensor index |
| zone | <code>number</code> | Zone |
| subZone | <code>number</code> | Sub-zone |

<a id="vscp_dot_measurement_dot_constants"></a>

#### measurement.constants : <code>object</code>
Measurement specific constants

**Kind**: static namespace of [<code>measurement</code>](#vscp_dot_measurement)  
<a id="vscp_dot_measurement_dot_constants_dot_units"></a>

##### constants.units : <code>Array.&lt;string&gt;</code>
VSCP units

**Kind**: static property of [<code>constants</code>](#vscp_dot_measurement_dot_constants)  
<a id="vscp_dot_measurement_dot_timeout"></a>

#### measurement.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>measurement</code>](#vscp_dot_measurement)  
<a id="vscp_dot_measurement_dot_toFixed"></a>

#### measurement.toFixed(value, precision) ⇒ <code>number</code>
Round value to a fixed precision.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Rounded value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>number</code> | Value |
| precision | <code>number</code> | Precision |

<a id="vscp_dot_measurement_dot_varInteger2Float"></a>

#### measurement.varInteger2Float(data) ⇒ <code>number</code>
Convert a integer value to float

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Float value  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>Array.&lt;number&gt;</code> | Byte array |

<a id="vscp_dot_measurement_dot_getDataCoding"></a>

#### measurement.getDataCoding(data) ⇒ <code>number</code>
Get data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Coding  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_getUnitFromDataCoding"></a>

#### measurement.getUnitFromDataCoding(data) ⇒ <code>number</code>
Get unit from data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Unit  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data coding |

<a id="vscp_dot_measurement_dot_getSensorIndexFromDataCoding"></a>

#### measurement.getSensorIndexFromDataCoding(data) ⇒ <code>number</code>
Get sensor index from data coding.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Sensor index  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data coding |

<a id="vscp_dot_measurement_dot_decodeClass10"></a>

#### measurement.decodeClass10(data) ⇒ <code>number</code>
Decode a class 10 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>Array.&lt;number&gt;</code> | Data (event data array where first data byte is the data coding) |

<a id="vscp_dot_measurement_dot_decodeClass60Number"></a>

#### measurement.decodeClass60Number(data) ⇒ <code>number</code>
Decode a class 60 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_decodeClass65Number"></a>

#### measurement.decodeClass65Number(data) ⇒ <code>number</code>
Decode a class 65 measurement.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Value as float  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>number</code> | Data |

<a id="vscp_dot_measurement_dot_convertFahrenheitToKelvin"></a>

#### measurement.convertFahrenheitToKelvin(value) ⇒ <code>number</code>
Convert from unit fahrenheit to unit kelvin.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertFahrenheitToCelsius"></a>

#### measurement.convertFahrenheitToCelsius(value) ⇒ <code>number</code>
Convert from unit fahrenheit to unit celsius.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertCelsiusToFahrenheit"></a>

#### measurement.convertCelsiusToFahrenheit(value) ⇒ <code>number</code>
Convert from unit celsius to unit fahrenheit.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertKelvinToCelsius"></a>

#### measurement.convertKelvinToCelsius(value) ⇒ <code>number</code>
Convert from unit kelvin to unit celsius.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertCelsiusToKelvin"></a>

#### measurement.convertCelsiusToKelvin(value) ⇒ <code>number</code>
Convert from unit celsius to unit kelvin.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertKelvinToFahrenheit"></a>

#### measurement.convertKelvinToFahrenheit(value) ⇒ <code>number</code>
Convert from unit kelvin to unit fahrenheit.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertMeterToFeet"></a>

#### measurement.convertMeterToFeet(value) ⇒ <code>number</code>
Convert from unit meter to unit feet.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertFeetToMeter"></a>

#### measurement.convertFeetToMeter(value) ⇒ <code>number</code>
Convert from unit feet to unit meter.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertMeterToInch"></a>

#### measurement.convertMeterToInch(value) ⇒ <code>number</code>
Convert from unit meter to unit inch.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_measurement_dot_convertInchToMeter"></a>

#### measurement.convertInchToMeter(value) ⇒ <code>number</code>
Convert from unit inch to unit meter.

**Kind**: static method of [<code>measurement</code>](#vscp_dot_measurement)  
**Returns**: <code>number</code> - Converted value  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>string</code> \| <code>number</code> | Value |

<a id="vscp_dot_register"></a>

### vscp.register : <code>object</code>
VSCP register access functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.register](#vscp_dot_register) : <code>object</code>
    * [.constants](#vscp_dot_register_dot_constants) : <code>enum</code>
    * [.timeout](#vscp_dot_register_dot_timeout) : <code>number</code>
    * [.read(options)](#vscp_dot_register_dot_read)
    * [.write(options)](#vscp_dot_register_dot_write)
    * [.writeBits(options)](#vscp_dot_register_dot_writeBits)
    * [.readAlarmStatus(options)](#vscp_dot_register_dot_readAlarmStatus)
    * [.readVscpVersion(options)](#vscp_dot_register_dot_readVscpVersion)
    * [.readNodeControlFlags(options)](#vscp_dot_register_dot_readNodeControlFlags)
    * [.readUserId(options)](#vscp_dot_register_dot_readUserId)
    * [.readManufacturerDevId(options)](#vscp_dot_register_dot_readManufacturerDevId)
    * [.readManufacturerSubDevId(options)](#vscp_dot_register_dot_readManufacturerSubDevId)
    * [.readNicknameId(options)](#vscp_dot_register_dot_readNicknameId)
    * [.readSelectedPage(options)](#vscp_dot_register_dot_readSelectedPage)
    * [.readFirmwareVersion(options)](#vscp_dot_register_dot_readFirmwareVersion)
    * [.readBootloaderAlgorithm(options)](#vscp_dot_register_dot_readBootloaderAlgorithm)
    * [.readUsedPages(options)](#vscp_dot_register_dot_readUsedPages)
    * [.readStdDevFamCode(options)](#vscp_dot_register_dot_readStdDevFamCode)
    * [.readStdDevType(options)](#vscp_dot_register_dot_readStdDevType)
    * [.readGUID(options)](#vscp_dot_register_dot_readGUID)
    * [.readMdfUrl(options)](#vscp_dot_register_dot_readMdfUrl)

<a id="vscp_dot_register_dot_constants"></a>

#### register.constants : <code>enum</code>
VSCP registers

**Kind**: static enum of [<code>register</code>](#vscp_dot_register)  
**Properties**

| Name | Type | Default |
| --- | --- | --- |
| ALARM_STATUS | <code>number</code> | <code>128</code> | 
| VSCP_VERSION_MAJOR | <code>number</code> | <code>129</code> | 
| VSCP_VERSION_MINOR | <code>number</code> | <code>130</code> | 
| NODE_CONTROL_FLAGS | <code>number</code> | <code>131</code> | 
| USER_ID_0 | <code>number</code> | <code>132</code> | 
| USER_ID_1 | <code>number</code> | <code>133</code> | 
| USER_ID_2 | <code>number</code> | <code>134</code> | 
| USER_ID_3 | <code>number</code> | <code>135</code> | 
| USER_ID_4 | <code>number</code> | <code>136</code> | 
| MANUFACTURER_DEV_ID_0 | <code>number</code> | <code>137</code> | 
| MANUFACTURER_DEV_ID_1 | <code>number</code> | <code>138</code> | 
| MANUFACTURER_DEV_ID_2 | <code>number</code> | <code>139</code> | 
| MANUFACTURER_DEV_ID_3 | <code>number</code> | <code>140</code> | 
| MANUFACTURER_SUB_DEV_ID_0 | <code>number</code> | <code>141</code> | 
| MANUFACTURER_SUB_DEV_ID_1 | <code>number</code> | <code>142</code> | 
| MANUFACTURER_SUB_DEV_ID_2 | <code>number</code> | <code>143</code> | 
| MANUFACTURER_SUB_DEV_ID_3 | <code>number</code> | <code>144</code> | 
| NICKNAME_ID | <code>number</code> | <code>145</code> | 
| PAGE_SELECT_MSB | <code>number</code> | <code>146</code> | 
| PAGE_SELECT_LSB | <code>number</code> | <code>147</code> | 
| FIRMWARE_VERSION_MAJOR | <code>number</code> | <code>148</code> | 
| FIRMWARE_VERSION_MINOR | <code>number</code> | <code>149</code> | 
| FIRMWARE_VERSION_SUB_MINOR | <code>number</code> | <code>150</code> | 
| BOOT_LOADER_ALGORITHM | <code>number</code> | <code>151</code> | 
| BUFFER_SIZE | <code>number</code> | <code>152</code> | 
| PAGES_USED | <code>number</code> | <code>153</code> | 
| STD_DEV_FAMILY_CODE_3 | <code>number</code> | <code>154</code> | 
| STD_DEV_FAMILY_CODE_2 | <code>number</code> | <code>155</code> | 
| STD_DEV_FAMILY_CODE_1 | <code>number</code> | <code>156</code> | 
| STD_DEV_FAMILY_CODE_0 | <code>number</code> | <code>157</code> | 
| STD_DEV_TYPE_3 | <code>number</code> | <code>158</code> | 
| STD_DEV_TYPE_2 | <code>number</code> | <code>159</code> | 
| STD_DEV_TYPE_1 | <code>number</code> | <code>160</code> | 
| STD_DEV_TYPE_0 | <code>number</code> | <code>161</code> | 
| RESTORE_STD_CFG | <code>number</code> | <code>162</code> | 
| GUID | <code>number</code> | <code>208</code> | 
| MDF_URL | <code>number</code> | <code>224</code> | 

<a id="vscp_dot_register_dot_timeout"></a>

#### register.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>register</code>](#vscp_dot_register)  
<a id="vscp_dot_register_dot_read"></a>

#### register.read(options)
Read one or more register values.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| [options.page] | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.count | <code>number</code> | Number of registers to read |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_write"></a>

#### register.write(options)
Write one or more register values.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.page | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.data | <code>Array.&lt;number&gt;</code> | Data array |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_writeBits"></a>

#### register.writeBits(options)
Change some bits of a register.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP connection |
| options.nodeId | <code>number</code> | Node id |
| options.page | <code>number</code> | Register page |
| options.offset | <code>number</code> | Register page offset |
| options.pos | <code>number</code> | Bit position |
| options.width | <code>number</code> | Bit width |
| options.data | <code>Array.&lt;number&gt;</code> | Data array |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readAlarmStatus"></a>

#### register.readAlarmStatus(options)
Read the alarm status from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readVscpVersion"></a>

#### register.readVscpVersion(options)
Read the supported VSCP version from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readNodeControlFlags"></a>

#### register.readNodeControlFlags(options)
Read the node control flags from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readUserId"></a>

#### register.readUserId(options)
Read the user id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readManufacturerDevId"></a>

#### register.readManufacturerDevId(options)
Read the manufacturer device id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readManufacturerSubDevId"></a>

#### register.readManufacturerSubDevId(options)
Read the manufacturer sub device id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readNicknameId"></a>

#### register.readNicknameId(options)
Read the nickname id from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readSelectedPage"></a>

#### register.readSelectedPage(options)
Read the current selected page from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readFirmwareVersion"></a>

#### register.readFirmwareVersion(options)
Read the firmware version from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readBootloaderAlgorithm"></a>

#### register.readBootloaderAlgorithm(options)
Read the bootloader algorithm from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readUsedPages"></a>

#### register.readUsedPages(options)
Read the number of used pages from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readStdDevFamCode"></a>

#### register.readStdDevFamCode(options)
Read the standard device family code from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readStdDevType"></a>

#### register.readStdDevType(options)
Read the standard device type from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readGUID"></a>

#### register.readGUID(options)
Read the GUID from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_register_dot_readMdfUrl"></a>

#### register.readMdfUrl(options)
Read the MDF URL from a node.

**Kind**: static method of [<code>register</code>](#vscp_dot_register)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_rest"></a>

### vscp.rest : <code>object</code>
VSCP REST api functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.rest](#vscp_dot_rest) : <code>object</code>
    * [.Client](#vscp_dot_rest_dot_Client)
        * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
        * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
        * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
        * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
        * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
        * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
        * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
        * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
        * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
        * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
        * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
        * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
        * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
        * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
        * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
        * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
        * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>

<a id="vscp_dot_rest_dot_Client"></a>

#### rest.Client
**Kind**: static class of [<code>rest</code>](#vscp_dot_rest)  

* [.Client](#vscp_dot_rest_dot_Client)
    * [new vscp.rest.Client(config)](#new_vscp_dot_rest_dot_Client_new)
    * [.baseUrl](#vscp_dot_rest_dot_Client_and_baseUrl) : <code>string</code>
    * [.pathPrefix](#vscp_dot_rest_dot_Client_and_pathPrefix) : <code>string</code>
    * [.apiVersion](#vscp_dot_rest_dot_Client_and_apiVersion) : <code>string</code>
    * [.sessionKey](#vscp_dot_rest_dot_Client_and_sessionKey) : <code>string</code>
    * [.openSession(options)](#vscp_dot_rest_dot_Client_and_openSession) ⇒ <code>object</code>
    * [.closeSession([options])](#vscp_dot_rest_dot_Client_and_closeSession) ⇒ <code>object</code>
    * [.getStatus([options])](#vscp_dot_rest_dot_Client_and_getStatus) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp_dot_rest_dot_Client_and_sendEvent) ⇒ <code>object</code>
    * [.readEvent([options])](#vscp_dot_rest_dot_Client_and_readEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp_dot_rest_dot_Client_and_setFilter) ⇒ <code>object</code>
    * [.clearQueue([options])](#vscp_dot_rest_dot_Client_and_clearQueue) ⇒ <code>object</code>
    * [.createVar(options)](#vscp_dot_rest_dot_Client_and_createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp_dot_rest_dot_Client_and_readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp_dot_rest_dot_Client_and_writeVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp_dot_rest_dot_Client_and_removeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp_dot_rest_dot_Client_and_listVar) ⇒ <code>object</code>

<a id="new_vscp_dot_rest_dot_Client_new"></a>

##### new vscp.rest.Client(config)
The VSCP client class handles the basic REST api of the VSCP daemon.The function interface uses jquery ajax call in the background and willreturn a Promise.


| Param | Type | Description |
| --- | --- | --- |
| config | <code>string</code> | Configuration |
| [config.baseUrl] | <code>string</code> | VSCP daemon URL (protocol + hostname + port) |
| [options.pathPrefix] | <code>string</code> | Path prefix (default: '/vscp'), which comes right after the base url. |
| [options.apiVersion] | <code>string</code> | API version (for future use) |

<a id="vscp_dot_rest_dot_Client_and_baseUrl"></a>

##### client.baseUrl : <code>string</code>
Base URL

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_pathPrefix"></a>

##### client.pathPrefix : <code>string</code>
Path prefix

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_apiVersion"></a>

##### client.apiVersion : <code>string</code>
REST API version (future use)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_sessionKey"></a>

##### client.sessionKey : <code>string</code>
Session key

**Kind**: instance property of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
<a id="vscp_dot_rest_dot_Client_and_openSession"></a>

##### client.openSession(options) ⇒ <code>object</code>
Open a session.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.user | <code>string</code> | User name |
| options.password | <code>string</code> | Password |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_closeSession"></a>

##### client.closeSession([options]) ⇒ <code>object</code>
Close a session.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_getStatus"></a>

##### client.getStatus([options]) ⇒ <code>object</code>
Get status and how many events are in the queue.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_sendEvent"></a>

##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | <code>object</code> | VSCP event |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_readEvent"></a>

##### client.readEvent([options]) ⇒ <code>object</code>
Read one or more VSCP events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.count] | <code>object</code> | Number of events to read |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_setFilter"></a>

##### client.setFilter(options) ⇒ <code>object</code>
Set filter.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter |
| [options.filterClass] | <code>number</code> | Class filter |
| [options.filterType] | <code>number</code> | Type filter |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID filter |
| [options.maskPriority] | <code>number</code> | Priority mask |
| [options.maskClass] | <code>number</code> | Class mask |
| [options.maskType] | <code>number</code> | Type mask |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID mask |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_clearQueue"></a>

##### client.clearQueue([options]) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| [options] | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Callback, which is called for successful request. |
| [options.onError] | <code>function</code> | Callback, which is called for failed request. |

<a id="vscp_dot_rest_dot_Client_and_createVar"></a>

##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_rest_dot_Client_and_readVar"></a>

##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_writeVar"></a>

##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_removeVar"></a>

##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_rest_dot_Client_and_listVar"></a>

##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_rest_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.listLong | <code>boolean</code> | When false the variable list dos not include value and note. If set to true value and note is included. |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_service"></a>

### vscp.service : <code>object</code>
VSCP service supporting functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.service](#vscp_dot_service) : <code>object</code>
    * [.Container](#vscp_dot_service_dot_Container)
        * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
        * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
        * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
        * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
        * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
        * [.create(options)](#vscp_dot_service_dot_Container_and_create)
        * [.write(options)](#vscp_dot_service_dot_Container_and_write)
        * [.read(options)](#vscp_dot_service_dot_Container_and_read)
    * [.timeout](#vscp_dot_service_dot_timeout) : <code>number</code>
    * [.whoIsThere(options)](#vscp_dot_service_dot_whoIsThere)
    * [.scan(options)](#vscp_dot_service_dot_scan)

<a id="vscp_dot_service_dot_Container"></a>

#### service.Container
**Kind**: static class of [<code>service</code>](#vscp_dot_service)  

* [.Container](#vscp_dot_service_dot_Container)
    * [new vscp.service.Container(options)](#new_vscp_dot_service_dot_Container_new)
    * [.client](#vscp_dot_service_dot_Container_and_client) : [<code>Client</code>](#vscp_dot_ws_dot_Client)
    * [.name](#vscp_dot_service_dot_Container_and_name) : <code>string</code>
    * [.data](#vscp_dot_service_dot_Container_and_data) : <code>Array.&lt;object&gt;</code>
    * [.separator](#vscp_dot_service_dot_Container_and_separator) : <code>Array.&lt;object&gt;</code>
    * [.create(options)](#vscp_dot_service_dot_Container_and_create)
    * [.write(options)](#vscp_dot_service_dot_Container_and_write)
    * [.read(options)](#vscp_dot_service_dot_Container_and_read)

<a id="new_vscp_dot_service_dot_Container_new"></a>

##### new vscp.service.Container(options)
The container is used to store javascript objects in a daemon variable as string.It supports one or more objects in a single variable!


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.name | <code>string</code> | Container name |

<a id="vscp_dot_service_dot_Container_and_client"></a>

##### container.client : [<code>Client</code>](#vscp_dot_ws_dot_Client)
VSCP websocket client

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_name"></a>

##### container.name : <code>string</code>
Complete container name (prefix + user defined name)

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_data"></a>

##### container.data : <code>Array.&lt;object&gt;</code>
Data container itself

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_separator"></a>

##### container.separator : <code>Array.&lt;object&gt;</code>
Data element separator

**Kind**: instance property of [<code>Container</code>](#vscp_dot_service_dot_Container)  
<a id="vscp_dot_service_dot_Container_and_create"></a>

##### container.create(options)
Create a container at the daemon.

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_Container_and_write"></a>

##### container.write(options)
Write the container to a daemon variable.The container must exist at the daemon!

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_Container_and_read"></a>

##### container.read(options)
Read the container from the daemon variable.

**Kind**: instance method of [<code>Container</code>](#vscp_dot_service_dot_Container)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_timeout"></a>

#### service.timeout : <code>number</code>
VSCP response timeout in ms

**Kind**: static constant of [<code>service</code>](#vscp_dot_service)  
<a id="vscp_dot_service_dot_whoIsThere"></a>

#### service.whoIsThere(options)
Request a response from all nodes on the communication bus and returnstheir GUID and MDF URL.

**Kind**: static method of [<code>service</code>](#vscp_dot_service)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_service_dot_scan"></a>

#### service.scan(options)
Scan for nodes.

**Kind**: static method of [<code>service</code>](#vscp_dot_service)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.begin | <code>number</code> | Node id where to start scanning |
| options.end | <code>number</code> | Node id where to stop scanning |
| options.onSuccess | <code>function</code> | Callback which is called on successful operation |
| [options.onError] | <code>function</code> | Callback which is called on failed operation |

<a id="vscp_dot_widget"></a>

### vscp.widget : <code>object</code>
VSCP widgets

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.widget](#vscp_dot_widget) : <code>object</code>
    * [.Button](#vscp_dot_widget_dot_Button)
        * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
        * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
        * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)
    * [.Thermometer](#vscp_dot_widget_dot_Thermometer)
        * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
        * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
        * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)
    * [.generateUUID()](#vscp_dot_widget_dot_generateUUID) ⇒ <code>string</code>
    * [.Image(options)](#vscp_dot_widget_dot_Image)

<a id="vscp_dot_widget_dot_Button"></a>

#### widget.Button
**Kind**: static class of [<code>widget</code>](#vscp_dot_widget)  

* [.Button](#vscp_dot_widget_dot_Button)
    * [new vscp.widget.Button(options)](#new_vscp_dot_widget_dot_Button_new)
    * [.draw()](#vscp_dot_widget_dot_Button_and_draw)
    * [.setEnabled(value)](#vscp_dot_widget_dot_Button_and_setEnabled)

<a id="new_vscp_dot_widget_dot_Button_new"></a>

##### new vscp.widget.Button(options)
A button widget.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.offImageUrl | <code>number</code> | URL to button which is in off state |
| options.onImageUrl | <code>number</code> | URL to button which is in on state |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |
| [options.scale] | <code>number</code> | Scale factor applied to the button image (default: 1.0) |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client, used for event communication |
| [options.bindToRemoteState] | <code>boolean</code> | Bind the button state to the remote state or not (default: false) |
| [options.receiveZone] | <code>number</code> | Zone where state events will come from (default: 255) |
| [options.receiveSubZone] | <code>number</code> | Sub-zone where state events will come from (default: 255) |
| [options.transmitZone] | <code>number</code> | Zone where button event will be sent to (default: 255) |
| [options.transmitSubZone] | <code>number</code> | Sub-zone where button event will be sent to (default: 255) |
| [options.index] | <code>number</code> | Button index (instance number)  (default: 0) |
| [options.enable] | <code>boolean</code> | Enable or disable button  (default: false) |

<a id="vscp_dot_widget_dot_Button_and_draw"></a>

##### button.draw()
Draw the button depended on its current state.

**Kind**: instance method of [<code>Button</code>](#vscp_dot_widget_dot_Button)  
<a id="vscp_dot_widget_dot_Button_and_setEnabled"></a>

##### button.setEnabled(value)
Enable or disable the button.

**Kind**: instance method of [<code>Button</code>](#vscp_dot_widget_dot_Button)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>boolean</code> | Enable (true) or disable (false) it |

<a id="vscp_dot_widget_dot_Thermometer"></a>

#### widget.Thermometer
**Kind**: static class of [<code>widget</code>](#vscp_dot_widget)  

* [.Thermometer](#vscp_dot_widget_dot_Thermometer)
    * [new vscp.widget.Thermometer(options)](#new_vscp_dot_widget_dot_Thermometer_new)
    * [.draw()](#vscp_dot_widget_dot_Thermometer_and_draw)
    * [.setEnabled(value)](#vscp_dot_widget_dot_Thermometer_and_setEnabled)

<a id="new_vscp_dot_widget_dot_Thermometer_new"></a>

##### new vscp.widget.Thermometer(options)
A thermometer widget.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.imageUrl | <code>number</code> | URL to thermometer image |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |
| options.data | <code>object</code> | Thermometer data |
| options.data.maxT | <code>number</code> | Max. temperature in degree celsius |
| options.data.minT | <code>number</code> | Min. temperature in degree celsius |
| options.data.x | <code>number</code> | x position of the lower left begin of the thermometer column in image |
| options.data.y | <code>number</code> | y position of the lower left begin of the thermometer column in image |
| options.data.height | <code>number</code> | Thermometer column height (only between numbers) |
| options.data.width | <code>number</code> | Thermometer column width |
| options.data.yOffset | <code>number</code> | Thermometer column height offset from the begin to the first number |
| options.data.color | <code>string</code> | HTML color, e.g. '#8A0000' |
| [options.scale] | <code>number</code> | Scale factor applied to the thermometer image (default: 1.0) |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client, used for event communication |
| [options.receiveZone] | <code>number</code> | Zone where state events will come from (default: 255) |
| [options.receiveSubZone] | <code>number</code> | Sub-zone where state events will come from (default: 255) |
| [options.sensorIndex] | <code>number</code> | Sensor index (default: 0) |
| [options.vscpClass] | <code>number</code> | VSCP measurement class (default: CLASS1.MEASUREMENT) |
| [options.vscpType] | <code>number</code> | VSCP measurement type (default: CLASS1.MEASUREMENT.TERMPERATURE) |
| [options.enable] | <code>boolean</code> | Enable or disable thermometer (default: true) |

<a id="vscp_dot_widget_dot_Thermometer_and_draw"></a>

##### thermometer.draw()
Draw the thermometer depended on its current state.

**Kind**: instance method of [<code>Thermometer</code>](#vscp_dot_widget_dot_Thermometer)  
<a id="vscp_dot_widget_dot_Thermometer_and_setEnabled"></a>

##### thermometer.setEnabled(value)
Enable or disable the thermometer.

**Kind**: instance method of [<code>Thermometer</code>](#vscp_dot_widget_dot_Thermometer)  

| Param | Type | Description |
| --- | --- | --- |
| value | <code>boolean</code> | Enable (true) or disable (false) it |

<a id="vscp_dot_widget_dot_generateUUID"></a>

#### widget.generateUUID() ⇒ <code>string</code>
Generate a UUID.

**Kind**: static method of [<code>widget</code>](#vscp_dot_widget)  
**Returns**: <code>string</code> - UUID  
<a id="vscp_dot_widget_dot_Image"></a>

#### widget.Image(options)
Add a image to the canvas.

**Kind**: static method of [<code>widget</code>](#vscp_dot_widget)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.canvasName | <code>string</code> | Name of the canvas, normally the canvas id |
| options.url | <code>string</code> | Path to the image |
| options.x | <code>number</code> | x position of the image in the canvas |
| options.y | <code>number</code> | y position of the image in the canvas |

<a id="vscp_dot_wizard"></a>

### vscp.wizard : <code>object</code>
VSCP wizard functionality based on a MDF

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.wizard](#vscp_dot_wizard) : <code>object</code>
    * [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
        * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
        * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
        * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
        * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
        * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
        * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
        * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
        * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)
    * [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
        * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
        * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
        * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
        * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
        * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
        * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)
    * [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
        * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
        * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
        * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
        * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
        * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)
    * [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
        * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
        * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
        * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
        * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
        * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)
    * [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
        * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
        * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
        * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
        * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
        * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)
    * [.Recipe](#vscp_dot_wizard_dot_Recipe)
        * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
        * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
        * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
        * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
        * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
        * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
        * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
        * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
        * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
        * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
        * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)
    * [.getRecipes(options)](#vscp_dot_wizard_dot_getRecipes) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)

<a id="vscp_dot_wizard_dot_MessageBox"></a>

#### wizard.MessageBox
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.MessageBox](#vscp_dot_wizard_dot_MessageBox)
    * [new vscp.wizard.MessageBox(options)](#new_vscp_dot_wizard_dot_MessageBox_new)
    * [.func](#vscp_dot_wizard_dot_MessageBox_and_func) : <code>string</code>
    * [.head](#vscp_dot_wizard_dot_MessageBox_and_head) : <code>string</code>
    * [.description](#vscp_dot_wizard_dot_MessageBox_and_description) : <code>string</code>
    * [.variableType](#vscp_dot_wizard_dot_MessageBox_and_variableType) : <code>string</code>
    * [.variableName](#vscp_dot_wizard_dot_MessageBox_and_variableName) : <code>string</code>
    * [.variableValue](#vscp_dot_wizard_dot_MessageBox_and_variableValue) : <code>string</code>
    * [.parse($messageBox)](#vscp_dot_wizard_dot_MessageBox_and_parse)

<a id="new_vscp_dot_wizard_dot_MessageBox_new"></a>

##### new vscp.wizard.MessageBox(options)
A message box.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.messageBox | <code>object</code> | Messagebox as jquery xml object |

<a id="vscp_dot_wizard_dot_MessageBox_and_func"></a>

##### messageBox.func : <code>string</code>
Function input or output

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_head"></a>

##### messageBox.head : <code>string</code>
Head

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_description"></a>

##### messageBox.description : <code>string</code>
Description

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableType"></a>

##### messageBox.variableType : <code>string</code>
Variable type

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableName"></a>

##### messageBox.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_variableValue"></a>

##### messageBox.variableValue : <code>string</code>
Variable value

**Kind**: instance property of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  
<a id="vscp_dot_wizard_dot_MessageBox_and_parse"></a>

##### messageBox.parse($messageBox)
Parse a messagebox object.

**Kind**: instance method of [<code>MessageBox</code>](#vscp_dot_wizard_dot_MessageBox)  

| Param | Type | Description |
| --- | --- | --- |
| $messageBox | <code>object</code> | Messagebox as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInReg"></a>

#### wizard.WriteBitInReg
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteBitInReg](#vscp_dot_wizard_dot_WriteBitInReg)
    * [new vscp.wizard.WriteBitInReg(options)](#new_vscp_dot_wizard_dot_WriteBitInReg_new)
    * [.pos](#vscp_dot_wizard_dot_WriteBitInReg_and_pos) : <code>number</code>
    * [.page](#vscp_dot_wizard_dot_WriteBitInReg_and_page) : <code>number</code>
    * [.offset](#vscp_dot_wizard_dot_WriteBitInReg_and_offset) : <code>number</code>
    * [.width](#vscp_dot_wizard_dot_WriteBitInReg_and_width) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteBitInReg_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteBitInReg_and_variableName) : <code>string</code>
    * [.parse(writeBitInReg)](#vscp_dot_wizard_dot_WriteBitInReg_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteBitInReg_new"></a>

##### new vscp.wizard.WriteBitInReg(options)
Bit in register access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeBitInReg | <code>object</code> | write-bit-in-reg as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInReg_and_pos"></a>

##### writeBitInReg.pos : <code>number</code>
Bit position

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_page"></a>

##### writeBitInReg.page : <code>number</code>
Register page

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_offset"></a>

##### writeBitInReg.offset : <code>number</code>
Register offset

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_width"></a>

##### writeBitInReg.width : <code>number</code>
Bit width

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_value"></a>

##### writeBitInReg.value : <code>number</code>
Value of bit width

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_variableName"></a>

##### writeBitInReg.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  
<a id="vscp_dot_wizard_dot_WriteBitInReg_and_parse"></a>

##### writeBitInReg.parse(writeBitInReg)
Parse a bit in register access method object.

**Kind**: instance method of [<code>WriteBitInReg</code>](#vscp_dot_wizard_dot_WriteBitInReg)  

| Param | Type | Description |
| --- | --- | --- |
| writeBitInReg | <code>object</code> | write-bit-in-reg as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInAbstraction"></a>

#### wizard.WriteBitInAbstraction
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteBitInAbstraction](#vscp_dot_wizard_dot_WriteBitInAbstraction)
    * [new vscp.wizard.WriteBitInAbstraction(options)](#new_vscp_dot_wizard_dot_WriteBitInAbstraction_new)
    * [.id](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_id) : <code>string</code>
    * [.pos](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos) : <code>number</code>
    * [.width](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_width) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName) : <code>string</code>
    * [.parse($writeBitInAbstraction)](#vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteBitInAbstraction_new"></a>

##### new vscp.wizard.WriteBitInAbstraction(options)
Bit in abstraction access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeBitInAbstraction | <code>object</code> | write-bit-in-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_id"></a>

##### writeBitInAbstraction.id : <code>string</code>
Abstract value id

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_pos"></a>

##### writeBitInAbstraction.pos : <code>number</code>
Bit position

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_width"></a>

##### writeBitInAbstraction.width : <code>number</code>
Bit width

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_value"></a>

##### writeBitInAbstraction.value : <code>number</code>
Value of bit width

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_variableName"></a>

##### writeBitInAbstraction.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  
<a id="vscp_dot_wizard_dot_WriteBitInAbstraction_and_parse"></a>

##### writeBitInAbstraction.parse($writeBitInAbstraction)
Parse a bit in abstraction access method object.

**Kind**: instance method of [<code>WriteBitInAbstraction</code>](#vscp_dot_wizard_dot_WriteBitInAbstraction)  

| Param | Type | Description |
| --- | --- | --- |
| $writeBitInAbstraction | <code>object</code> | write-bit-in-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteRegister"></a>

#### wizard.WriteRegister
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteRegister](#vscp_dot_wizard_dot_WriteRegister)
    * [new vscp.wizard.WriteRegister(options)](#new_vscp_dot_wizard_dot_WriteRegister_new)
    * [.page](#vscp_dot_wizard_dot_WriteRegister_and_page) : <code>number</code>
    * [.offset](#vscp_dot_wizard_dot_WriteRegister_and_offset) : <code>number</code>
    * [.value](#vscp_dot_wizard_dot_WriteRegister_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteRegister_and_variableName) : <code>string</code>
    * [.parse($writeRegister)](#vscp_dot_wizard_dot_WriteRegister_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteRegister_new"></a>

##### new vscp.wizard.WriteRegister(options)
Register access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeRegister | <code>object</code> | write-register as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteRegister_and_page"></a>

##### writeRegister.page : <code>number</code>
Register page

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_offset"></a>

##### writeRegister.offset : <code>number</code>
Register offset

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_value"></a>

##### writeRegister.value : <code>number</code>
Register value

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_variableName"></a>

##### writeRegister.variableName : <code>string</code>
Variable name

**Kind**: instance property of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  
<a id="vscp_dot_wizard_dot_WriteRegister_and_parse"></a>

##### writeRegister.parse($writeRegister)
Parse a register access method object.

**Kind**: instance method of [<code>WriteRegister</code>](#vscp_dot_wizard_dot_WriteRegister)  

| Param | Type | Description |
| --- | --- | --- |
| $writeRegister | <code>object</code> | write-register as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteAbstraction"></a>

#### wizard.WriteAbstraction
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.WriteAbstraction](#vscp_dot_wizard_dot_WriteAbstraction)
    * [new vscp.wizard.WriteAbstraction(options)](#new_vscp_dot_wizard_dot_WriteAbstraction_new)
    * [.id](#vscp_dot_wizard_dot_WriteAbstraction_and_id) : <code>string</code>
    * [.value](#vscp_dot_wizard_dot_WriteAbstraction_and_value) : <code>number</code>
    * [.variableName](#vscp_dot_wizard_dot_WriteAbstraction_and_variableName) : <code>number</code>
    * [.parse($writeAbstraction)](#vscp_dot_wizard_dot_WriteAbstraction_and_parse)

<a id="new_vscp_dot_wizard_dot_WriteAbstraction_new"></a>

##### new vscp.wizard.WriteAbstraction(options)
Abstraction access method.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.writeAbstraction | <code>object</code> | write-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_WriteAbstraction_and_id"></a>

##### writeAbstraction.id : <code>string</code>
Abstract value id

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_value"></a>

##### writeAbstraction.value : <code>number</code>
Abstract value

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_variableName"></a>

##### writeAbstraction.variableName : <code>number</code>
Variable name

**Kind**: instance property of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  
<a id="vscp_dot_wizard_dot_WriteAbstraction_and_parse"></a>

##### writeAbstraction.parse($writeAbstraction)
Parse a abstraction access method object.

**Kind**: instance method of [<code>WriteAbstraction</code>](#vscp_dot_wizard_dot_WriteAbstraction)  

| Param | Type | Description |
| --- | --- | --- |
| $writeAbstraction | <code>object</code> | write-abstraction as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe"></a>

#### wizard.Recipe
**Kind**: static class of [<code>wizard</code>](#vscp_dot_wizard)  

* [.Recipe](#vscp_dot_wizard_dot_Recipe)
    * [new vscp.wizard.Recipe(options)](#new_vscp_dot_wizard_dot_Recipe_new)
    * [.name](#vscp_dot_wizard_dot_Recipe_and_name) : <code>string</code>
    * [.description](#vscp_dot_wizard_dot_Recipe_and_description) : <code>string</code>
    * [.writeBitInRegs](#vscp_dot_wizard_dot_Recipe_and_writeBitInRegs) : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
    * [.writeBitInAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions) : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
    * [.writeRegisters](#vscp_dot_wizard_dot_Recipe_and_writeRegisters) : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
    * [.writeAbstractions](#vscp_dot_wizard_dot_Recipe_and_writeAbstractions) : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
    * [.messageBoxes](#vscp_dot_wizard_dot_Recipe_and_messageBoxes) : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
    * [.mdf](#vscp_dot_wizard_dot_Recipe_and_mdf) : <code>object</code>
    * [.parse($recipe)](#vscp_dot_wizard_dot_Recipe_and_parse)
    * [.write(options)](#vscp_dot_wizard_dot_Recipe_and_write)

<a id="new_vscp_dot_wizard_dot_Recipe_new"></a>

##### new vscp.wizard.Recipe(options)
A recipe.


| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.recipe | <code>object</code> | Recipe as jquery xml object |
| options.mdf | <code>object</code> | MDF as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe_and_name"></a>

##### recipe.name : <code>string</code>
Recipe name

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_description"></a>

##### recipe.description : <code>string</code>
Recipe description

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeBitInRegs"></a>

##### recipe.writeBitInRegs : [<code>Array.&lt;WriteBitInReg&gt;</code>](#vscp_dot_wizard_dot_WriteBitInReg)
Bit access methods in registers

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeBitInAbstractions"></a>

##### recipe.writeBitInAbstractions : <code>Array.&lt;vscp.wizard.WriteBitAbstractions&gt;</code>
Bit access methods in abstract value

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeRegisters"></a>

##### recipe.writeRegisters : [<code>Array.&lt;WriteRegister&gt;</code>](#vscp_dot_wizard_dot_WriteRegister)
Register access methods

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_writeAbstractions"></a>

##### recipe.writeAbstractions : [<code>Array.&lt;WriteAbstraction&gt;</code>](#vscp_dot_wizard_dot_WriteAbstraction)
Abstract access methods

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_messageBoxes"></a>

##### recipe.messageBoxes : [<code>Array.&lt;MessageBox&gt;</code>](#vscp_dot_wizard_dot_MessageBox)
Messageboxes

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_mdf"></a>

##### recipe.mdf : <code>object</code>
MDF

**Kind**: instance property of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  
<a id="vscp_dot_wizard_dot_Recipe_and_parse"></a>

##### recipe.parse($recipe)
Parse a recipe object.

**Kind**: instance method of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  

| Param | Type | Description |
| --- | --- | --- |
| $recipe | <code>object</code> | Recipe as jquery xml object |

<a id="vscp_dot_wizard_dot_Recipe_and_write"></a>

##### recipe.write(options)
Write a recipe.

**Kind**: instance method of [<code>Recipe</code>](#vscp_dot_wizard_dot_Recipe)  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.client | [<code>Client</code>](#vscp_dot_ws_dot_Client) | VSCP websocket client |
| options.nodeId | <code>number</code> | Node id |

<a id="vscp_dot_wizard_dot_getRecipes"></a>

#### wizard.getRecipes(options) ⇒ [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe)
Get recipes from a MDF in JSON format.

**Kind**: static method of [<code>wizard</code>](#vscp_dot_wizard)  
**Returns**: [<code>Array.&lt;Recipe&gt;</code>](#vscp_dot_wizard_dot_Recipe) - Recipe array  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.mdf | <code>object</code> | The mdf as jquery xml object |

<a id="vscp_dot_ws"></a>

### vscp.ws : <code>object</code>
VSCP websocket api functions

**Kind**: static namespace of [<code>vscp</code>](#vscp)  

* [.ws](#vscp_dot_ws) : <code>object</code>
    * [.Client](#vscp_dot_ws_dot_Client)
        * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
        * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
        * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
        * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
        * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
        * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
        * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
        * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
        * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
        * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
        * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
        * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
        * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
        * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
        * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
        * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
        * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
        * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
        * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
        * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
        * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
        * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
        * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
        * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
        * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
        * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
        * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
        * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
        * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
        * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
        * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
        * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
        * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
        * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
        * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
        * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
        * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
        * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
        * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
        * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
        * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
        * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
        * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
        * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
        * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>

<a id="vscp_dot_ws_dot_Client"></a>

#### ws.Client
**Kind**: static class of [<code>ws</code>](#vscp_dot_ws)  

* [.Client](#vscp_dot_ws_dot_Client)
    * [new vscp.ws.Client()](#new_vscp_dot_ws_dot_Client_new)
    * [.socket](#vscp_dot_ws_dot_Client_and_socket) : <code>object</code>
    * [.url](#vscp_dot_ws_dot_Client_and_url) : <code>string</code>
    * [.userName](#vscp_dot_ws_dot_Client_and_userName) : <code>string</code>
    * [.userId](#vscp_dot_ws_dot_Client_and_userId) : <code>number</code>
    * [.userFullname](#vscp_dot_ws_dot_Client_and_userFullname) : <code>string</code>
    * [.userRights](#vscp_dot_ws_dot_Client_and_userRights) : <code>array</code>
    * [.userRemotes](#vscp_dot_ws_dot_Client_and_userRemotes) : <code>array</code>
    * [.userEvents](#vscp_dot_ws_dot_Client_and_userEvents) : <code>array</code>
    * [.userNote](#vscp_dot_ws_dot_Client_and_userNote) : <code>string</code>
    * [.password](#vscp_dot_ws_dot_Client_and_password) : <code>string</code>
    * [.vscpkey](#vscp_dot_ws_dot_Client_and_vscpkey) : <code>string</code>
    * [.authdomain](#vscp_dot_ws_dot_Client_and_authdomain) : <code>string</code>
    * [.passwordHash](#vscp_dot_ws_dot_Client_and_passwordHash) : <code>string</code>
    * [.onConnError](#vscp_dot_ws_dot_Client_and_onConnError) : <code>function</code>
    * [.onMessage](#vscp_dot_ws_dot_Client_and_onMessage) : <code>function</code>
    * [.onEvent](#vscp_dot_ws_dot_Client_and_onEvent) : <code>Array.&lt;function()&gt;</code>
    * [.onVariable](#vscp_dot_ws_dot_Client_and_onVariable) : <code>function</code>
    * [.onTableRow](#vscp_dot_ws_dot_Client_and_onTableRow) : <code>function</code>
    * [.state](#vscp_dot_ws_dot_Client_and_state) : <code>number</code>
    * [.substate](#vscp_dot_ws_dot_Client_and_substate) : <code>number</code>
    * [.states](#vscp_dot_ws_dot_Client_and_states) : <code>enum</code>
    * [.substates](#vscp_dot_ws_dot_Client_and_substates) : <code>enum</code>
    * [.addEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_addEventListener)
    * [.removeEventListener(eventListener)](#vscp_dot_ws_dot_Client_and_removeEventListener)
    * [.getAuthHash(userName, password, str_iv)](#vscp_dot_ws_dot_Client_and_getAuthHash) ⇒ <code>string</code>
    * [.onWebSocketOpen()](#vscp_dot_ws_dot_Client_and_onWebSocketOpen)
    * [.onWebSocketClose()](#vscp_dot_ws_dot_Client_and_onWebSocketClose)
    * [.onWebSocketMessage(msg)](#vscp_dot_ws_dot_Client_and_onWebSocketMessage)
    * [.connect(options)](#vscp_dot_ws_dot_Client_and_connect) ⇒ <code>object</code>
    * [.disconnect(options)](#vscp_dot_ws_dot_Client_and_disconnect) ⇒ <code>object</code>
    * [.start(options)](#vscp_dot_ws_dot_Client_and_start) ⇒ <code>object</code>
    * [.stop(options)](#vscp_dot_ws_dot_Client_and_stop) ⇒ <code>object</code>
    * [.clearQueue(options)](#vscp_dot_ws_dot_Client_and_clearQueue) ⇒ <code>object</code>
    * [.sendEvent(options)](#vscp_dot_ws_dot_Client_and_sendEvent) ⇒ <code>object</code>
    * [.setFilter(options)](#vscp_dot_ws_dot_Client_and_setFilter) ⇒ <code>object</code>
    * [.createVar(options)](#vscp_dot_ws_dot_Client_and_createVar) ⇒ <code>object</code>
    * [.readVar(options)](#vscp_dot_ws_dot_Client_and_readVar) ⇒ <code>object</code>
    * [.writeVar(options)](#vscp_dot_ws_dot_Client_and_writeVar) ⇒ <code>object</code>
    * [.resetVar(options)](#vscp_dot_ws_dot_Client_and_resetVar) ⇒ <code>object</code>
    * [.removeVar(options)](#vscp_dot_ws_dot_Client_and_removeVar) ⇒ <code>object</code>
    * [.lengthVar(options)](#vscp_dot_ws_dot_Client_and_lengthVar) ⇒ <code>object</code>
    * [.lastChangeVar(options)](#vscp_dot_ws_dot_Client_and_lastChangeVar) ⇒ <code>object</code>
    * [.listVar(options)](#vscp_dot_ws_dot_Client_and_listVar) ⇒ <code>object</code>
    * [.readTable(options)](#vscp_dot_ws_dot_Client_and_readTable) ⇒ <code>object</code>

<a id="new_vscp_dot_ws_dot_Client_new"></a>

##### new vscp.ws.Client()
VSCP websocket client, used for connection establishment to a VSCP server.

<a id="vscp_dot_ws_dot_Client_and_socket"></a>

##### client.socket : <code>object</code>
Websocket

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_url"></a>

##### client.url : <code>string</code>
url used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userName"></a>

##### client.userName : <code>string</code>
User name used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userId"></a>

##### client.userId : <code>number</code>
User id from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userFullname"></a>

##### client.userFullname : <code>string</code>
User full name from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userRights"></a>

##### client.userRights : <code>array</code>
User rights from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userRemotes"></a>

##### client.userRemotes : <code>array</code>
User allowed remotes from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userEvents"></a>

##### client.userEvents : <code>array</code>
User allowed events from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_userNote"></a>

##### client.userNote : <code>string</code>
User note from authentication AUTH1

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_password"></a>

##### client.password : <code>string</code>
Password used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_vscpkey"></a>

##### client.vscpkey : <code>string</code>
Secret key used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_authdomain"></a>

##### client.authdomain : <code>string</code>
authdomain used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_passwordHash"></a>

##### client.passwordHash : <code>string</code>
Password hash used for connection establishment

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onConnError"></a>

##### client.onConnError : <code>function</code>
Callback called on any connection error

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onMessage"></a>

##### client.onMessage : <code>function</code>
Callback called on any received VSCP response message

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onEvent"></a>

##### client.onEvent : <code>Array.&lt;function()&gt;</code>
Callbacks called on any received VSCP event message

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onVariable"></a>

##### client.onVariable : <code>function</code>
Callback called on any received variable (see LSTVAR command)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onTableRow"></a>

##### client.onTableRow : <code>function</code>
Callback called on any received table row (see GT command)

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_state"></a>

##### client.state : <code>number</code>
VSCP websocket is not connected right now

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_substate"></a>

##### client.substate : <code>number</code>
VSCP event traffic is closed

**Kind**: instance property of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_states"></a>

##### client.states : <code>enum</code>
States of the VSCP websocket

**Kind**: instance enum of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| DISCONNECTED | <code>number</code> | <code>0</code> | Not connected |
| CONNECTED | <code>number</code> | <code>1</code> | Standard websocket connection established |
| AUTHENTICATED | <code>number</code> | <code>2</code> | Authentication with VSCP server successful |

<a id="vscp_dot_ws_dot_Client_and_substates"></a>

##### client.substates : <code>enum</code>
Substates of the VSCP websocket

**Kind**: instance enum of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Properties**

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| CLOSED | <code>number</code> | <code>0</code> | No events sent from server |
| OPEN | <code>number</code> | <code>1</code> | Events sent from server |

<a id="vscp_dot_ws_dot_Client_and_addEventListener"></a>

##### client.addEventListener(eventListener)
Add a event listener.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp_dot_ws_dot_Client_and_removeEventListener"></a>

##### client.removeEventListener(eventListener)
Remove a event listener.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| eventListener | <code>function</code> | Event listener function |

<a id="vscp_dot_ws_dot_Client_and_getAuthHash"></a>

##### client.getAuthHash(userName, password, str_iv) ⇒ <code>string</code>
Calculates the VSCP server websocket authentication hash.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>string</code> - Authentication ("encrypted user:password")  

| Param | Type | Description |
| --- | --- | --- |
| userName | <code>string</code> | User name |
| password | <code>string</code> | Password |
| str_iv | <code>string</code> | 16 random byte iv in hex form |

<a id="vscp_dot_ws_dot_Client_and_onWebSocketOpen"></a>

##### client.onWebSocketOpen()
This function is called by the websocket in case the connection is established.
It will initiate the authentication with the VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onWebSocketClose"></a>

##### client.onWebSocketClose()
This function is called by the websocket in case that the connection is closed.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
<a id="vscp_dot_ws_dot_Client_and_onWebSocketMessage"></a>

##### client.onWebSocketMessage(msg)
This function is called for any websocket message (VSCP server response message).

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  

| Param | Type | Description |
| --- | --- | --- |
| msg | <code>string</code> | VSCP server response message |

<a id="vscp_dot_ws_dot_Client_and_connect"></a>

##### client.connect(options) ⇒ <code>object</code>
Connect to a VSCP server with the given URL.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_ws_dot_Client_and_disconnect"></a>

##### client.disconnect(options) ⇒ <code>object</code>
Disconnect from a VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful disconnection. |

<a id="vscp_dot_ws_dot_Client_and_start"></a>

##### client.start(options) ⇒ <code>object</code>
Start receiving events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_stop"></a>

##### client.stop(options) ⇒ <code>object</code>
Stop receiving events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_clearQueue"></a>

##### client.clearQueue(options) ⇒ <code>object</code>
Clear the VSCP event queue on the server side.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_sendEvent"></a>

##### client.sendEvent(options) ⇒ <code>object</code>
Send a VSCP event to the VSCP server.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.event | [<code>Event</code>](#vscp_dot_Event) | VSCP event to send |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_setFilter"></a>

##### client.setFilter(options) ⇒ <code>object</code>
Set a filter in the VSCP server for VSCP events.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.filterPriority] | <code>number</code> | Priority filter (default: 0) |
| [options.filterClass] | <code>number</code> | Class filter (default: 0) |
| [options.filterType] | <code>number</code> | Type filter (default: 0) |
| [options.filterGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID filter (default: 0) |
| [options.maskPriority] | <code>number</code> | Priority mask (default: 0) |
| [options.maskClass] | <code>number</code> | Class mask (default: 0xffff) |
| [options.maskType] | <code>number</code> | Type mask (default: 0xffff) |
| [options.maskGuid] | <code>Array.&lt;number&gt;</code> \| <code>string</code> | GUID mask (default: 0) |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_createVar"></a>

##### client.createVar(options) ⇒ <code>object</code>
Create a a VSCP remote variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

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

<a id="vscp_dot_ws_dot_Client_and_readVar"></a>

##### client.readVar(options) ⇒ <code>object</code>
Read a value from a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_writeVar"></a>

##### client.writeVar(options) ⇒ <code>object</code>
Write a value to a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| options.value | <code>string</code> | Variable value |
| options.type | <code>number</code> | Variable type |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_resetVar"></a>

##### client.resetVar(options) ⇒ <code>object</code>
Reset a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_removeVar"></a>

##### client.removeVar(options) ⇒ <code>object</code>
Remove a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_lengthVar"></a>

##### client.lengthVar(options) ⇒ <code>object</code>
Get a VSCP server variable length.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_lastChangeVar"></a>

##### client.lastChangeVar(options) ⇒ <code>object</code>
Get last change of a VSCP server variable.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Variable name |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_listVar"></a>

##### client.listVar(options) ⇒ <code>object</code>
List all VSCP server variables.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| [options.regex] | <code>string</code> | Regular expression to filter variables |
| options.onVariable | <code>function</code> | Function which is called per variable |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_ws_dot_Client_and_readTable"></a>

##### client.readTable(options) ⇒ <code>object</code>
Get data from a table.
If "begin" and "end" are omitted, the whole table is returned.

**Kind**: instance method of [<code>Client</code>](#vscp_dot_ws_dot_Client)  
**Returns**: <code>object</code> - Promise  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Options |
| options.name | <code>string</code> | Table name |
| options.begin | <code>string</code> | Date when to begin ( ISO form YY-MM-DD HH:MM:SS ) |
| options.end | <code>string</code> | Date when to end ( ISO form YY-MM-DD HH:MM:SS ) |
| options.onTableRow | <code>function</code> | Function which is called on every received table row |
| [options.onSuccess] | <code>function</code> | Function which is called on a successful operation |
| [options.onError] | <code>function</code> | Function which is called on a failed operation |

<a id="vscp_dot_getVarTypeName"></a>

### vscp.getVarTypeName(n) ⇒ <code>string</code>
Get variable type name as string by numerical code.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Variable type name  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Numerical code |

<a id="vscp_dot_getVarTypeNumerical"></a>

### vscp.getVarTypeNumerical(str) ⇒ <code>number</code>
Get numerical code of variable type from string.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>number</code> - Variable type numerical code  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Variable type name |

<a id="vscp_dot_getEditorModeFromType"></a>

### vscp.getEditorModeFromType(n) ⇒ <code>string</code>
Get ace editor formation mode string from numerical variable type code.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Ace editro formation mode string  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | Variable type numerical code |

<a id="vscp_dot_b64EncodeUnicode"></a>

### vscp.b64EncodeUnicode(str) ⇒ <code>string</code>
Encode base64 unicode safe.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Base64  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Unicode string |

<a id="vscp_dot_b64DecodeUnicode"></a>

### vscp.b64DecodeUnicode(str) ⇒ <code>string</code>
Decode base64 unicode safe.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Unicode string  

| Param | Type | Description |
| --- | --- | --- |
| str | <code>string</code> | Base64 |

<a id="vscp_dot_isBase64Type"></a>

### vscp.isBase64Type(type) ⇒ <code>bool</code>
Determine whether the given variable type is a type stored base64 encoded or not.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>bool</code> - Stored base64 encoded (true) or not (false).  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |

<a id="vscp_dot_decodeValueIfBase64"></a>

### vscp.decodeValueIfBase64(type, value) ⇒ <code>string</code>
Decode the value if its base64 encoded.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Decoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |

<a id="vscp_dot_encodeValueIfBase64"></a>

### vscp.encodeValueIfBase64(type, value) ⇒ <code>string</code>
Encode the value if its stored in base64.

**Kind**: static method of [<code>vscp</code>](#vscp)  
**Returns**: <code>string</code> - Encoded value if type is base64 encoded type otherwise original value.  

| Param | Type | Description |
| --- | --- | --- |
| type | <code>number</code> | Variable type numerical code |
| value | <code>string</code> | Value |


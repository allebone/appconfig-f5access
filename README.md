# appconfig-f5access
AppConfig PLIST for f5access

## IBM Attribute References

- %email% (Email Address: first.last@us.af.mil)
- %domain% (AD Domain Name)
- %username% (Username: first.last@us.af.mil)
- %upn% (User Principle Name: 123456789123@mil)
- %fullname% (Users Full Name: Bryan Allebone)
- %devicename% (Device Name: OMNI000057685)
- %deviceSerialNumber% (Vendor Serial Number: XXXXXXXXXX)
- %csn% (MDM ID, Vendor + Vendor Serial Number: ApplXXXXXXXXXXX)
- %wifiMacAddress% (Wi-Fi MAC Address: 00:01:02:03:04:05)
- %deviceid% (UDID)

## F5 Access Attribute References

- MdmAssignedid (STRING) -- The internal device ID assigned to the device by the MOM.
- Mdminstanceld (STRING) -- An arbitrary string that identifies particular MD Instance.
- MamDeviceUniqueld (STRING) -- An assigned ID for the device,
- MdmDeviceWMacAddress (STRING) -- The wireless MAC address of the device.
- MamDeviceSerialNumber (STRING) -- An assigned serial number for the device
- 
##F5 Document Comments

session.client.mdm_device_unique_id, session.client.unique_id	This value is provided by an MDM with the MdmDeviceUniqueId or UDID attribute. If both attributes are provided, MdmDeviceUniqueId takes preference. If neither is provided this session variable is not present. If this field is provided by the MDM, both session variables are present. An example value is RC1KQLCJFOJEEM0XIOB3P52OMUQ3UN9Y3SDA5RWR.

session.client.mdm_assigned_id	This value is provided by the MDM in the MdmAssignedId attribute. If this attribute is not provided, the session variable is not present.

session.client.mdm_instance_id	The value is provided by the MDM in the MdmInstanceId attribute. If this attribute is not provided, the session variable is not present.

session.client.mdm_device_wifi_mac_address	The value is provided by the MDM in the MdmDeviceWifiMacAddress or WiFiMAC attribute. If both attributes are provided, MdmDeviceWifiMacAddress takes preference. If neither attribute is provided, the session variable is not present.

session.client.mdm_device_serial_number	The value is provided by the MDM in the MdmDeviceSerialNumber or SerialNumber attribute.If both attributes are provided, MdmDeviceSerialNumber takes preference. If neither attribute is provided, the session variable is not present.

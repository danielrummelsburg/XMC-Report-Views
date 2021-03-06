# Extreme Management (NetSight) FlexViews for EXOS devices

Community Driven repository

## FlexViews
* [Firmware information](tpl/XOS_firmware_Info.tpl?raw=true)
* [Learned MAC to IP](tpl/XOS_Nodealias_MAC-IP_learned.tpl?raw=true)
* [Vlan IP ports](tpl/XOS_VLAN-IP-Port.tpl?raw=true)
* [L3 interface stats](tpl/XOS_L3interface_stats.tpl?raw=true)
* [Link Aggregation](tpl/XOS_sharing.tpl?raw=true)
* [LACP Link Aggregation](tpl/XOS_LACP-sharing.tpl?raw=true)
* [PoE system](tpl/XOS_SystemPoE.tpl?raw=true)
* [PoE port](tpl/XOS_PortPoE.tpl?raw=true)


## Comments & Columns
##### Firmware information
extremeSystemID, extremeImageBooted, sysUpTime, extremeMsmFailoverCause, sysName, extremePrimarySoftwareRev, extremeSecondarySoftwareRev, extremeImageToUseOnReboot, extremeBootROMVersion

##### Learned MAC to IP
extremeFdbIpFdbPortIfIndex, extremeFdbIpFdbIPAddress, extremeFdbIpFdbMacAddress

##### Vlan IP ports
extremeVlanIfVlanId, extremeVlanIfDescr, extremeVlanIpNetAddress, extremeVlanIpNetMask, extremeVlanOpaqueTaggedPorts, extremeVlanOpaqueUntaggedPorts, extremeVlanIfType, extremeVlanIpForwardingState

##### L3 interface stats
extremeStatsPortIfIndex, ifName, extremeStatsVlanNameIndex, extremePortVlanStatsCntrType, extremePortConfigureVlanStatus, extremePortVlanTotalReceivedBytesCounter, extremePortVlanTotalReceivedFramesCounter

##### Link Aggregation
MemberPort_ifName,ifAlias,ifDescr,ifAdminStatus, ifOperStatus, MasterPort_ifName,extremePortLoadshare2Status, extremePortLoadshare2Algorithm

##### LACP Link Aggregation
ifName,ifAlias, ifDescr, ifAdminStatus, ifOperStatus, extremeLacpGroup, extremeLacpMemberPort, extremeLacpAggStatus

##### System PoE
extremePethSystemAdminEnable, extremePethSystemDisconnectPrecedence, extremePethSystemUsageThreshold, extremePethSystemPowerSupplyMode, extremePethSystemLegacyEnable

##### Port PoE - with xos version 22.2.1.5 sometimes the switch does snmp timeout :(
ifName, ifAlias, extremePethPortOperatorLimit, extremePethPortViolationPrecedence, extremePethPortMeasuredPower, extremePethPortReservedBudget


## Examples
* [Link Aggregation](sample/XOS_sharing.png)
* [LACP Link Aggregation](sample/XOS_LACP-sharing.png)
* [PoE system](sample/XOS_SystemPoE.png)
* [PoE port](sample/XOS_PortPoE.png)

## MIBs
All necessary MIBs are included in the Extreme Management Center (NetSight) already.

>Be Extreme
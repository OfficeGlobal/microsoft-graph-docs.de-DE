# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „Windows10EndpointProtectionConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows10EndpointProtectionConfigurations auflisten](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_list.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen der [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)-Objekte auf.|
|[windows10EndpointProtectionConfiguration abrufen](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_get.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Liest die Eigenschaften und Beziehungen des [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)-Objekts auf.|
|[windows10EndpointProtectionConfiguration erstellen](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_create.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Erstellen Sie ein neues [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)-Objekt.|
|[windows10EndpointProtectionConfiguration löschen](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_delete.md)|Keine|Löscht eine [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[windows10EndpointProtectionConfiguration aktualisieren](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_update.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|firewallBlockStatefulFTP|Boolescher Wert|Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Konfiguriert die Leerlaufzeitüberschreitung für Sicherheitszuweisungen in Sekunden, von 300 bis einschließlich 3600. Dies ist der Zeitraum, nach dem Sicherheitszuweisungen ablaufen und gelöscht werden. Gültige Werte: 300 bis 3600.|
|firewallPreSharedKeyEncodingMethod|Zeichenfolge|Wählen Sie die Verschlüsselung des vorinstallierten Schlüssels aus, die verwendet werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolescher Wert|Konfiguriert IPSec-Ausnahmen so, dass IPv6-ICMP-Typcodes für Nachbarsuche zugelassen werden. |
|firewallIPSecExemptionsAllowICMP|Boolescher Wert|Konfiguriert IPSec-Ausnahmen so, dass ICMP zugelassen wird.|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolescher Wert|Konfiguriert IPSec-Ausnahmen so, dass IPv6-ICMP-Typcodes für Routersuche zugelassen werden. |
|firewallIPSecExemptionsAllowDHCP|Boolescher Wert|Konfiguriert IPSec-Ausnahmen so, dass sowohl IPv4- als auch IPv6-DHCP-Datenverkehr zugelassen werden.|
|firewallCertificateRevocationListCheckMethod|Zeichenfolge|Gibt an, wie die Zertifikatsperrliste erzwungen werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolescher Wert|Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weisen Sie das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.|
|firewallPacketQueueingMethod|Zeichenfolge|Konfiguriert, wie das Einfügen des Pakets in die Warteschlange im Tunnelgatewayszenario angewendet werden sollte. Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für private Netzwerke.|
|defenderAttackSurfaceReductionExcludedPaths|Zeichenfolgenauflistung|Liste von EXE-Dateien und -Ordnern, die aus Regeln zur Verringerung der Angriffsfläche ausgeschlossen werden sollen.|
|defenderGuardedFoldersAllowedAppPaths|Zeichenfolgenauflistung|Liste von Pfaden der EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.|
|defenderAdditionalGuardedFolders|Zeichenfolgenauflistung|Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen.|
|defenderExploitProtectionXml|Binär|XML-Inhalte mit Informationen zu Exploit-Schutzdetails.|
|defenderExploitProtectionXmlFileName|Zeichenfolge|Der Name der Datei, aus der DefenderExploitProtectionXml abgerufen wurde.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolescher Wert|Gibt an, ob verhindert werden soll, dass Benutzer Exploit-Schutzeinstellungen überschreiben.|
|appLockerApplicationControl|Zeichenfolge|Ermöglicht, dass der Administrator auswählt, welche App-Typen auf Geräten zulässig sind. Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|smartScreenEnableInShell|Boolescher Wert|Ermöglicht, dass IT-Administratoren SmartScreen für Windows konfigurieren.|
|smartScreenBlockOverrideForFiles|Boolescher Wert|Ermöglicht, dass IT-Administratoren steuern, ob Benutzer SmartScreen-Warnungen ignorieren und bösartige Dateien ausführen können.|
|applicationGuardEnabled|Boolescher Wert|Windows Defender Anwendung Guard aktivieren|
|applicationGuardBlockFileTransfer|Zeichenfolge|Blockiert, dass die Zwischenablage weder Bilddateien noch Textdateien überträgt. Mögliche Werte: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolescher Wert|Blockiert, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.|
|applicationGuardAllowPersistence|Boolescher Wert|Lässt zu, dass vom Benutzer generierte Daten innerhalb des App Guard-Containers (Favoriten, Cookies, Webkennwörter usw.) dauerhaft gespeichert werden.|
|applicationGuardForceAuditing|Boolescher Wert|Erzwingt, dass die Überwachung Windows-Protokolle und-Ereignisse dauerhaft speichert, um Sicherheits-/Compliancekriterien (Beispielereignisse sind Benutzeranmeldung und -abmeldung, Verwendung von Berechtigungen, Softwareinstallation, Systemänderungen usw.) erfüllt werden.|
|applicationGuardBlockClipboardSharing|Zeichenfolge|Blockiert, dass die Zwischenablage Daten von Host zu Container, von Container zu Host, beide Richtungen oder gar keine Richtung freigibt. Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolescher Wert|Lässt das Drucken von Container in PDF zu.|
|applicationGuardAllowPrintToXPS|Boolescher Wert|Lässt das Drucken von Container zu XPS zu.|
|applicationGuardAllowPrintToLocalPrinters|Boolescher Wert|Lässt das Drucken vom Container auf lokalen Druckern zu.|
|applicationGuardAllowPrintToNetworkPrinters|Boolescher Wert|Lässt das Drucken vom Container auf Netzwerkdruckern zu.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolescher Wert|Ermöglicht, dass der Administrator die Eingabeaufforderung bei Warnungen für andere Datenträgerverschlüsselungen auf Benutzercomputern deaktiviert.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolescher Wert|Ermöglicht, dass der Administrator anfordert, dass die Verschlüsselung mithilfe von BitLocker aktiviert wird. Diese Richtlinie gilt nur für eine mobile SKU.|
|bitLockerEncryptDevice|Boolescher Wert|Ermöglicht, dass der Administrator anfordert, dass die Verschlüsselung mithilfe von BitLocker aktiviert wird.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|BitLocker-Richtlinie für Wechseldatenträger.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Zuweisungen|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




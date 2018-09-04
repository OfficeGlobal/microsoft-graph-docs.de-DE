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
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|firewallBlockStatefulFTP|Boolesch|Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600. Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden. Gültige Werte: 300 bis 3600.|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|Wählen Sie den vorinstallierten Schlüssel für die zu verwendende Codierung. Mögliche Werte sind `deviceDefault`, `none` und `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.|
|firewallIPSecExemptionsAllowICMP|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.|
|firewallIPSecExemptionsAllowDHCP|Boolesch|Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|Geben Sie an, wie die Zertifikats-Sperrliste erzwungen werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolesch|Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|Konfiguriert, wie das Paket für die Warteschlange im Szenario mit dem Tunnel-Gateway angewendet werden soll. Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für private Netzwerke.|
|defenderAttackSurfaceReductionExcludedPaths|Collection von Objekten des Typs „String“|Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen.|
|defenderGuardedFoldersAllowedAppPaths|Collection von Objekten des Typs „String“|Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen.|
|defenderAdditionalGuardedFolders|Collection von Objekten des Typs „String“|Liste von Ordnerpfaden, die der Liste geschützter Ordner hinzugefügt werden sollen.|
|defenderExploitProtectionXml|Binär|XML-Inhalte mit Details zum Exploit-Schutz.|
|defenderExploitProtectionXmlFileName|Zeichenfolge|Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde.|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolesch|Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps. Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|smartScreenEnableInShell|Boolesch|Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.|
|smartScreenBlockOverrideForFiles|Boolesch|Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.|
|applicationGuardEnabled|Boolesch|Aktiviert Windows Defender Application Guard.|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|Sperren der Zwischenablage für die Übertragung von Bild- oder Textdaten oder beiden. Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolesch|Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.|
|applicationGuardAllowPersistence|Boolesch|Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).|
|applicationGuardForceAuditing|Boolesch|Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung. Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolesch|Erlaubt das Drucken im PDF-Format aus dem Container.|
|applicationGuardAllowPrintToXPS|Boolesch|Erlaubt das Drucken im XPS-Format aus dem Container.|
|applicationGuardAllowPrintToLocalPrinters|Boolesch|Erlaubt das Drucken auf lokalen Druckern aus dem Container.|
|applicationGuardAllowPrintToNetworkPrinters|Boolesch|Erlaubt das Drucken auf Netzwerkdruckern aus dem Container.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolesch|Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolesch|Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern. Diese Richtlinie gilt nur für Mobilgeräte-SKUs.|
|bitLockerEncryptDevice|Boolesch|Ermöglicht es dem Administrator, eine Aktivierung der Verschlüsselung mittels BitLocker anzufordern.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|BitLocker-Richtlinie für Wechseldatenträger.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Aufgaben|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}-->
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




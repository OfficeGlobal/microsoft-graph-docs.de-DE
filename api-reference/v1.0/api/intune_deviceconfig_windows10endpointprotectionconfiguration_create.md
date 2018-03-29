# <a name="create-windows10endpointprotectionconfiguration"></a>Erstellen von „windows10EndpointProtectionConfiguration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode erstellt ein neues Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EndpointProtectionConfiguration“ an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EndpointProtectionConfiguration“ erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|firewallBlockStatefulFTP|Boolean|Blockiert statusbehaftete FTP-Verbindungen mit dem Gerät.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Konfiguriert das Leerlauftimeout für Sicherheitszuordnungen in Sekunden, von 300 bis einschließlich 3600. Dies ist der Zeitraum, nach dem Sicherheitszuordnungen ablaufen und gelöscht werden. Gültige Werte: 300 bis 3600.|
|firewallPreSharedKeyEncodingMethod|String|Diese Eigenschaft legt die Codierung des vorinstallierten Schlüssels fest. Mögliche Werte sind: `deviceDefault`, `none` und `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Nachbarsuche zulässig sind.|
|firewallIPSecExemptionsAllowICMP|Boolean|Konfiguriert IPSec-Ausnahmen, sodass ICMP zulässig ist.|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|Konfiguriert IPSec-Ausnahmen, sodass IPv6-ICMP-Codes für die Routersuche zulässig sind.|
|firewallIPSecExemptionsAllowDHCP|Boolean|Konfiguriert IPSec-Ausnahmen, sodass sowohl IPv4-basierter als auch IPv6-basierter DHC-Datenverkehr zulässig ist.|
|firewallCertificateRevocationListCheckMethod|String|Gibt an, wie die Zertifikatssperrliste erzwungen werden soll. Mögliche Werte sind: `deviceDefault`, `none`, `attempt` und `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Wenn ein Authentifizierungssatz nicht vollständig von einem Schlüsselerstellungsmodul unterstützt wird, weist diese Einstellung das Modul an, nur nicht unterstützte Authentifizierungssuites zu ignorieren und nicht den gesamten Satz.|
|firewallPacketQueueingMethod|String|Konfiguriert, wie Paketwarteschlangen im Tunnelgatewayszenario implementiert werden sollen. Mögliche Werte sind: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound` und `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für Domänennetzwerke.|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für öffentliche Netzwerke.|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Konfiguriert die Firewallprofileinstellungen für private Netzwerke.|
|defenderAttackSurfaceReductionExcludedPaths|Collection von Objekten des Typs „String“|Liste von EXE-Dateien und Ordnern, die von Regeln zur Verringerung der Angriffsfläche ausgenommen werden sollen|
|defenderGuardedFoldersAllowedAppPaths|Collection von Objekten des Typs „String“|Liste von Pfaden zu EXE-Dateien, die auf geschützte Ordner zugreifen dürfen|
|defenderAdditionalGuardedFolders|Collection von Objekten des Typs „String“|Liste von Ordnerpfaden, die der Liste der geschützter Ordner hinzugefügt werden sollen|
|defenderExploitProtectionXml|Binary|XML-Inhalte mit Details zum Exploit-Schutz|
|defenderExploitProtectionXmlFileName|String|Name der Datei, aus der „DefenderExploitProtectionXml“ abgerufen wurde|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|Gibt an, ob verhindert werden soll, dass Benutzer die Einstellungen für den Exploit-Schutz überschreiben.|
|appLockerApplicationControl|String|Ermöglicht dem Administrator die Festlegung der auf Geräten zulässigen Typen von Apps. Mögliche Werte sind: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker` und `auditComponentsStoreAppsAndSmartlocker`.|
|smartScreenEnableInShell|Boolean|Ermöglicht IT-Administratoren die Konfiguration von SmartScreen für Windows.|
|smartScreenBlockOverrideForFiles|Boolean|Ermöglicht es IT-Administratoren, zu steuern, ob Benutzer SmartScreen-Warnungen ignorieren und Schaddateien ausführen dürfen.|
|applicationGuardEnabled|Boolean|Aktiviert Windows Defender Application Guard.|
|applicationGuardBlockFileTransfer|String|Blockiert die Übertragung von Bilddateien oder Textdateien oder beiden Dateitypen durch die Zwischenablage. Mögliche Werte sind: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone` und `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Boolean|Unterbindet, dass Unternehmenswebsites unternehmensfremde Inhalte laden, z. B. Plug-Ins von Drittanbietern.|
|applicationGuardAllowPersistence|Boolean|Erlaubt die dauerhafte Speicherung benutzergenerierter Daten im App Guard Container (Favoriten, Cookies, Webkennwörter usw.).|
|applicationGuardForceAuditing|Boolean|Erzwingt die dauerhafte Speicherung von Windows-Protokollen und -Ereignissen durch die Überwachung zwecks Erfüllung von Sicherheits- und Compliancevorgaben (Beispielereignisse sind Benutzeranmeldungen und -abmeldungen, die Verwendung von Berechtigungen, die Installation von Software und Änderungen am System).|
|applicationGuardBlockClipboardSharing|String|Blockiert die Freigabe von Zwischenablagedaten zwischen Host und Container, zwischen Container und Host, in beide Richtungen oder in keine Richtung. Mögliche Werte sind: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost` und `blockNone`.|
|applicationGuardAllowPrintToPDF|Boolean|Erlaubt das Drucken im PDF-Format über Container.|
|applicationGuardAllowPrintToXPS|Boolean|Erlaubt das Drucken im XPS-Format über Container.|
|applicationGuardAllowPrintToLocalPrinters|Boolean|Erlaubt das Drucken mit lokalen Druckern über Container.|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|Erlaubt das Drucken mit Netzwerkdruckern über Container.|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|Ermöglicht es dem Administrator, den Warnhinweis bezüglich anderer Festplattenverschlüsselungslösungen auf Benutzer-PCs zu deaktivieren.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert. Diese Richtlinie gilt nur für Mobilgeräte-SKUs.|
|bitLockerEncryptDevice|Boolean|Ermöglicht, dass der Administrator die Aktivierung der Verschlüsselung mittels BitLocker fordert.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|BitLocker-Richtlinie für Wechseldatenträger|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4309

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
    "firewallEnabled": "blocked",
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
    "firewallEnabled": "blocked",
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
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
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
    "firewallEnabled": "blocked",
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
    "firewallEnabled": "blocked",
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
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




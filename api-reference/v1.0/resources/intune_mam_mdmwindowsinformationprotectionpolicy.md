Ressourcentyp dmWindowsInformationProtectionPolicy

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Ressource repräsentiert eine Windows Information Protection-Richtlinie zur Verwendung mit einer MDM-Lösung.  

Sie erbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mdmWindowsInformationProtectionPolicy“](../api/intune_mam_mdmwindowsinformationprotectionpolicy_list.md)|Sammlung von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) auf.|
|[Abrufen von „mdmWindowsInformationProtectionPolicy“](../api/intune_mam_mdmwindowsinformationprotectionpolicy_get.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Erstellen von „mdmWindowsInformationProtectionPolicy“](../api/intune_mam_mdmwindowsinformationprotectionpolicy_create.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Erstellt neue Objekte des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Löschen von „mdmWindowsInformationProtectionPolicy“](../api/intune_mam_mdmwindowsinformationprotectionpolicy_delete.md)|Keiner|Löscht Objekte des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Aktualisieren von „mdmWindowsInformationProtectionPolicy“](../api/intune_mam_mdmwindowsinformationprotectionpolicy_update.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|WIP-Erzwingungsstufe. Siehe die Enumerations-Definition für unterstützte Werte. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Mögliche Werte: sind `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.|
|enterpriseDomain|Zeichenfolge|Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProtectedDomainNames|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectionUnderLockConfigRequired|Boolesch|Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann. Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|revokeOnUnenrollDisabled|Boolesch|Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird. Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien. Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|rightsManagementServicesTemplateId|GUID|GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID. Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|azureRightsManagementServicesAllowed|Boolesch|Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|iconsVisible|Boolesch|Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden. Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectedApps|Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptApps|Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt. Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseNetworkDomainNames|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren. Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)-Sammlung|Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen. Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten. Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80). Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)-Sammlung|Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren. Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt. Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRangesAreAuthoritative|Boolesch|Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden. Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServers|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist eine Liste von Proxyservern. Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseInternalProxyServers|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver. Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“. Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert. Sie gelten als Adressen im Unternehmensnetzwerk. Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServersAreAuthoritative|Boolesch|Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden. Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|neutralDomainResources|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|indexingEncryptedStoresOrItemsBlocked|Boolesch|Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|smbAutoEncryptedFileExtensions|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|isAssigned|Boolesch|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Sammlung|Eine weitere Möglichkeit zur Eingabe geschützter Apps über XML-Dateien. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)-Sammlung|Eine weitere Möglichkeit zur Eingabe ausgenommener Apps über XML-Dateien. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|Aufgaben|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste der Sicherheitsgruppen, für die die Richtlinie gilt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy"
}-->
``` json
{
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)",

"Warning: /api-reference/v1.0/resources/intune_mam_mdmwindowsinformationprotectionpolicy.md:
      Paragraph text found before a valid header: dmWindowsInformation...",

"Warning: /api-reference/v1.0/resources/intune_mam_mdmwindowsinformationprotectionpolicy.md:
      Paragraph text found before a valid header: Policy for Windows i...",

"Warning: /api-reference/v1.0/resources/intune_mam_mdmwindowsinformationprotectionpolicy.md:
      Paragraph text found before a valid header: Inherits from [windo...",

"Warning: /api-reference/v1.0/resources/intune_mam_managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"

  ],
}
-->




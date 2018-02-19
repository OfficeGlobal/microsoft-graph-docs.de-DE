# <a name="windowsinformationprotectionpolicy-resource-type"></a>Ressourcentyp „windowsInformationProtectionPolicy“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Ressource repräsentiert eine Windows Information Protection-Richtlinie zur Verwendung ohne MDM-Lösung.

Sie erbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windowsInformationProtectionPolicy“](../api/intune_mam_windowsinformationprotectionpolicy_list.md)|Sammlung von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) auf.|
|[Abrufen von „windowsInformationProtectionPolicy“](../api/intune_mam_windowsinformationprotectionpolicy_get.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Erstellen von „windowsInformationProtectionPolicy“](../api/intune_mam_windowsinformationprotectionpolicy_create.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Erstellt neue Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Löschen von „windowsInformationProtectionPolicy“](../api/intune_mam_windowsinformationprotectionpolicy_delete.md)|Keiner|Löscht Objekte des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Aktualisieren von „windowsInformationProtectionPolicy“](../api/intune_mam_windowsinformationprotectionpolicy_update.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|String|Beschreibung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|String|Schlüssel der Entität. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|version|String|Version der Entität. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|enforcementLevel|String|WIP-Erzwingungsstufe. Die unterstützten Werte finden Sie in der Enum-Definition. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Mögliche Werte sind: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt` und `encryptAuditAndBlock`.|
|enterpriseDomain|String|Primäre Unternehmensdomäne. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProtectedDomainNames|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Liste der zu schützenden Unternehmensdomänen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectionUnderLockConfigRequired|Boolean|Gibt an, ob die Funktion „Protection under Lock“ (auch als „Encrypt under PIN“ bezeichnet) konfiguriert werden muss. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|Gibt ein Wiederherstellungszertifikat an, das zur Wiederherstellung von Daten in verschlüsselten Dateien verwendet werden kann. Dieses Zertifikat ist identisch mit dem DRA-Zertifikat (Data Recovery Agent, Datenwiederherstellungs-Agent) für EFS (Encrypting File System, verschlüsselndes Dateisystem). Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|revokeOnUnenrollDisabled|Boolean|Diese Richtlinie steuert, ob die WIP-Schlüssel widerrufen werden, wenn für ein Gerät die Registrierung im Verwaltungsdienst aufgehoben wird. Ist diese Eigenschaft auf „1“ gesetzt (Schlüssel nicht widerrufen), werden die Schlüssel nicht widerrufen, und der Benutzer hat auch nach der Aufhebung der Registrierung weiterhin Zugriff auf geschützte Dateien. Wenn die Schlüssel nicht widerrufen werden, wird später auch keine Bereinigung von widerrufenen Dateien durchgeführt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|rightsManagementServicesTemplateId|Guid|GUID der für die RMS-Verschlüsselung zu verwendenden Vorlagen-ID. Mithilfe der RMS-Vorlage kann der IT-Administrator konfigurieren, wer Zugriff auf RMS-geschützte Dateien hat und wie lange diese Zugriffsrechte gültig sind. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|azureRightsManagementServicesAllowed|Boolean|Gibt an, ob die Azure RMS-Verschlüsselung für WIP erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|iconsVisible|Boolean|Legt fest, ob Overlays zu den Symbolen WIP-geschützter Dateien im Explorer und zu den Kacheln unternehmensexklusiver Apps im Startmenü hinzugefügt werden. Ab Windows 10 Version 1703 konfiguriert diese Einstellung auch die Sichtbarkeit des WIP-Symbols in der Titelleiste WIP-geschützter Apps. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectedApps|Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Geschützte Anwendungen können auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden durch Verschlüsselung geschützt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptApps|Sammlung von Objekten des Typs [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Von der Richtlinie ausgenommene Apps können ebenfalls auf Unternehmensdaten zugreifen. Die von diesen Anwendungen verarbeiteten Daten werden jedoch nicht geschützt. Das liegt daran, dass einige geschäftskritische Unternehmensanwendungen möglicherweise Kompatibilitätsprobleme mit verschlüsselten Daten haben. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseNetworkDomainNames|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist die Liste der Domänen, die die Grenzen des Unternehmens definieren. Daten, die aus einer dieser Domänen an ein Gerät gesendet werden, gelten als Unternehmensdaten und werden geschützt. Diese Adressen werden als sicheres Ziel für die Übermittlung von Unternehmensdaten betrachtet. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxiedDomains|Sammlung von Objekten des Typs [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)|Enthält eine Liste aller in der Cloud gehosteten Enterprise-Ressourcen-Domänen, die geschützt werden müssen. Verbindungen zu diesen Ressourcen gelten als Unternehmensdaten. Ist ein Proxy mit einer Cloudressource gekoppelt, wird Datenverkehr zu dieser Cloudressource über das Unternehmensnetzwerk weitergeleitet, und zwar über den angegebenen Proxyserver (auf Port 80). Für einen zu diesem Zweck verwendeten Proxyserver muss auch eine Richtlinie des Typs „enterpriseInternalProxyServers“ konfiguriert sein. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRanges|Sammlung von Objekten des Typs [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)|Legt die Unternehmens-IP-Bereiche fest, die die Computer im Unternehmensnetzwerk definieren. Daten, die von diesen Computern gesendet werden, gelten als Teil des Unternehmens und werden geschützt. Diese Adressen gelten als sichere Ziel für die Übermittlung von Unternehmensdaten. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRangesAreAuthoritative|Boolean|Boolescher Wert, der den Client anweist, die konfigurierte Liste zu akzeptieren und nicht zu versuchen, mittels Heuristik andere Subnetze zu finden. Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServers|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist eine Liste von Proxyservern. Alle Server, die nicht in dieser Liste aufgeführt sind, gelten nicht als Unternehmensserver. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseInternalProxyServers|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Dies ist die durch Trennzeichen getrennte Liste der internen Proxyserver. Beispiel: „157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59“. Diese Proxys wurden vom Administrator für Verbindungen zu bestimmten Ressourcen im Internet konfiguriert. Sie gelten als Adressen im Unternehmensnetzwerk. Die Proxys werden nur verwendet, um Richtlinien des Typs „enterpriseProxiedDomains“ so zu konfigurieren, dass Datenverkehr zu den betreffenden Domänen zwingend über diese Proxys weitergeleitet wird. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServersAreAuthoritative|Boolean|Boolescher Wert, der den Client anweist, die konfigurierte Proxyliste zu akzeptieren und nicht zu versuchen, andere Arbeitsproxys zu finden. Der Standardwert ist „false“. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|neutralDomainResources|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Liste der Domänennamen, die als Arbeitsressource oder als Privatressource verwendet werden dürfen. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|indexingEncryptedStoresOrItemsBlocked|Boolean|Dieser Schalter ist für den Windows Search-Indexer gedacht. Er steuert, ob die Indizierung von Elementen erlaubt ist. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|smbAutoEncryptedFileExtensions|Sammlung von Objekten des Typs [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Definiert eine Liste von Dateierweiterungen. Dateien mit diesen Erweiterungen werden verschlüsselt, wenn sie von einer SMB-Freigabe innerhalb der Unternehmensgrenzen kopiert werden. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|isAssigned|Boolean|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|revokeOnMdmHandoffDisabled|Boolean|Neue Eigenschaft in RS2. Dokumentation noch ausstehend.|
|mdmEnrollmentUrl|String|URL zur Registrierung in der MDM-Lösung|
|windowsHelloForBusinessBlocked|Boolean|Boolescher Wert, der Windows Hello for Business als Methode für die Anmeldung bei Windows festlegt|
|pinMinimumLength|Int32|Ganze Zahl, die festlegt, wie viele Zeichen die PIN mindestens haben muss. Der Standardwert ist „4“. Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 4. Die größte Zahl, die Sie konfigurieren können, muss kleiner sein als die Zahl, die Sie für die Richtlinieneinstellung zur Festlegung der PIN-Maximallänge angegeben haben, oder kleiner als 127 (je nachdem, welche Zahl kleiner ist).|
|pinUppercaseLetters|String|Ganzzahlwert, der konfiguriert, ob Großbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen. Der Standardwert lautet „NotAllow“. Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.|
|pinLowercaseLetters|String|Ganzzahlwert, der konfiguriert, ob Kleinbuchstaben in der Windows Hello for Business-PIN verwendet werden dürfen. Der Standardwert lautet „NotAllow“. Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.|
|pinSpecialCharacters|String|Ganzzahlwert, der konfiguriert, ob Sonderzeichen in der Windows Hello for Business-PIN verwendet werden dürfen. Zu den zulässigen Sonderzeichen für Windows Hello for Business-Gesten gehören: ! " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~. Der Standardwert lautet „NotAllow“. Mögliche Werte sind: `notAllow`, `requireAtLeastOne` und `allow`.|
|pinExpirationDays|Int32|Ganzzahlwert, der angibt, wie viele Tage die PIN verwendet werden darf, bevor das System den Benutzer auffordert, sie zu ändern. Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 730. Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0. Wenn Sie für diese Richtlinie „0“ festlegen, läuft die PIN des Benutzers niemals ab. Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt. Der Standardwert lautet „0“.|
|numberOfPastPinsRemembered|Int32|Ganzzahlwert, der angibt, wie viele der zuletzt dem Benutzerkonto zugeordneten PINs nicht wiederverwendet werden dürfen. Die größte Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 50. Die kleinste Zahl, die Sie als Wert für diese Richtlinieneinstellung konfigurieren können, ist 0. Wenn Sie für diese Richtlinie „0“ festlegen, wird keine Speicherung früherer PINs erzwungen. Dieser Knoten wurde in Windows 10 Version 1511 hinzugefügt. Der Standardwert lautet „0“.|
|passwordMaximumAttemptCount|Int32|Legt fest, wie oft die Authentifizierung fehlschlagen darf, bevor das Gerät zurückgesetzt wird. Ein Wert von „0“ deaktiviert die Funktion zur Gerätezurücksetzung. Gültig sind Ganzzahlen X, wobei gilt 4 <= X <= 16 für Desktops und 0 <= X <= 999 für Mobilgeräte.|
|minutesOfInactivityBeforeDeviceLock|Int32|Gibt an, wie viele Minuten sich das Gerät maximal im Leerlauf befinden darf, bevor eine PIN- oder Kennwortsperre aktiviert wird.   Gültig sind Ganzzahlen X, wobei gilt 0 <= X <= 999.|
|daysWithoutContactBeforeUnenroll|Int32|Offline-Intervall (in Tagen), nach dem die App-Daten gelöscht werden |

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|protectedAppLockerFiles|Sammlung von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Eine weitere Möglichkeit, geschützte Apps per XML-Datei anzugeben. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptAppLockerFiles|Sammlung von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Eine weitere Möglichkeit, von der Richtlinie ausgenommene Apps per XML-Datei anzugeben. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|assignments|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste der Sicherheitsgruppen, für die die Richtlinie gilt. Geerbt von [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
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
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```




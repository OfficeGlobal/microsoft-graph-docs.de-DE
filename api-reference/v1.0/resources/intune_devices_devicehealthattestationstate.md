# <a name="devicehealthattestationstate-resource-type"></a>Ressourcentyp „deviceHealthAttestationState“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastUpdateDateTime|String|Zeitstempel der letzten Aktualisierung|
|contentNamespaceUrl|String|Version des DHA-Berichts (Version des Namespace)|
|deviceHealthAttestationStatus|String|Version des DHA-Berichts (Version des Namespace)|
|contentVersion|String|Version des Integritätsnachweisstatus-Schemas|
|issuedDateTime|DateTimeOffset|Datum und Uhrzeit der Evaluierung des Geräts durch eine MDM-Lösung bzw. der Registrierung des Geräts in einer MDM-Lösung|
|attestationIdentityKey|String|Ist auf einem Gerät ein AIK (Attestation Identity Key) vorhanden, bedeutet das, dass das Gerät über ein EK-Zertifikat (Endorsement Key-Zertifikat) verfügt.|
|resetCount|Int64|Häufigkeit, mit der ein PC-Gerät in den Ruhezustand gewechselt bzw. den Betrieb fortgesetzt hat|
|restartCount|Int64|Häufigkeit, mit der ein PC-Gerät neu gestartet wurde|
|dataExcutionPolicy|String|Eine DEP-Richtlinie definiert eine Reihe von Hardware- und Softwaretechnologien, die zusätzliche Arbeitsspeicherprüfungen durchführen. |
|bitLockerStatus|String|Aktiviert oder deaktiviert die BitLocker-Laufwerkverschlüsselung.|
|bootManagerVersion|String|Version des Start-Managers|
|codeIntegrityCheckVersion|String|Version des Start-Managers|
|secureBoot|String|Ist „secureBoot“ aktiviert, müssen die Hauptkomponenten über die korrekten Kryptografiesignaturen verfügen.|
|bootDebugging|String|Ist „bootDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.|
|operatingSystemKernelDebugging|String|Ist „operatingSystemKernelDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.|
|codeIntegrity|String| Ist „codeIntegrity“ aktiviert, wird ausschließlich Code ausgeführt, dessen Integrität verifiziert wurde.|
|testSigning|String|Ist „testSigning“ aktiviert, wird vom Gerät während des Starts keine Signaturprüfung erzwungen.|
|safeMode|String|Der abgesicherte Modus ist eine Option zur Problembehandlung unter Windows. Sie startet den Computer in einen eingeschränkten Zustand.|
|windowsPE|String|Betriebssystem mit eingeschränkten Diensten, das den Computer für Windows vorbereitet|
|earlyLaunchAntiMalwareDriverProtection|String|ELAM schützt die Computer in Ihrem Netzwerk, während sie starten.|
|virtualSecureMode|String|VSM ist ein Container, der bei Kernelkompromittierung wichtige Komponenten schützt.|
|pcrHashAlgorithm|String|Informationsattribut, das den Hashalgorithmus angibt, der vom TPM verwendet wurde|
|bootAppSecurityVersion|String|Sicherheitsversionsnummer der Startanwendung|
|bootManagerSecurityVersion|String|Sicherheitsversionsnummer der Startanwendung|
|tpmVersion|String|Sicherheitsversionsnummer der Startanwendung|
|pcr0|String|Kennzahl, die in PCR\[0\] erfasst ist|
|secureBootConfigurationPolicyFingerPrint|String|Fingerabdruck der benutzerdefinierten Richtlinie für die Konfiguration der Option „Sicherer Start“|
|codeIntegrityPolicy|String|Die Codeintegritätsrichtlinie, die die Sicherheit der Startumgebung steuert|
|bootRevisionListInfo|String|Die Startüberarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde|
|operatingSystemRevListInfo|String|Die Betriebssystem-Überarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde|
|healthStatusMismatchInfo|String|Dieses Attribut wird angezeigt, wenn der DHA-Dienst ein Integritätsproblem erkennt.|
|healthAttestationSupportedStatus|String|Dieses Attribut gibt an, ob das Gerät DHA unterstützt.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```




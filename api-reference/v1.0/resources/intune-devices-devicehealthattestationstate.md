---
title: Ressourcentyp „deviceHealthAttestationState“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256147"
---
# <a name="devicehealthattestationstate-resource-type"></a>Ressourcentyp „deviceHealthAttestationState“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastUpdateDateTime|Zeichenfolge|Zeitstempel der letzten Aktualisierung|
|contentNamespaceUrl|Zeichenfolge|Version des DHA-Berichts (Version des Namespace)|
|deviceHealthAttestationStatus|Zeichenfolge|Version des DHA-Berichts (Version des Namespace)|
|contentVersion|Zeichenfolge|Version des Integritätsnachweisstatus-Schemas|
|issuedDateTime|DateTimeOffset|Datum und Uhrzeit der Evaluierung des Geräts durch eine MDM-Lösung bzw. der Registrierung des Geräts in einer MDM-Lösung|
|attestationIdentityKey|Zeichenfolge|Ist auf einem Gerät ein AIK (Attestation Identity Key) vorhanden, bedeutet das, dass das Gerät über ein EK-Zertifikat (Endorsement Key-Zertifikat) verfügt.|
|resetCount|Int64|Häufigkeit, mit der ein PC-Gerät in den Ruhezustand gewechselt bzw. den Betrieb fortgesetzt hat|
|restartCount|Int64|Häufigkeit, mit der ein PC-Gerät neu gestartet wurde|
|dataExcutionPolicy|Zeichenfolge|Eine DEP-Richtlinie definiert eine Reihe von Hardware- und Softwaretechnologien, die zusätzliche Arbeitsspeicherprüfungen durchführen. |
|bitLockerStatus|Zeichenfolge|Aktiviert oder deaktiviert die BitLocker-Laufwerkverschlüsselung.|
|bootManagerVersion|Zeichenfolge|Version des Start-Managers|
|codeIntegrityCheckVersion|Zeichenfolge|Version des Start-Managers|
|secureBoot|Zeichenfolge|Ist „secureBoot“ aktiviert, müssen die Hauptkomponenten über die korrekten Kryptografiesignaturen verfügen.|
|bootDebugging|Zeichenfolge|Ist „bootDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.|
|operatingSystemKernelDebugging|Zeichenfolge|Ist „operatingSystemKernelDebugging“ aktiviert, wird das Gerät zu Entwicklungs- und Testzwecken verwendet.|
|codeIntegrity|Zeichenfolge| Ist „codeIntegrity“ aktiviert, wird ausschließlich Code ausgeführt, dessen Integrität verifiziert wurde.|
|testSigning|Zeichenfolge|Ist „testSigning“ aktiviert, wird vom Gerät während des Starts keine Signaturprüfung erzwungen.|
|safeMode|Zeichenfolge|Der abgesicherte Modus ist eine Option zur Problembehandlung unter Windows. Sie startet den Computer in einen eingeschränkten Zustand.|
|windowsPE|Zeichenfolge|Betriebssystem mit eingeschränkten Diensten, das den Computer für Windows vorbereitet|
|earlyLaunchAntiMalwareDriverProtection|Zeichenfolge|ELAM schützt die Computer in Ihrem Netzwerk, während sie starten.|
|virtualSecureMode|Zeichenfolge|VSM ist ein Container, der bei Kernelkompromittierung wichtige Komponenten schützt.|
|pcrHashAlgorithm|Zeichenfolge|Informationsattribut, das den Hashalgorithmus angibt, der vom TPM verwendet wurde|
|bootAppSecurityVersion|Zeichenfolge|Sicherheitsversionsnummer der Startanwendung|
|bootManagerSecurityVersion|Zeichenfolge|Sicherheitsversionsnummer der Startanwendung|
|tpmVersion|Zeichenfolge|Sicherheitsversionsnummer der Startanwendung|
|pcr0|Zeichenfolge|Kennzahl, die in PCR\[0\] erfasst ist|
|secureBootConfigurationPolicyFingerPrint|Zeichenfolge|Fingerabdruck der benutzerdefinierten Richtlinie für die Konfiguration der Option „Sicherer Start“|
|codeIntegrityPolicy|Zeichenfolge|Die Codeintegritätsrichtlinie, die die Sicherheit der Startumgebung steuert|
|bootRevisionListInfo|Zeichenfolge|Die Startüberarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde|
|operatingSystemRevListInfo|String|Die Betriebssystem-Überarbeitungsliste, die während des ersten Starts auf einem Gerät mit Integritätsnachweis geladen wurde|
|healthStatusMismatchInfo|Zeichenfolge|Dieses Attribut wird angezeigt, wenn der DHA-Dienst ein Integritätsproblem erkennt.|
|healthAttestationSupportedStatus|String|Dieses Attribut gibt an, ob das Gerät DHA unterstützt.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
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




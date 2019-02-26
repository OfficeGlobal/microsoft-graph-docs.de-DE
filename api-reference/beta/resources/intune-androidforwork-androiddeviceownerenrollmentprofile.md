---
title: Androiddeviceownerenrollmentprofile hinzugefügt-Ressourcentyp
description: Registrierungsprofil zur Registrierung von COSU-Geräten, die Google Cloud Management verwenden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd22f0686a39dbd4531bb4228f5ed1ecca27b6bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164414"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>Androiddeviceownerenrollmentprofile hinzugefügt-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Registrierungsprofil zur Registrierung von COSU-Geräten, die Google Cloud Management verwenden

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidDeviceOwnerEnrollmentProfiles aufListen](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|[androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekte.|
|[Androiddeviceownerenrollmentprofile hinzugefügt abrufen](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Lesen von Eigenschaften und Beziehungen des [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.|
|[Androiddeviceownerenrollmentprofile hinzugefügt erstellen](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Erstellen eines neuen [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.|
|[Androiddeviceownerenrollmentprofile hinzugefügt löschen](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|Keine|Löscht eine [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).|
|[Androiddeviceownerenrollmentprofile hinzugefügt aktualisieren](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Aktualisieren der Eigenschaften eines [androiddeviceownerenrollmentprofile hinzugefügt](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) -Objekts.|
|[Aktion „revokeToken“](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|Keine|Noch nicht dokumentiert|
|[Aktion „createToken“](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|Keiner|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|accountId|Zeichenfolge|Mandanten-GUID, zu der das Registrierungsprofil gehört|
|id|string|Eindeutige GUID des Registrierungsprofils|
|displayName|Zeichenfolge|Anzeigename des Registrierungsprofils|
|description|String|Beschreibung des Registrierungsprofils|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Registrierungsprofils|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Registrierungsprofils|
|tokenValue|Zeichenfolge|Wert des zuletzt für das Registrierungsprofil erstellten Tokens|
|tokenCreationDateTime|DateTimeOffset|Datum der Erstellung des zuletzt erstellten Tokens.|
|tokenExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens|
|enrolledDeviceCount|Int32|Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte|
|qrCodeContent|Zeichenfolge|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





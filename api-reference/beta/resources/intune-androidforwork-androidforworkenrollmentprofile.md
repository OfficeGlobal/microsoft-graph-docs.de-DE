---
title: Ressourcentyp „androidForWorkEnrollmentProfile“
description: Registrierungsprofil zur Registrierung von COSU-Geräten, die Google Cloud Management verwenden
localization_priority: Normal
ms.openlocfilehash: a10e3a153cc21837ab015ab0c08e8c8b6ee0ac9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890972"
---
# <a name="androidforworkenrollmentprofile-resource-type"></a>Ressourcentyp „androidForWorkEnrollmentProfile“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Registrierungsprofil zur Registrierung von COSU-Geräten, die Google Cloud Management verwenden
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „androidForWorkEnrollmentProfile“](../api/intune-androidforwork-androidforworkenrollmentprofile-list.md)|Sammlung von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) auf.|
|[Abrufen von „androidForWorkEnrollmentProfile“](../api/intune-androidforwork-androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Erstellen von „androidForWorkEnrollmentProfile“](../api/intune-androidforwork-androidforworkenrollmentprofile-create.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Erstellt neue Objekte des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Löschen von „androidForWorkEnrollmentProfile“](../api/intune-androidforwork-androidforworkenrollmentprofile-delete.md)|Keiner|Löscht Objekte des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Aktualisieren von „androidForWorkEnrollmentProfile“](../api/intune-androidforwork-androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Aktualisiert die Eigenschaften von Objekten des Typs [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Aktion „revokeToken“](../api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „createToken“](../api/intune-androidforwork-androidforworkenrollmentprofile-createtoken.md)|Keiner|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|accountId|Zeichenfolge|Mandanten-GUID, zu der das Registrierungsprofil gehört|
|id|Zeichenfolge|Eindeutige GUID des Registrierungsprofils|
|displayName|Zeichenfolge|Anzeigename des Registrierungsprofils|
|description|Zeichenfolge|Beschreibung des Registrierungsprofils|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Registrierungsprofils|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Registrierungsprofils|
|tokenValue|Zeichenfolge|Wert des zuletzt für das Registrierungsprofil erstellten Tokens|
|tokenExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs des zuletzt erstellten Tokens|
|enrolledDeviceCount|Int32|Gesamtzahl der mit dem Registrierungsprofil registrierten Android-Geräte|
|qrCodeContent|Zeichenfolge|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
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






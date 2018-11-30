---
title: localizedNotificationMessage-Ressourcentyp
description: Der Textinhalt einer Benachrichtigungsvorlage für das angegebene Gebietsschema.
ms.openlocfilehash: 97cd17a99cf7803819d67051c124d34ab279d805
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019970"
---
# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Der Textinhalt einer Benachrichtigungsvorlage für das angegebene Gebietsschema.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[localizedNotificationMessages auflisten](../api/intune-notification-localizednotificationmessage-list.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekte.|
|[localizedNotificationMessage abrufen](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Lesen von Eigenschaften und Beziehungen des [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.|
|[localizedNotificationMessage erstellen](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.|
|[localizedNotificationMessage löschen](../api/intune-notification-localizednotificationmessage-delete.md)|Keine|Löschen einer [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[localizedNotificationMessage aktualisieren](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Aktualisieren der Eigenschaften eines [LocalizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|Gebietsschema|String|Das Gebietsschema für das diese Nachricht bestimmt ist.|
|Betreff|String|Die Vorlage für den Betreff der Nachricht.|
|messageTemplate|String|Die Vorlage für den Inhalt der Nachricht.|
|isDefault|Boolescher Wert|Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist. Dieser Kennzeichnung kann nur festgelegt werden. Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```




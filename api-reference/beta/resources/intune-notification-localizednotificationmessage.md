---
title: localizedNotificationMessage-Ressourcentyp
description: Der Textinhalt einer Benachrichtigungsvorlage für das angegebene Gebietsschema.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53a33c5d83821ff5131b601bd5687e7d98634c00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825788"
---
# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|Gebietsschema|Zeichenfolge|Das Gebietsschema für das diese Nachricht bestimmt ist.|
|Betreff|Zeichenfolge|Die Vorlage für den Betreff der Nachricht.|
|messageTemplate|Zeichenfolge|Die Vorlage für den Inhalt der Nachricht.|
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






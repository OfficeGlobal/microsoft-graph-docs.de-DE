---
title: localizedNotificationMessage-Ressourcentyp
description: Der Textinhalt einer Benachrichtigungsvorlage für das angegebene Gebietsschema.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec08211781dc5fb1ae499d7a4fd8436660cc4e84
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251496"
---
# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|Gebietsschema|Zeichenfolge|Das Gebietsschema für das diese Nachricht bestimmt ist.|
|Betreff|Zeichenfolge|Die Vorlage für den Betreff der Nachricht.|
|messageTemplate|Zeichenfolge|Die Vorlage für den Inhalt der Nachricht.|
|isDefault|Boolean|Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist. Dieser Kennzeichnung kann nur festgelegt werden. Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.|

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




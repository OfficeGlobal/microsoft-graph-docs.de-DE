---
title: Ressourcentyp „notificationMessageTemplate“
description: " Abschnitt. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen."
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b9f298da4a4f37cde60ddc93402bf6d08d3f4f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912435"
---
# <a name="notificationmessagetemplate-resource-type"></a>Ressourcentyp „notificationMessageTemplate“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Benachrichtigungs-E-Mails sind Nachrichten, die an Endbenutzer gesendet werden, die gegen die vom Administrator definierten Konformitätsrichtlinien verstoßen. Auswählen und konfigurieren können Administratoren die Benachrichtigungen in der Intune-Verwaltungskonsole auf der Seite für die Erstellung von Konformitätsrichtlinien, im Abschnitt „Actions for non-compliance“. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-list.md)|Sammlung von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) auf.|
|[Abrufen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Erstellen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Löschen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-delete.md)|Keiner|Löscht Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Aktualisieren von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Aktualisiert die Eigenschaften von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Aktion „sendTestMessage“](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|Keiner|Sendet eine Testnachricht unter Verwendung des für das Standardgebietsschema festgelegten Objekts des Typs „notificationMessageTemplate“.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Anzeigename für die Benachrichtigungs-E-Mail-Vorlage|
|defaultLocale|Zeichenfolge|Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|Optionen für das Branding der Nachrichtenvorlage. Das Branding wird in der Intune-Verwaltungskonsole definiert. Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|localizedNotificationMessages|Sammlung von Objekten des Typs [localizedNotificationMessages](../resources/intune-notification-localizednotificationmessage.md)|Liste der lokalisierten Nachrichten für die Benachrichtigungs-E-Mail-Vorlage|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```




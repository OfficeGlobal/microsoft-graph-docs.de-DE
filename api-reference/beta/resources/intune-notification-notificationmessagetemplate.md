---
title: Ressourcentyp „notificationMessageTemplate“
description: Benachrichtigungs-E-Mails sind Nachrichten, die an Endbenutzer gesendet werden, die gegen die vom Administrator definierten Konformitätsrichtlinien verstoßen. Auswählen und konfigurieren können Administratoren die Benachrichtigungen in der Intune-Verwaltungskonsole auf der Seite für die Erstellung von Konformitätsrichtlinien, im Abschnitt „Actions for non-compliance“. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 487b536b8e957ff695899ce4b22e11d11088e06f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143372"
---
# <a name="notificationmessagetemplate-resource-type"></a>Ressourcentyp „notificationMessageTemplate“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Benachrichtigungs-E-Mails sind Nachrichten, die an Endbenutzer gesendet werden, die gegen die vom Administrator definierten Konformitätsrichtlinien verstoßen. Auswählen und konfigurieren können Administratoren die Benachrichtigungen in der Intune-Verwaltungskonsole auf der Seite für die Erstellung von Konformitätsrichtlinien, im Abschnitt „Actions for non-compliance“. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-list.md)|Sammlung von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) auf.|
|[Abrufen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Erstellen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Löschen von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-delete.md)|Keine|Löscht Objekte des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Aktualisieren von „notificationMessageTemplate“](../api/intune-notification-notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Aktualisiert die Eigenschaften von Objekten des Typs [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Aktion „sendTestMessage“](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|Keiner|Sendet eine Testnachricht unter Verwendung des für das Standardgebietsschema festgelegten Objekts des Typs „notificationMessageTemplate“.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Anzeigename für die Benachrichtigungs-E-Mail-Vorlage|
|defaultLocale|Zeichenfolge|Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|Optionen für das Branding der Nachrichtenvorlage. Das Branding wird in der Intune-Verwaltungskonsole definiert. Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz.|

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
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





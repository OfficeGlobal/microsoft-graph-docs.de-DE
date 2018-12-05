---
title: Ressourcentyp „notificationMessageTemplate“
description: " Abschnitt. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen."
ms.openlocfilehash: a7d38c1a8952b1d7b8fe170b179b5b6c3bc019a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063448"
---
# <a name="notificationmessagetemplate-resource-type"></a>Ressourcentyp „notificationMessageTemplate“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|id|String|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|String|Anzeigename für die Benachrichtigungs-E-Mail-Vorlage|
|defaultLocale|String|Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|Optionen für das Branding der Nachrichtenvorlage. Das Branding wird in der Intune-Verwaltungskonsole definiert. Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität.|

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





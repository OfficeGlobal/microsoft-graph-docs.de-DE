---
title: schemaExtension-Ressourcentyp (Schemaerweiterungen)
description: 'Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 90acbfb0e7a6b031303ae3286f1a5ed366a2a8c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523855"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>schemaExtension-Ressourcentyp (Schemaerweiterungen)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mithilfe von Schemaerweiterungen können Sie ein Schema definieren, um stark typisierte benutzerdefinierte Daten zu erweitern und einem Ressourcentyp hinzuzufügen. Die benutzerdefinierten Daten werden in der erweiterten Ressource als komplexer Typ angezeigt. 

Schemaerweiterungen werden von den folgenden Ressourcentypen unterstützt:

 - [administrativeUnit](administrativeunit.md)
 - [contact](contact.md)
 - [device](device.md)
 - [event](event.md) in einem Benutzer oder Office 365-Gruppenkalender
 - [post](post.md) einer Office 365-Gruppe
 - [group](group.md)
 - [message](message.md) 
 - [organization](organization.md)
 - [user](user.md)

Im [Beispiel für Schemaerweiterungen](/graph/extensibility-schema-groups) erfahren Sie, wie Sie benutzerdefinierte Daten zu Gruppen hinzufügen.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Create](../api/schemaextension-post-schemaextensions.md) | schemaExtension |Dient zum Erstellen einer Schemaerweiterungsdefinition.|
|[List](../api/schemaextension-list.md) | schemaExtension |Auflisten der Avaialbe SchemaExtension Definitionen und deren Eigenschaften.|
|[Get](../api/schemaextension-get.md) | schemaExtension |Dient zum Lesen der Eigenschaften einer bestimmten schemaExtension-Definition.|
|[Update](../api/schemaextension-update.md) | schemaExtension   |Dient zum Aktualisieren einer schemaExtension-Definition. |
|[Delete](../api/schemaextension-delete.md) | Keine |Dient zum Löschen einer schemaExtension-Definition. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Beschreibung für die Schemaerweiterung.|
|id|String|Der eindeutige Bezeichner für die Schemaerweiterungsdefinition. <br>Sie können einen Wert mit einer von zwei Methoden zuweisen: <ul><li>Verketten Sie den Namen einer Ihrer überprüften Domänen mit einem Namen für die Schemaerweiterung, um eine eindeutige Zeichenfolge in diesem Format zu bilden: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Beispiel: `contoso_mySchema`. </li><li>Geben Sie einen Schemanamen an, und verwenden Sie diesen Schemanamen in Microsoft Graph zum Vervollständigen der **id**-Zuweisung in diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Zum Beispiel: `extkvbmkofy_mySchema`.</li></ul>Diese Eigenschaft kann nach dem Erstellen nicht mehr geändert werden. |
|owner|Zeichenfolge|Die `appId` der Anwendung, die der Besitzer der Schemaerweiterung ist. Diese Eigenschaft kann bei der Erstellung bereitgestellt werden, um den Besitzer anzugeben.  Wird Sie nicht bereitgestellt, wird die `appId` der aufrufenden Anwendung als Besitzer festgelegt. In beiden Fällen muss der angemeldete Benutzer angemeldet der Besitzer der Anwendung sein. Wurde diese Eigenschaft einmal festgelegt, ist sie schreibgeschützt und kann nicht geändert werden.|
|properties|[extensionSchemaProperty](extensionschemaproperty.md)-Sammlung|Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden.|
|status|String|Der Lebenszyklusstatus der Schemaerweiterung. Mögliche Statuswerte sind: **InDevelopment**, **Available** und **Deprecated**. Wird bei der Erstellung automatisch auf **InDevelopment** festgelegt. Unter [Schemaerweiterungen](/graph/extensibility-overview#schema-extensions) finden Sie weitere Informationen zu den möglichen Statusübergängen und Verhaltensweisen.|
|targetTypes|String-Sammlung|Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann. Wählen Sie aus **AdministrativeUnit**, **wenden Sie sich an**, **Gerät**, **Ereignis**, **Gruppe**, **Nachricht**, **Organisation**, **Veröffentlichen**oder **Benutzer**.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schemaextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

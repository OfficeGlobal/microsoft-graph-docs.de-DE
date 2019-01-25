---
title: Ressourcentyp directoryRoleTemplate
description: 'Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle DirectoryRole an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den -Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter RoleTemplateId der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. Hinweis: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526158"
---
# <a name="directoryroletemplate-resource-type"></a>Ressourcentyp directoryRoleTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|directoryRoleTemplate abrufen | [directoryRoleTemplate](directoryroletemplate.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.|
|displayName|String|Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt. |
|id|string|Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine



## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

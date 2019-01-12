---
title: Ressourcentyp directoryRoleTemplate
description: 'Stellt eine Verzeichnis Rollenvorlage dar. Vorlage Rolle Directory gibt die Eigenschaftswerte einer Directory-Rolle (DirectoryRole). Es ist eine zugehörige Verzeichnis Rolle Template-Objekt für jede der Directory Rollen, die in einem Mandanten aktiviert werden können. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Andere Rollen verfügbaren Verzeichnis zu aktivieren, die Sie Senden einer POST-Anforderung an den `/directoryRoles` Endpunkt mit der ID des Directory Rolle die Rolle Directory auf dem basiert angegebenen Vorlage im **RoleTemplateId** -Parameter der Anforderung. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie dann zum Lesen und Zuweisen von Mitgliedern zur Rolle Directory starten. **Hinweis**: Directory Rollenvorlage ist für die Rolle der Benutzer Directory verfügbar gemacht werden. Die Benutzer-Directory-Rolle ist implizit und ist für Directory-Clients nicht sichtbar. Jeder Benutzer in den Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57dec43699ba75c7e936fa02dbdf09df74dd06ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966993"
---
# <a name="directoryroletemplate-resource-type"></a>Ressourcentyp directoryRoleTemplate

Stellt eine Verzeichnisrollenvorlage dar. Eine Verzeichnisrollenvorlage gibt die Eigenschaftswerte einer Verzeichnisrolle [DirectoryRole](directoryrole.md) an. Für jede Verzeichnisrolle, die in einem Mandanten aktiviert werden kann, gibt es eine zugehörige Verzeichnisrollenvorlage. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zur Aktivierung anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung an den `/directoryRoles`-Endpunkt mit der ID der Verzeichnisrollenvorlage, auf der die Verzeichnisrolle basiert, die im Parameter **RoleTemplateId** der Anfrage angegeben ist. Nach dem erfolgreichen Abschluss dieser Anforderung können Sie die Verzeichnisrolle lesen und ihr Mitglieder zuweisen. **Hinweis**: Eine Verzeichnisrollenvorlage wird für die Verzeichnisrolle der Benutzer verfügbar gemacht. Die Benutzer-Verzeichnisrolle ist implizit und für Verzeichnis-Clients nicht sichtbar. Jeder Benutzer im Mandanten wird von der Infrastruktur dieser Rolle zugewiesen. Die Rolle ist bereits aktiviert. Verwenden Sie diese Vorlage nicht.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryRoleTemplate abrufen](../api/directoryroletemplate-get.md) | [directoryRoleTemplate](directoryroletemplate.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRoleTemplate-Objekts.|
|[directoryRoleTemplate auflisten](../api/directoryroletemplate-list.md) | [directoryRoleTemplate-Sammlung](directoryroletemplate.md) |Dient zum Abrufen einer Liste von directoryRoleTemplate-Objekten.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|Zeichenfolge|Die festzulegende Beschreibung für die Verzeichnisrolle. Schreibgeschützt.|
|displayName|Zeichenfolge|Der festzulegende Name für die Verzeichnisrolle. Schreibgeschützt. |
|id|Zeichenfolge|Der eindeutige Bezeichner für die Vorlage. Geerbt von [directoryObject](directoryobject.md). Sie geben die **id** der Verzeichnisrollenvorlage die Eigenschaft **RoleTemplateId** in der POST-Anforderung zum Aktivieren einer [DirectoryRole](directoryrole.md) in einen Mandanten an. Schlüssel, lässt keine Nullwerte zu. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine



## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

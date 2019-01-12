---
title: Ressourcentyp directoryRole
description: Stellt eine Azure AD-Directory-Rolle. Azure Active Directory Directory Rollen sind auch bekannt als *Administratorrollen*. Weitere Informationen zu Rollen Verzeichnis (Administrator) finden Sie unter Zuweisen von Administratorrollen in Azure Active Directory. Mit dem Microsoft Graph können Sie Directory Rollen erteilen sie die Berechtigungen der Zielrolle Benutzer zuweisen. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Zum Aktivieren von anderen verfügbaren Verzeichnis Rollen senden Sie eine POST-Anforderung mit der ID der DirectoryRoleTemplate, auf dem die Rolle Directory basiert. Erbt von directoryObject.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b3379bbbecd86612043dcc3cb8455f5c43ba9cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939546"
---
# <a name="directoryrole-resource-type"></a>Ressourcentyp directoryRole

Stellt eine Azure AD-Directory-Rolle. Azure Active Directory Directory Rollen sind auch bekannt als *Administratorrollen*. Weitere Informationen zu Rollen Verzeichnis (Administrator) finden Sie unter [Zuweisen von Administratorrollen in Azure Active Directory](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Mit dem Microsoft Graph können Sie Directory Rollen erteilen sie die Berechtigungen der Zielrolle Benutzer zuweisen. Um eine Rolle Directory lesen oder deren Member aktualisieren möchten, müssen sie zuerst im Mandanten aktiviert werden. Nur die Administratoren im Unternehmen Directory-Rolle ist standardmäßig aktiviert. Zum Aktivieren von anderen verfügbaren Verzeichnis Rollen senden Sie eine POST-Anforderung mit der ID der [DirectoryRoleTemplate](directoryroletemplate.md) , auf dem die Rolle Directory basiert. Erbt von [directoryObject](directoryobject.md).
Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryrole-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryRole abrufen](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts. |
|[directoryRoles auflisten](../api/directoryrole-list.md) | [directoryRole-Sammlung](directoryrole.md) | Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind. |
|[Mitglied hinzufügen](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.|
|[Mitglieder auflisten](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.|
|[Mitglied entfernen](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.|
|[directoryRole aktivieren](../api/directoryrole-post-directoryroles.md) |[directoryRole](directoryrole.md) | Dient zum Aktivieren einer Verzeichnisrolle.|
|[delta](../api/directoryrole-delta.md)|directoryRole-Sammlung| Rufen Sie inkrementelle Änderungen für Directory Rollen. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|Zeichenfolge|Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt. |
|displayName|Zeichenfolge|Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt. |
|id|Zeichenfolge|Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.|
|roleTemplateId|String| Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|Elemente|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
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
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

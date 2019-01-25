---
title: Ressourcentyp directoryRole
description: Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter Zuweisen von Administratorrollen in Azure AD. Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der directoryRoleTemplate, auf der die Verzeichnisrolle basiert. Erbt von directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521250"
---
# <a name="directoryrole-resource-type"></a>Ressourcentyp directoryRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Azure AD-Verzeichnisrolle dar. Azure AD-Verzeichnisrollen werden auch als *Administratorrollen* bezeichnet. Weitere Informationen zu diesen Verzeichnis-(Administrator)Rollen finden Sie unter [Zuweisen von Administratorrollen in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Mit Microsoft Graph können Sie Benutzer zu Verzeichnisrollen zuweisen, um ihnen Berechtigungen der Zielrolle zuzuweisen. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren sind standardmäßig aktiviert. Zum Aktivieren anderer verfügbarer Verzeichnisrollen senden Sie eine POST-Anforderung mit der ID der [directoryRoleTemplate](directoryroletemplate.md), auf der die Verzeichnisrolle basiert. Erbt von [directoryObject](directoryobject.md).

Standardmäßig werden Directory Rollen Recherchediensts Mandanten geltende sein.  Verzeichnis Rollen (derzeit nur das *Konto ein Benutzeradministrator* und *Helpdesk Admin*) können jedoch auch [administrative Einheiten](administrativeunit.md)zugewiesen werden.

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryrole-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryRole abrufen](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des directoryRole-Objekts.|
|[directoryRoles auflisten](../api/directoryrole-list.md) | [directoryRole-Sammlung](directoryrole.md) | Dient zum Auflisten der Verzeichnisrollen, die im Mandanten aktiviert sind. |
|[Mitglied hinzufügen](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Fügen Sie der Verzeichnisrolle einen Benutzer durch Veröffentlichen in der Mitgliedernavitionseingenschaft hinzu.|
|[Mitglieder auflisten](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Benutzer, die Mitglieder der Verzeichnisrolle sind, aus der Mitgliedernavigationseigenschaft ab.|
|[Mitglied entfernen](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Dient zum Entfernen eines Benutzers aus der Verzeichnisrolle.|
|[Mitglieder der Liste bezogenen-Rolle](../api/directoryrole-list-members.md) |scopedRoleMembership-Sammlung| Die Elemente dieser Rolle Verzeichnis, die [administrative Einheiten](administrativeunit.md)mithilfe der Auflistung der ScopedRoleMembership Ressource zugeordnet werden aufgelistet.|
|[delta](../api/directoryrole-delta.md)|directoryRole-Sammlung| Rufen Sie inkrementelle Änderungen für Directory Rollen. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|description|Zeichenfolge|Die Beschreibung für die Verzeichnisrolle. Schreibgeschützt. |
|displayName|String|Der Anzeigename für die Verzeichnisrolle. Schreibgeschützt. |
|id|Zeichenfolge|Die eindeutige ID für die Verzeichnisrolle. Geerbt von [directoryObject](directoryobject.md). Schlüssel, lässt keine Nullwerte zu, schreibgeschützt.|
|roleTemplateId|String| Die **id** der [directoryRoleTemplate](directoryroletemplate.md), auf der diese Rolle basiert. Die Eigenschaft muss angegeben werden, wenn eine Verzeichnisrolle mit einer POST-Operation in einem Mandanten aktiviert wird. Nach der Aktivierung der Verzeichnisrolle ist die Eigenschaft schreibgeschützt. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md)-Sammlung|Benutzer, die Mitglieder dieser Verzeichnisrolle sind. HTTP-Methoden: GET, POST, DELETE. Schreibgeschützt. Lässt Nullwerte zu.|
|scopedMembers|scopedRoleMembership-Sammlung| Mitglieder dieser Rolle Directory [administrative Einheiten](administrativeunit.md)zugeordnet sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

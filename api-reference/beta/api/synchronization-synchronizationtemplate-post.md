---
title: Erstellen von SynchronisationVorlage
description: Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509889"
---
# <a name="create-synchronizationtemplate"></a>Erstellen von SynchronisationVorlage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     |Directory.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |Nicht unterstützt|
|Anwendung                            |Nicht unterstützt| 

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a>Anforderungsheader

| Name           | Typ    | Beschreibung|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt erstellt werden soll. Die `id`, `applicationId` und `factoryTag` Eigenschaften sind erforderlich. Wenn keine `schema` erfolgt mit der Vorlage Standardschema verknüpft die `factoryTag` Eigenschaft verwendet werden.

### <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.

### <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

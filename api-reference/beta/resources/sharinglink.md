---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 7f0ecdbb498ee75133ec9499027f7cfdc6191327
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480418"
---
# <a name="sharinglink-resource-type"></a>sharingLink-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **sharingLink** -Ressource gruppiert Link bezogene Datenelemente in einer einzelnen Struktur.

Wenn eine [**Permission**](permission.md) -Ressource ein **sharingLink** -Facet ungleich NULL aufweist, stellt die Berechtigung einen Freigabe Link dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilt wurden).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ          | Beschreibung
|:---------------|:--------------|:-------------------------------------
| application    | [Identität][]  | Die App, der der Link zugeordnet ist.
| type           | Zeichenfolge        | Der Typ des erstellten Links.
| scope          | Zeichenfolge        | Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.
| preventsDownload | Boolesch       | Wenn true, kann der Benutzer diesen Link nur verwenden, um das Element im Web anzuzeigen, und kann es nicht verwenden, um den Inhalt des Elements herunterzuladen. Nur für OneDrive for Business und SharePoint.
| webHtml        | Zeichenfolge        | Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.
| webUrl         | String        | Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.

[Identität]: identity.md

### <a name="type-options"></a>Typoptionen

In der folgenden Tabelle sind die möglichen Werte für die **Type** -Eigenschaft definiert.

| Wert    | Funktion     | Beschreibung
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.
| `edit`   | `write`  | Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.
| `embed`  | `read`   | Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann. Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.

### <a name="scope-options"></a>Bereichsoptionen

In der folgenden Tabelle sind die möglichen Werte für die **Scope** -Eigenschaft definiert.

| Wert            | Beschreibung
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Jeder, der über die Verknüpfung verfügt, hat Zugriff, ohne sich anmelden zu müssen. Dies kann Personen außerhalb Ihrer Organisation sein.
| `organization`   | Jeder, der bei Ihrer Organisation (Mandant) angemeldet ist, kann über den Link Zugriff erhalten. Nur in OneDrive for Business und SharePoint verfügbar.
| `existingAccess` | Nur Personen, denen bereits auf andere Weise Zugriff auf das Element gewährt wurde, können über diesen Link auf das Element zugreifen. Nur in OneDrive for Business und SharePoint verfügbar.
| `users`          | Der Link gewährt Zugriff nur auf eine bestimmte Personenliste. Nur in OneDrive for Business und SharePoint verfügbar.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

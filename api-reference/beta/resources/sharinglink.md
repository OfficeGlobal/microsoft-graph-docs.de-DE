---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521453"
---
# <a name="sharinglink-resource-type"></a>SharingLink-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.

Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).

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
| type           | String        | Der Typ des erstellten Links.
| scope          | String        | Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.
| preventsDownload | Boolescher Wert       | Wenn True, klicken Sie dann der Benutzer kann nur dieser Link zum Anzeigen des Elements im Web verwenden, und nicht verwenden, um den Inhalt des Artikels herunterladen. Nur für OneDrive für Unternehmen und SharePoint.
| webHtml        | Zeichenfolge        | Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.
| webUrl         | String        | Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.

[Identity]: identity.md

### <a name="type-options"></a>Typ-Optionen

Die folgende Tabelle zeigt die möglichen Werte für die **Type** -Eigenschaft.

| Wert    | Funktion     | Beschreibung
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.
| `edit`   | `write`  | Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.
| `embed`  | `read`   | Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann. Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.

### <a name="scope-options"></a>Bereichsoptionen

Die folgende Tabelle zeigt die möglichen Werte für die Eigenschaft **Bereich** .

| Wert            | Beschreibung
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Jeder Benutzer mit den Link hat Zugriff, ohne Anmeldung. Dies kann Personen außerhalb Ihrer Organisation enthalten.
| `organization`   | Den Link können alle Benutzer in Ihrer Organisation (Mandant) signiert um Zugriff zu erhalten. Nur in OneDrive für Unternehmen und SharePoint verfügbar.
| `existingAccess` | Nur Personen, die bereits Zugriff auf das Element mit anderen Mitteln gewährt wurde, können das Element mit diesem Link zugreifen. Nur in OneDrive für Unternehmen und SharePoint verfügbar.
| `users`          | Der Link gewährt Zugriff nur für eine bestimmte Liste von Personen. Nur in OneDrive für Unternehmen und SharePoint verfügbar.

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

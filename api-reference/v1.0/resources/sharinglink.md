---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7639dab9f63a948b3e9a849d8d320de60f5a0954
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270489"
---
# <a name="sharinglink-resource-type"></a>SharingLink-Ressourcentyp

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
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ          | Beschreibung
|:------------|:--------------|:-------------------------------------
| Anwendung | [Identität][]  | Die App, der der Link zugeordnet ist.
| Typ        | Zeichenfolge        | Der Typ des erstellten Links.
| Bereich       | Zeichenfolge        | Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.
| webHtml     | Zeichenfolge        | Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.
| webUrl      | Zeichenfolge        | Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.

[Identität]: identity.md

## <a name="type-options"></a>Typ-Optionen

In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:

| Wert   | Funktion    | Beschreibung
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.
| `edit`  | `write` | Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.
| `embed` | `read`  | Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann. Eingebettete Links sind nicht für OneDrive for Business oder SharePoint verfügbar.

## <a name="scope-options"></a>Bereichsoptionen

| Wert          | Beschreibung
|:---------------|:------------------------------------------------------------
| `anonymous`    | Jeder Benutzer mit dem Link hat Zugriff, ohne sich anmelden zu müssen. Hierzu können auch Personen außerhalb Ihrer Organisation zählen.
| `organization` | Alle Benutzer, die in Ihrer Organisation (Mandant) angemeldet sind, können den Link benutzen, um Zugriff zu erhalten. Nur in OneDrivefor Business und SharePoint verfügbar.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->

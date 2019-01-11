---
title: sectionGroup-Ressourcentyp
description: Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.
localization_priority: Normal
ms.openlocfilehash: 9e955d91fa49642100694da66421665a0d67b3da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855426"
---
# <a name="sectiongroup-resource-type"></a>sectionGroup-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Abschnittsgruppe in einem OneNote-Notizbuch. Abschnittsgruppen können Abschnitte und Abschnittsgruppen enthalten.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|id|String|Der eindeutige Bezeichner der Abschnittsgruppe. Schreibgeschützt.|
|lastModifiedBy|[identitySet](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit der letzten Änderung der Abschnittsgruppe. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|displayName|String|Der Name der Abschnittsgruppe.|
|sectionGroupsUrl|String|Die URL für die Navigationseigenschaft `sectionGroups`, die alle Abschnittsgruppen in der Abschnittsgruppe zurückgibt. Schreibgeschützt.|
|sectionsUrl|String|Die URL für die Navigationseigenschaft `sections`, die alle Abschnitte in der Abschnittsgruppe zurückgibt. Schreibgeschützt.|
|self|String|Der Endpunkt, an dem Sie Details zur Abschnittsgruppe abrufen können. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Das Notizbuch, das die Abschnittsgruppe enthält. Schreibgeschützt.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Die Abschnittsgruppe, die die Abschnittsgruppe enthält. Schreibgeschützt.|
|sectionGroups|[SectionGroup](sectiongroup.md)-Sammlung|Die Abschnittsgruppen im Abschnitt. Schreibgeschützt. Lässt Nullwerte zu.|
|Abschnitte|[Section](section.md)-Sammlung|Die Abschnitte in der Abschnittsgruppe. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abschnittsgruppe abrufen](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |Dient zum Lesen der Eigenschaften und Beziehungen der Abschnittsgruppe.|
|[Abschnittsgruppe erstellen](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Dient zum Erstellen einer Abschnittsgruppe durch Veröffentlichung in der sectionGroups-Sammlung in der angegebenen Abschnittsgruppe.|
|[Abschnittsgruppen auflisten](../api/sectiongroup-list-sectiongroups.md) |[SectionGroup](sectiongroup.md)-Sammlung| Dient zum Abrufen der Sammlung von Abschnittsgruppen in der angegebenen Abschnittsgruppe.|
|[Abschnitt erstellen](../api/sectiongroup-post-sections.md) |[Section](section.md)| Dient zum Erstellen eines Abschnitts durch Veröffentlichung in der sections-Sammlung in der angegebenen Abschnittsgruppe.|
|[Abschnitte auflisten](../api/sectiongroup-list-sections.md) |[Section](section.md)-Sammlung| Dient zum Abrufen einer Sammlung von Abschnitten in der angegebenen Abschnittsgruppe.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

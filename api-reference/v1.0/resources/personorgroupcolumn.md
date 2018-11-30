---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018780"
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn-Ressourcentyp

Die **personOrGroupColumn** zu einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname              | Typ    | Beschreibung
|:---------------------------|:--------|:--------------------------------------
| **allowMultipleSelection** | boolean | Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.
| **displayAs**              | string  | Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe. Siehe unten.
| **chooseFromType**         | string  | Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können. Müssen `peopleAndGroups` oder `peopleOnly` sein.

## <a name="displayas-options"></a>DisplayAs-Optionen

| DisplayAs-Wert               | Beschreibung
|:------------------------------|:-----------------------
| **account**                   | Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B. i:0#.f|Mitgliedschaft|jane@contoso.com).
| **department**                | Die Abteilung der Person oder Gruppe.
| **firstName**                 | The person's first name.
| **id**                        | Die ID der Person oder Gruppe im Verzeichnis.
| **lastName**                  | Der Nachname der Person.
| **mobilePhone**               | Die Mobiltelefonnummer der Person.
| **name**                      | Der Name der Person.
| **nameWithPictureAndDetails** | Der Name der Person mit ihrem Bild und zusätzlichen Details.
| **nameWithPresence**          | Standard. Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).
| **office**                    | Die Büronummer der Person.
| **pictureOnly36x36**          | Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.
| **pictureOnly48x48**          | Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.
| **pictureOnly72x72**          | Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.
| **sipAddress**                | Die SIP-Adresse der Person.
| **title**                     | Titel der Person in der Organisation.
| **userName**                  | Die Person oder der Benutzername der Gruppe.
| **workEmail**                 | Die Person oder die E-Mail-Adresse der Gruppe.
| **workPhone**                 | Die Telefonnummer bei der Arbeit der Person.

Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->

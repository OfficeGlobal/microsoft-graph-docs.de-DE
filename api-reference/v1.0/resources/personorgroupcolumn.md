---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 37c324ddb1863e3e589e7d17ea60bd879e50771f
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267556"
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn-Ressourcentyp

Die **personOrGroupColumn** zu einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.

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
| **allowMultipleSelection** | boolesch | Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.
| **displayAs**              | Zeichenfolge  | Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe. Siehe unten.
| **chooseFromType**         | Zeichenfolge  | Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können. Müssen `peopleAndGroups` oder `peopleOnly` sein.

## <a name="displayas-options"></a>DisplayAs-Optionen

| DisplayAs-Wert               | Beschreibung
|:------------------------------|:-----------------------
| **Konto**                   | Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B. i:0#.f|Mitgliedschaft|jane@contoso.com).
| **Abteilung**                | Die Abteilung der Person oder Gruppe.
| **firstName**                 | Der Vorname der Person.
| **ID**                        | Die ID der Person oder Gruppe im Verzeichnis.
| **lastName**                  | Der Nachname der Person.
| **mobilePhone**               | Die Mobiltelefonnummer der Person.
| **Name**                      | Der Name der Person.
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

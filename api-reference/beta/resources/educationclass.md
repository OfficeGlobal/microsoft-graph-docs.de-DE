---
title: educationClass-Ressourcentyp
description: 'Stellt eine Klasse in einer Schule dar. Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID. Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte. Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e02cc4b10e4f1f933921f86735f9b09610cfe818
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800012"
---
# <a name="educationclass-resource-type"></a>educationClass-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Klasse in einer Schule dar. Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID. Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte. Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[EducationClass abrufen](../api/educationclass-get.md) | [educationClass](educationclass.md) |Lesen von Eigenschaften und Beziehungen eines **educationClass**-Objekts.|
|[Mitglied hinzufügen](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „members“.|
|[Mitglieder auflisten](../api/educationclass-list-members.md) |[educationUser](educationuser.md)-Sammlung| Abrufen einer **educationUser**-Objektsammlung.|
|[Kursteilnehmer entfernen](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „members“.|
|[Schulen auflisten](../api/educationclass-list-schools.md) |[educationSchool](educationschool.md)-Sammlung| Abrufen einer **educationSchool**-Objektsammlung.|
|[Lehrer hinzufügen](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „teachers“.|
|[Lehrer auflisten](../api/educationclass-list-teachers.md) |[educationUser](educationuser.md)-Sammlung| Abrufen einer Liste der Lehrer für die Klasse|
|[Lehrer entfernen](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „teachers“.|
|[EducationAssignment erstellen](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| Erstellen Sie eine neue **educationAssignment** durch veröffentlichen in der Assignments-Auflistung.|
|[Zuweisungen auflisten](../api/educationclass-list-assignments.md) |[educationAssignment](../resources/educationassignment.md) -Sammlung| Rufen Sie eine **educationAssignment** -Objektsammlung ab.|
|[Gruppe abrufen](../api/educationclass-get-group.md) |[group](group.md)| Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.|
|[EducationCategory erstellen](../api/educationclass-post-category.md) | [educationCategory](educationCategory.md) | Erstellen Sie eine neue **educationCategory** für diese Klasse.|
|[Kategorien auflisten](../api/educationclass-list-categories.md) | [educationCategory](educationCategory.md) -Sammlung | Rufen Sie eine Liste der **educationCategory** -Objekte ab, die zu dieser Klasse gehören.|
|[Aktualisieren](../api/educationclass-update.md) | [educationClass](educationclass.md)    |Aktualisieren eines **educationClass**-Objekts. |
|[Löschen](../api/educationclass-delete.md) | Keine |Löschen eines **educationClass**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id| Zeichenfolge| Eindeutiger Bezeichner für die Klasse|
|description|Zeichenfolge| Beschreibung der Klasse|
|displayName|String| Der Name der Klasse|
|mailNickname|String| E-Mail-Name zum Senden von E-Mails an alle Mitglieder, wenn diese Option aktiviert ist. |
|createdBy|[identitySet](identityset.md)| Entität, die die Klasse erstellt hat. |
|classCode|String| Von der Schule verwendeter Klassencode zum Identifizieren der Klasse|
|externalId|String| ID der Klasse aus dem Synchronisierungssystem |
|externalName|String|Der Name der Klasse im Synchronisierungssystem|
|externalSource|string| Quelle, aus der diese Klasse erstellt wurde. Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.|
|term|[educationTerm](educationterm.md)|Der Zeitraum für diese Klasse.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|members|[educationUser](../resources/educationuser.md)-Sammlung| Alle Benutzer in der Klasse. Lässt Nullwerte zu.|
|schools|[educationSchool](../resources/educationschool.md)-Sammlung| Alle Schulen, denen dieser Klasse zugeordnet ist. Lässt Nullwerte zu.|
|teachers|[educationUser](../resources/educationuser.md)-Sammlung|  Alle Lehrer in der Klasse. Lässt Nullwerte zu.|
|assignments|[educationAssignment](../resources/educationassignment.md) -Sammlung| Alle dieser Klasse zugeordneten Zuordnungen. Lässt Nullwerte zu.|
|categories|[educationCategory](../resources/educationassignment.md) -Sammlung| Alle Kategorien, die dieser Klasse zugeordnet sind. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

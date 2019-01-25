---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523512"
---
# <a name="educationroot-resource-type"></a>educationRoot-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. Einige Objekte im `/education`-Namespace finden Sie in anderen Bereichen von Microsoft Graph (z. B. [Benutzer](user.md)). Der Education-Namespace bietet ausbildungsspezifische Eigenschaften und Features für diese Objekte.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[EducationClass erstellen](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| Erstellen eines neuen **educationClass**-Objekts durch Bereitstellen in die Klassensammlung.|
|[Klassen auflisten](../api/educationroot-list-classes.md) |[educationClass](educationclass.md)-Sammlung| Abrufen einer **educationClass**-Objektsammlung.|
|[EducationSchool erstellen](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| Erstellen eines neuen **educationSchool**-Objekts durch Bereitstellen in der Sammlung der Schulen.|
|[Schulen auflisten](../api/educationroot-list-schools.md) |[educationSchool](educationschool.md)-Sammlung| Abrufen einer **educationSchool**-Objektsammlung.|
|[EducationUser erstellen](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| Erstellen eines neuen **educationUser**-Objekts durch Bereitstellen in der Benutzersammlung.|
|[Benutzer auflisten](../api/educationroot-list-users.md) |[educationUser](educationuser.md)-Sammlung| Abrufen einer **educationUser**-Objektsammlung.|

## <a name="properties"></a>Eigenschaften
Keine.

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|me|[educationUser](educationuser.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|schools|[educationSchool](educationschool.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|users|[educationUser](educationuser.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

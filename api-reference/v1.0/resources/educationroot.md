---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5b9f17cf82c6839a95f1fd81405aa675e0f4d6ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943200"
---
# <a name="educationroot-resource-type"></a>educationRoot-Ressourcentyp

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

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

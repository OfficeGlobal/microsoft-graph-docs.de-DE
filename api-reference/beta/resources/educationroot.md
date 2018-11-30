---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
ms.openlocfilehash: 01845df878d5e6a4fe01cb29f73d73b6980cfa9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059175"
---
# <a name="educationroot-resource-type"></a>educationRoot-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: educationSchool-Ressourcentyp
description: 'Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2549d8babd000a36f0ff3ccd38541ef3c1b2e466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925819"
---
# <a name="educationschool-resource-type"></a>educationSchool-Ressourcentyp

Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get](../api/educationschool-get.md) | [educationSchool](educationschool.md) |Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.|
|[Klasse hinzufügen](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.|
|[Klassen auflisten](../api/educationschool-list-classes.md) |[educationClass](educationclass.md)-Sammlung| Abrufen der **educationClass**-Objektsammlung.|
|[Klasse entfernen](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.|
|[Benutzer hinzufügen](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.|
|[Benutzer auflisten](../api/educationschool-list-users.md) |[educationUser](educationuser.md)-Sammlung| Abrufen der **educationUser**-Objektsammlung.|
|[Benutzer entfernen](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.|
|[Aktualisieren](../api/educationschool-update.md) | [educationSchool](educationschool.md) |Aktualisieren eines **educationSchool**-Objekts. |
|[Löschen](../api/educationschool-delete.md) | Keine |Löschen eines **educationSchool**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String|GUID dieser Schule|
|displayName| String| Anzeigename der Schule| 
|description| String | Beschreibung der Schule| 
|status| string| Schreibgeschützt. Die möglichen Werte sind: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| educationExternalSource| Schreibgeschützt.  Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| String| Die E-Mail-Adresse des Prinzipals|
|principalName| String | Der Name des Prinzipals|
|externalPrincipalId| String | Die ID des Prinzipals im Synchronisierungssystem |
|highestGrade|String| Höchste unterrichtete Klasse |
|lowestGrade|String| Niedrigste unterrichtete Klasse |
|schoolNumber|String| Schulnummer|
|externalId|String| Die ID der Schule im Synchronisierungssystem |
|phone|String| Die Telefonnummer der Schule |
|fax|String| Die Faxnummer der Schule |
|address|[physicalAddress](physicaladdress.md)| Die Adresse der Schule|
|createdBy|[identitySet](identityset.md)|Entität, die Schule erstellt hat.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md)-Sammlung| In der Schule unterrichtete Klassen. Lässt Nullwerte zu.|
|users|[educationUser](educationuser.md)-Sammlung| Benutzer in der Schule. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

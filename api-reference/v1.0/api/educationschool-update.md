---
title: Educationschool-Eigenschaften aktualisieren
description: Aktualisieren der Eigenschaften eines school-Objekts.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: a0a3ee2ea291cf48224d6dfa6294f0a1e521435c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862279"
---
# <a name="update-educationschool-properties"></a>Educationschool-Eigenschaften aktualisieren

Aktualisieren der Eigenschaften eines school-Objekts.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Nicht unterstützt  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName| String| Anzeigename der Schule| 
|description| String | Beschreibung der Schule| 
|principalEmail| String| Die E-Mail-Adresse des Prinzipals|
|principalName| String | Der Name des Prinzipals|
|externalPrincipalId| String | Die ID des Prinzipals im Synchronisierungssystem |
|highestGrade|String| Höchste unterrichtete Klasse |
|lowestGrade|String| Niedrigste unterrichtete Klasse |
|schoolNumber|String| Schulnummer|
|externalId|String| Die ID der Schule im Synchronisierungssystem |
|phone|String| Die Telefonnummer der Schule |
|fax|String| Die Faxnummer der Schule |
|address|[physicalAddress](../resources/physicaladdress.md)| Die Adresse der Schule|
|createdBy|[identitySet](../resources/identityset.md)|Entität, die Schule erstellt hat.|

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationSchool](../resources/educationschool.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

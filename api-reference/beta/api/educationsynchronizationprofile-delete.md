---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2aaa0d47bcc98c814ad525deb781ac7a7df28d87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512472"
---
# <a name="delete-a-educationsynchronizationprofile"></a>Löschen einer educationSynchronizationProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Löschen eines Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten auf Grundlage des Bezeichners.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen |
|:-----------|:----------|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | EduAdministration.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich.  |
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben, aber kein Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

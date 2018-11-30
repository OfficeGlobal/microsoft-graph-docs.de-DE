---
title: Löschen einer educationSynchronizationProfile
description: Löschen Sie eine Schule Synchronisierung Datenprofil im Mandanten auf Grundlage des Bezeichners.
ms.openlocfilehash: 829b723b48eb9a15750bc9d0e00ba50d432e8ab6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062774"
---
# <a name="delete-a-educationsynchronizationprofile"></a>Löschen einer educationSynchronizationProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|Delegierte (Persönliches Microsoft-Konto|Nicht unterstützt|
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

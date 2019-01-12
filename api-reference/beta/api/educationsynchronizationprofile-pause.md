---
title: Pause-Synchronisierung auf ein educationSynchronizationProfile
description: Halten Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4979ed19c9a01d6a7ff2d43f7f3755d03b4b070c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950683"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a>Pause-Synchronisierung auf ein educationSynchronizationProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Halten Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen |
|:-----------|:----------|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | EduAdministration.ReadWrite |
|Delegierte (Persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a>Antwort

Es ist keine Antworttext.

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```

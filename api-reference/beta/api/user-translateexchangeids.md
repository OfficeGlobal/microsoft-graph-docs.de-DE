---
title: 'Benutzer: TranslateExchangeIds'
description: Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571289"
---
# <a name="user-translateexchangeids"></a>Benutzer: TranslateExchangeIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Übersetzen Sie IDs von Outlook-bezogene Ressourcen zwischen den Formaten.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:----------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | User.ReadBasic, User.Read, User.ReadWrite |
| Anwendung | User.Read.All, User.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a>Anforderungsheader

| Name | Wert |
|:-----|:------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

| Parameter | Typ | Beschreibung |
|:----------|:-----|:------------|
| inputIds | Edm.String-Auflistung | Eine Sammlung von Bezeichnern zu konvertieren. Alle Bezeichner in der Auflistung der gleichen ID Quelltyp benötigen und für Elemente im selben Postfach werden müssen. Maximale Größe dieser Auflistung ist 1000 Zeichenfolgen. |
| sourceIdType | exchangeIdFormat | Die ID-Typ der Bezeichner in der `InputIds` Parameter. |
| targetIdType | exchangeIdFormat | Der angeforderte ID-Typ zu konvertieren. |

### <a name="exchangeidformat-values"></a>ExchangeIdFormat Werte

| Werte | Beschreibung |
|:-------|:------------|
| entryId | Das Format von binären Eintrag ID von MAPI-Clients verwendet wird. |
| ewsId | Das ID-Format wird von Exchange-Webdienste-Clients verwendet. |
| immutableEntryId | Die MAPI-kompatibles unveränderlich ID Binärformat. |
| restId | Das ID-Standardformat, von Microsoft Graph verwendet. |
| restImmutableEntryId | Unveränderlich ID Format wird von Microsoft Graph. |

Die binären Dateiformate (`entryId` und `immutableEntryId`) base64-codierte URL-sichere sind. URL-Safeness wird durch Ändern der base64-Codierung binäre Daten auf folgende Weise implementiert:

- Ersetzen Sie `+` mit`-`
- Ersetzen Sie `/` mit`_`
- Entfernen Sie alle nachfolgenden Füllzeichen (`=`)
- Eine ganze Zahl an das Ende der Zeichenfolge, die angibt, wie viele Füllzeichen aus der ursprünglichen Datei hinzufügen (`0`, `1`, oder `2`)

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine [ConvertIdResult](../resources/convertidresult.md) -Auflistung im Antworttext.

## <a name="example"></a>Beispiel

Das folgende Beispiel zeigt, wie mehrere Bezeichner der REST-API-Standardformat konvertiert (`restId`) in das unveränderlich REST-Format (`restImmutableEntryId`).

### <a name="request"></a>Anforderung

Hier sehen Sie die Beispielanforderung:
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

### <a name="response"></a>Antwort

Nachfolgend finden Sie die Beispielantwort
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

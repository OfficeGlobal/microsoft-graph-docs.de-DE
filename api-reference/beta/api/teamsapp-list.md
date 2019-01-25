---
title: Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog
description: 'Liste apps aus dem Microsoft-Teams, app-Katalog. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d43f9a8cca7c16bab3b0dec90b26d4c9c6d4d33c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519269"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste der [apps](../resources/teamsapp.md) aus dem Microsoft-Teams, app-Katalog. Dazu gehören apps aus dem Microsoft-Teams Store als auch apps aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog). Wenn Sie apps aus app-Katalog nur Ihrer Organisation erhalten möchten, geben Sie `Organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Hinweis:** Nur globale Administratoren können diese API aufrufen. 

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:----------------------------------     |:-------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | AppCatalog.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt|
| Anwendung                            | Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile        | Wert           |
|:--------------|:--------------  |
| Authorization | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Keine.

>**Hinweis:** Sie können die Felder des [TeamsCatalogApp](../resources/teamsapp.md) -Objekts in der Ergebnisliste verkürzte filtern. Sie können eine der folgenden Filter Vorgänge verwenden: gleich, nicht gleich, und, oder, und nicht.

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [TeamsCatalogApp](../resources/teamsapp.md) .

## <a name="examples"></a>Beispiele
### <a name="example-1"></a>Beispiel 1
Das folgende Beispiel listet alle Anwendungen, die für Ihre Mandanten spezifisch sind.

#### <a name="request"></a>Anforderung
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a>Antwort
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a>Beispiel 2

Das folgende Beispiel listet Applikationen mit einer bestimmten ID.

#### <a name="request"></a>Anforderung
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>Antwort
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

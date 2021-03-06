---
title: Auflisten von Websites
description: Liste der verfügbaren [Standorte] [] in einer Organisation, die bereitgestellten Filterkriterien entsprechen und Abfragen Optionen.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f225d9990637f8251ae40e3f66b0f993bbf74f32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520340"
---
# <a name="enumerate-sites"></a>Auflisten von Websites

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste der verfügbaren [Websites][] in einer Organisation, die bereitgestellten Filterkriterien entsprechen und Abfragen Optionen.

Derzeit werden nur die folgenden Abfrageoptionen unterstützt:

| Filter-Anweisung             | SELECT-Anweisung        | Beschreibung
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | Werden alle auf der Stammebene Websitesammlungen in der Organisation aufgelistet. Ermitteln die Website der Homepage für jede Region nützlich.

Darüber hinaus können Sie **[eine Suchabfrage für die Auflistung "/ sites"][]** angegebenen Schlüsselwörter übereinstimmenden Websites suchen verwenden.

Suche
[sites]: ../resources/site.md

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:--------------------------------------|:-------------------------------------
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | Sites.Read.All, Sites.ReadWrite.All
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt
|Anwendung                            | Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a>Beispiel

#### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

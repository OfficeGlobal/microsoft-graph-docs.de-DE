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
# <a name="enumerate-sites"></a><span data-ttu-id="f8c6d-103">Auflisten von Websites</span><span class="sxs-lookup"><span data-stu-id="f8c6d-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c6d-104">Liste der verfügbaren [Websites][] in einer Organisation, die bereitgestellten Filterkriterien entsprechen und Abfragen Optionen.</span><span class="sxs-lookup"><span data-stu-id="f8c6d-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="f8c6d-105">Derzeit werden nur die folgenden Abfrageoptionen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="f8c6d-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="f8c6d-106">Filter-Anweisung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-106">Filter statement</span></span>             | <span data-ttu-id="f8c6d-107">SELECT-Anweisung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-107">Select statement</span></span>        | <span data-ttu-id="f8c6d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="f8c6d-109">Werden alle auf der Stammebene Websitesammlungen in der Organisation aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="f8c6d-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="f8c6d-110">Ermitteln die Website der Homepage für jede Region nützlich.</span><span class="sxs-lookup"><span data-stu-id="f8c6d-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="f8c6d-111">Darüber hinaus können Sie **[eine Suchabfrage für die Auflistung "/ sites"][]** angegebenen Schlüsselwörter übereinstimmenden Websites suchen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f8c6d-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

<span data-ttu-id="f8c6d-112">Suche</span><span class="sxs-lookup"><span data-stu-id="f8c6d-112">[search]: site-search.md</span></span>
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f8c6d-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8c6d-114">Permissions</span></span>

<span data-ttu-id="f8c6d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8c6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8c6d-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8c6d-117">Permission type</span></span>                        | <span data-ttu-id="f8c6d-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8c6d-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f8c6d-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8c6d-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8c6d-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c6d-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f8c6d-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8c6d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8c6d-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8c6d-122">Not supported.</span></span>
|<span data-ttu-id="f8c6d-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-123">Application</span></span>                            | <span data-ttu-id="f8c6d-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c6d-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f8c6d-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="f8c6d-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8c6d-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8c6d-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8c6d-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="f8c6d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8c6d-128">Response</span></span>

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

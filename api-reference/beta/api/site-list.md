---
title: Auflisten von Websites
description: Liste der verfügbaren [Standorte] [] in einer Organisation, die bereitgestellten Filterkriterien entsprechen und Abfragen Optionen.
localization_priority: Normal
ms.openlocfilehash: 87ce5b68ccadffa6e0422c413ab79ee784f361c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855818"
---
# <a name="enumerate-sites"></a><span data-ttu-id="65d1c-103">Auflisten von Websites</span><span class="sxs-lookup"><span data-stu-id="65d1c-103">Enumerate sites</span></span>

> <span data-ttu-id="65d1c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65d1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65d1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65d1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65d1c-106">Liste der verfügbaren [Websites][] in einer Organisation, die bereitgestellten Filterkriterien entsprechen und Abfragen Optionen.</span><span class="sxs-lookup"><span data-stu-id="65d1c-106">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="65d1c-107">Derzeit werden nur die folgenden Abfrageoptionen unterstützt:</span><span class="sxs-lookup"><span data-stu-id="65d1c-107">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="65d1c-108">Filter-Anweisung</span><span class="sxs-lookup"><span data-stu-id="65d1c-108">Filter statement</span></span>             | <span data-ttu-id="65d1c-109">SELECT-Anweisung</span><span class="sxs-lookup"><span data-stu-id="65d1c-109">Select statement</span></span>        | <span data-ttu-id="65d1c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65d1c-110">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="65d1c-111">Werden alle auf der Stammebene Websitesammlungen in der Organisation aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="65d1c-111">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="65d1c-112">Ermitteln die Website der Homepage für jede Region nützlich.</span><span class="sxs-lookup"><span data-stu-id="65d1c-112">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="65d1c-113">Darüber hinaus können Sie **[eine Suchabfrage für die Auflistung "/ sites"][]** angegebenen Schlüsselwörter übereinstimmenden Websites suchen verwenden.</span><span class="sxs-lookup"><span data-stu-id="65d1c-113">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[Suche]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="65d1c-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65d1c-116">Permissions</span></span>

<span data-ttu-id="65d1c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d1c-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65d1c-119">Permission type</span></span>                        | <span data-ttu-id="65d1c-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65d1c-120">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="65d1c-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65d1c-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="65d1c-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d1c-122">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="65d1c-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65d1c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d1c-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65d1c-124">Not supported.</span></span>
|<span data-ttu-id="65d1c-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65d1c-125">Application</span></span>                            | <span data-ttu-id="65d1c-126">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d1c-126">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="65d1c-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65d1c-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="65d1c-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65d1c-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="65d1c-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65d1c-129">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="65d1c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="65d1c-130">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->

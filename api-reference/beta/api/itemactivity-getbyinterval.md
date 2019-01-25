---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Rufen Sie Element-Aktivität Stats ab, indem Sie Intervall
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516455"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="6f3d6-102">Rufen Sie Element-Aktivität Stats ab, indem Sie Intervall</span><span class="sxs-lookup"><span data-stu-id="6f3d6-102">Get item activity stats by interval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f3d6-103">Rufen Sie [ItemActivityStats][] für die Aktivitäten, die stattgefunden unter diese Ressource innerhalb des angegebenen Zeitintervalls.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-103">Get [itemActivityStats][] for the activities that took place under this resource within the specified time interval.</span></span>

><span data-ttu-id="6f3d6-104">**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-104">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="6f3d6-105">Analytics Aggregate möglicherweise nicht für alle Aktivitätstypen von zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-105">Analytics aggregates might not be available for all action types.</span></span>

[itemActivityStats]: ../resources/itemactivitystat.md

## <a name="permissions"></a><span data-ttu-id="6f3d6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f3d6-107">Permissions</span></span>

<span data-ttu-id="6f3d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f3d6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f3d6-110">Permission type</span></span>                        | <span data-ttu-id="6f3d6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f3d6-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6f3d6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f3d6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f3d6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3d6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="6f3d6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f3d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f3d6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f3d6-115">Not supported.</span></span>
|<span data-ttu-id="6f3d6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f3d6-116">Application</span></span>                            | <span data-ttu-id="6f3d6-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3d6-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6f3d6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f3d6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="6f3d6-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="6f3d6-119">Function parameters</span></span>

| <span data-ttu-id="6f3d6-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="6f3d6-120">Parameter</span></span>      | <span data-ttu-id="6f3d6-121">Typ</span><span class="sxs-lookup"><span data-stu-id="6f3d6-121">Type</span></span>               | <span data-ttu-id="6f3d6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f3d6-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="6f3d6-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f3d6-123">startDateTime</span></span>  | <span data-ttu-id="6f3d6-124">Zeichenfolge (Zeitstempel)</span><span class="sxs-lookup"><span data-stu-id="6f3d6-124">string (timestamp)</span></span> | <span data-ttu-id="6f3d6-125">Die Anfangszeit über die aggregierte Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="6f3d6-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6f3d6-126">endDateTime</span></span>    | <span data-ttu-id="6f3d6-127">Zeichenfolge (Zeitstempel)</span><span class="sxs-lookup"><span data-stu-id="6f3d6-127">string (timestamp)</span></span> | <span data-ttu-id="6f3d6-128">Die Endzeit über die aggregierte Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="6f3d6-129">Intervall</span><span class="sxs-lookup"><span data-stu-id="6f3d6-129">interval</span></span>       | <span data-ttu-id="6f3d6-130">string</span><span class="sxs-lookup"><span data-stu-id="6f3d6-130">string</span></span>             | <span data-ttu-id="6f3d6-131">Das Intervall Aggregation.</span><span class="sxs-lookup"><span data-stu-id="6f3d6-131">The aggregation interval.</span></span>

## <a name="example"></a><span data-ttu-id="6f3d6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f3d6-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6f3d6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f3d6-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a><span data-ttu-id="6f3d6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f3d6-134">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
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
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

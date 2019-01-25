---
title: Verwendet wird
description: Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: e73536d5933d6293539eb00ba8cdc2e85ce5fa93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526102"
---
# <a name="list-used"></a><span data-ttu-id="43c3d-103">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="43c3d-103">List used</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43c3d-104">Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="43c3d-104">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="43c3d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43c3d-105">Permissions</span></span>
<span data-ttu-id="43c3d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43c3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c3d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43c3d-108">Permission type</span></span>      | <span data-ttu-id="43c3d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43c3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43c3d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43c3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43c3d-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c3d-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="43c3d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43c3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43c3d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43c3d-113">Not supported.</span></span>    |
|<span data-ttu-id="43c3d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43c3d-114">Application</span></span> | <span data-ttu-id="43c3d-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c3d-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43c3d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43c3d-116">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="43c3d-117">Anfordern eines anderen Benutzers verwendete Dokumente gibt Ergebnisse sortiert nach 'LastModifiedDateTime' und 'LastAccessedDateTime' auf 'LastModifiedDateTime' festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="43c3d-117">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43c3d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="43c3d-118">Optional query parameters</span></span>
<span data-ttu-id="43c3d-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43c3d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="43c3d-120">Sie können die `$filter` Abfragen Parameter zum Filtern verwendet von Elementen.</span><span class="sxs-lookup"><span data-stu-id="43c3d-120">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="43c3d-121">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="43c3d-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="43c3d-122">Basierend auf Containertyp oder:</span><span class="sxs-lookup"><span data-stu-id="43c3d-122">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="43c3d-123">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="43c3d-123">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="43c3d-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43c3d-124">Request headers</span></span>
| <span data-ttu-id="43c3d-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43c3d-125">Header</span></span>       |  <span data-ttu-id="43c3d-126">Wert</span><span class="sxs-lookup"><span data-stu-id="43c3d-126">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="43c3d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c3d-127">Authorization</span></span>  | <span data-ttu-id="43c3d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43c3d-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="43c3d-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43c3d-130">Accept</span></span>  | <span data-ttu-id="43c3d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="43c3d-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c3d-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43c3d-132">Request body</span></span>
<span data-ttu-id="43c3d-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43c3d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c3d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="43c3d-134">Response</span></span>

<span data-ttu-id="43c3d-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [verwendet](../resources/insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="43c3d-135">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43c3d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43c3d-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43c3d-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43c3d-137">Request</span></span>

<span data-ttu-id="43c3d-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43c3d-138">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="43c3d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="43c3d-139">Response</span></span>

<span data-ttu-id="43c3d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43c3d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
            }
        }
    ]
}
```

### <a name="expanding-resource"></a><span data-ttu-id="43c3d-143">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="43c3d-143">Expanding resource</span></span>
<span data-ttu-id="43c3d-144">Die Ressource, die durch eine verwendeten Erkenntnisse kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="43c3d-144">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

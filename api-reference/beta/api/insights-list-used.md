---
title: Verwendet wird
description: Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.
ms.openlocfilehash: a9e5390e38e4e697f55676304edb4544e4c2ded5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062612"
---
# <a name="list-used"></a><span data-ttu-id="db10d-103">Verwendet wird</span><span class="sxs-lookup"><span data-stu-id="db10d-103">List used</span></span>

> <span data-ttu-id="db10d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db10d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db10d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db10d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db10d-106">Berechnete Insight, der die Liste der Dateien mit einem Benutzer zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="db10d-106">Calculated insight that returns the list of files used with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="db10d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db10d-107">Permissions</span></span>
<span data-ttu-id="db10d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db10d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db10d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db10d-110">Permission type</span></span>      | <span data-ttu-id="db10d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db10d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db10d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db10d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db10d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db10d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db10d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db10d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db10d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db10d-115">Not supported.</span></span>    |
|<span data-ttu-id="db10d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db10d-116">Application</span></span> | <span data-ttu-id="db10d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db10d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db10d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db10d-118">HTTP request</span></span>
```http
GET /me/insights/used
```
<span data-ttu-id="db10d-119">Anfordern eines anderen Benutzers verwendete Dokumente gibt Ergebnisse sortiert nach 'LastModifiedDateTime' und 'LastAccessedDateTime' auf 'LastModifiedDateTime' festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="db10d-119">Requesting other user's used documents returns results sorted by 'lastModifiedDateTime' and 'lastAccessedDateTime' is set to 'lastModifiedDateTime'.</span></span>
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db10d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="db10d-120">Optional query parameters</span></span>
<span data-ttu-id="db10d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="db10d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="db10d-122">Sie können die `$filter` Abfragen Parameter zum Filtern verwendet von Elementen.</span><span class="sxs-lookup"><span data-stu-id="db10d-122">You can use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="db10d-123">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="db10d-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="db10d-124">Basierend auf Containertyp oder:</span><span class="sxs-lookup"><span data-stu-id="db10d-124">Or based on Container Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="db10d-125">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="db10d-125">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="db10d-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db10d-126">Request headers</span></span>
| <span data-ttu-id="db10d-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db10d-127">Header</span></span>       |  <span data-ttu-id="db10d-128">Wert</span><span class="sxs-lookup"><span data-stu-id="db10d-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="db10d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="db10d-129">Authorization</span></span>  | <span data-ttu-id="db10d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db10d-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="db10d-132">Accept</span><span class="sxs-lookup"><span data-stu-id="db10d-132">Accept</span></span>  | <span data-ttu-id="db10d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="db10d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db10d-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db10d-134">Request body</span></span>
<span data-ttu-id="db10d-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="db10d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db10d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="db10d-136">Response</span></span>

<span data-ttu-id="db10d-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der Elemente im Antworttext [verwendet](../resources/insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="db10d-137">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db10d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db10d-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db10d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="db10d-139">Request</span></span>

<span data-ttu-id="db10d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db10d-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a><span data-ttu-id="db10d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="db10d-141">Response</span></span>

<span data-ttu-id="db10d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db10d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span> 
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

### <a name="expanding-resource"></a><span data-ttu-id="db10d-145">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="db10d-145">Expanding resource</span></span>
<span data-ttu-id="db10d-146">Die Ressource, die durch eine verwendeten Erkenntnisse kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="db10d-146">The resource referenced by a used insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```

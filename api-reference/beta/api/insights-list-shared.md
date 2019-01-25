---
title: Gemeinsame Liste
description: Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2eef2a9b306984a8ad05bcf8fefca2458d609ab1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517351"
---
# <a name="list-shared"></a><span data-ttu-id="a770d-103">Gemeinsame Liste</span><span class="sxs-lookup"><span data-stu-id="a770d-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a770d-104">Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="a770d-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a770d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a770d-105">Permissions</span></span>
<span data-ttu-id="a770d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a770d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a770d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a770d-108">Permission type</span></span>      | <span data-ttu-id="a770d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a770d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a770d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a770d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a770d-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a770d-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a770d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a770d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a770d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a770d-113">Not supported.</span></span>    |
|<span data-ttu-id="a770d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a770d-114">Application</span></span> | <span data-ttu-id="a770d-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a770d-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a770d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a770d-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="a770d-117">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer, die nicht von einer anderen Person:</span><span class="sxs-lookup"><span data-stu-id="a770d-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a770d-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a770d-118">Optional query parameters</span></span>
<span data-ttu-id="a770d-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a770d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a770d-120">Sie können die `$filter` Parameter zum Filtern von freigegebenen Elemente Abfragen.</span><span class="sxs-lookup"><span data-stu-id="a770d-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="a770d-121">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="a770d-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="a770d-122">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="a770d-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="a770d-123">Sie können auch von einem bestimmten Benutzer gemeinsam genutzte Dateien abrufen.</span><span class="sxs-lookup"><span data-stu-id="a770d-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="a770d-124">Beispielsweise durch Angabe der `lastshared/sharedby/address` Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="a770d-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="a770d-125">Finden Sie unter den komplexen Typ [SharingDetail](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="a770d-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a770d-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a770d-126">Request headers</span></span>
| <span data-ttu-id="a770d-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a770d-127">Header</span></span>       |  <span data-ttu-id="a770d-128">Wert</span><span class="sxs-lookup"><span data-stu-id="a770d-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="a770d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a770d-129">Authorization</span></span>  | <span data-ttu-id="a770d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a770d-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a770d-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a770d-132">Accept</span></span>  | <span data-ttu-id="a770d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a770d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a770d-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a770d-134">Request body</span></span>
<span data-ttu-id="a770d-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a770d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a770d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a770d-136">Response</span></span>

<span data-ttu-id="a770d-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der [freigegebenen](../resources/insights-shared.md) Elemente im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a770d-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a770d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a770d-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a770d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a770d-139">Request</span></span>

<span data-ttu-id="a770d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a770d-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="a770d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a770d-141">Response</span></span>

<span data-ttu-id="a770d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a770d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
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
```

### <a name="expanding-resource"></a><span data-ttu-id="a770d-145">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="a770d-145">Expanding resource</span></span>
<span data-ttu-id="a770d-146">Die Ressource, die durch einen freigegebenen Einblick kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="a770d-146">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/insights-list-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

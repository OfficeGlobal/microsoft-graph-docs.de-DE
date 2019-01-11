---
title: Gemeinsame Liste
description: Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: eb9d0165d61559d5f31af486b96e1127c9c7c43c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843267"
---
# <a name="list-shared"></a><span data-ttu-id="717e3-103">Gemeinsame Liste</span><span class="sxs-lookup"><span data-stu-id="717e3-103">List shared</span></span>

> <span data-ttu-id="717e3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="717e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="717e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="717e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="717e3-106">Berechnete Insight, der die Liste der Dateien, die ein Benutzer freigegeben zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="717e3-106">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="717e3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="717e3-107">Permissions</span></span>
<span data-ttu-id="717e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="717e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="717e3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="717e3-110">Permission type</span></span>      | <span data-ttu-id="717e3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="717e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="717e3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="717e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="717e3-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717e3-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="717e3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="717e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="717e3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="717e3-115">Not supported.</span></span>    |
|<span data-ttu-id="717e3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="717e3-116">Application</span></span> | <span data-ttu-id="717e3-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="717e3-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="717e3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="717e3-118">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="717e3-119">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer, die nicht von einer anderen Person:</span><span class="sxs-lookup"><span data-stu-id="717e3-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="717e3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="717e3-120">Optional query parameters</span></span>
<span data-ttu-id="717e3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="717e3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="717e3-122">Sie können die `$filter` Parameter zum Filtern von freigegebenen Elemente Abfragen.</span><span class="sxs-lookup"><span data-stu-id="717e3-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="717e3-123">Beispielsweise basierend auf:</span><span class="sxs-lookup"><span data-stu-id="717e3-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="717e3-124">Finden Sie die verfügbaren Containertypen und Typen, die Sie nach [ResourceVisualization](../resources/insights-resourcevisualization.md)filtern können.</span><span class="sxs-lookup"><span data-stu-id="717e3-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="717e3-125">Sie können auch von einem bestimmten Benutzer gemeinsam genutzte Dateien abrufen.</span><span class="sxs-lookup"><span data-stu-id="717e3-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="717e3-126">Beispielsweise durch Angabe der `lastshared/sharedby/address` Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="717e3-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="717e3-127">Finden Sie unter den komplexen Typ [SharingDetail](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="717e3-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="717e3-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="717e3-128">Request headers</span></span>
| <span data-ttu-id="717e3-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="717e3-129">Header</span></span>       |  <span data-ttu-id="717e3-130">Wert</span><span class="sxs-lookup"><span data-stu-id="717e3-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="717e3-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="717e3-131">Authorization</span></span>  | <span data-ttu-id="717e3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="717e3-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="717e3-134">Annehmen</span><span class="sxs-lookup"><span data-stu-id="717e3-134">Accept</span></span>  | <span data-ttu-id="717e3-135">application/json</span><span class="sxs-lookup"><span data-stu-id="717e3-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="717e3-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="717e3-136">Request body</span></span>
<span data-ttu-id="717e3-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="717e3-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="717e3-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="717e3-138">Response</span></span>

<span data-ttu-id="717e3-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste der [freigegebenen](../resources/insights-shared.md) Elemente im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="717e3-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="717e3-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="717e3-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="717e3-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="717e3-141">Request</span></span>

<span data-ttu-id="717e3-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="717e3-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="717e3-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="717e3-143">Response</span></span>

<span data-ttu-id="717e3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="717e3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="717e3-147">Erweitern der Ressource</span><span class="sxs-lookup"><span data-stu-id="717e3-147">Expanding resource</span></span>
<span data-ttu-id="717e3-148">Die Ressource, die durch einen freigegebenen Einblick kann erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="717e3-148">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```

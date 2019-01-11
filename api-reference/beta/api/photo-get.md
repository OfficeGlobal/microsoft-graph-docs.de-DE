---
title: Foto abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.
localization_priority: Normal
ms.openlocfilehash: ff46fca695140cabf363f9bccfcc61bc4fb50279
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824465"
---
# <a name="get-photo"></a><span data-ttu-id="e55cf-103">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="e55cf-103">Get photo</span></span>

> <span data-ttu-id="e55cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e55cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e55cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e55cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e55cf-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="e55cf-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e55cf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e55cf-107">Permissions</span></span>
<span data-ttu-id="e55cf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e55cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e55cf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e55cf-110">Permission type</span></span>      | <span data-ttu-id="e55cf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e55cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e55cf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e55cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e55cf-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e55cf-113">Files.Read</span></span>    |
|<span data-ttu-id="e55cf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e55cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e55cf-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="e55cf-115">Files.Read</span></span>    |
|<span data-ttu-id="e55cf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e55cf-116">Application</span></span> | <span data-ttu-id="e55cf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e55cf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e55cf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e55cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e55cf-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e55cf-119">Optional query parameters</span></span>
<span data-ttu-id="e55cf-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e55cf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e55cf-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e55cf-121">Request headers</span></span>
| <span data-ttu-id="e55cf-122">Name</span><span class="sxs-lookup"><span data-stu-id="e55cf-122">Name</span></span>       | <span data-ttu-id="e55cf-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e55cf-123">Type</span></span> | <span data-ttu-id="e55cf-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e55cf-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e55cf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e55cf-125">Authorization</span></span>  | <span data-ttu-id="e55cf-126">string</span><span class="sxs-lookup"><span data-stu-id="e55cf-126">string</span></span>  | <span data-ttu-id="e55cf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e55cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e55cf-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e55cf-129">Request body</span></span>
<span data-ttu-id="e55cf-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e55cf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e55cf-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e55cf-131">Response</span></span>

<span data-ttu-id="e55cf-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e55cf-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e55cf-133">Beispiele</span><span class="sxs-lookup"><span data-stu-id="e55cf-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="e55cf-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e55cf-134">Request</span></span>
<span data-ttu-id="e55cf-135">Dies ist ein Beispiel für die Anforderung von Foto-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="e55cf-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="e55cf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e55cf-136">Response</span></span>
<span data-ttu-id="e55cf-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e55cf-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="e55cf-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e55cf-138">Request</span></span>
<span data-ttu-id="e55cf-139">Hier ist ein Beispiel für die Anforderung der Fotobytes.</span><span class="sxs-lookup"><span data-stu-id="e55cf-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="e55cf-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="e55cf-140">Response</span></span>
<span data-ttu-id="e55cf-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e55cf-141">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored","@odata.type": "stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

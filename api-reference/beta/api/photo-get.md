---
title: Foto abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.
localization_priority: Normal
ms.openlocfilehash: ffe127cf7e59a4cf29275a7673cb95e1ce7e4581
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510351"
---
# <a name="get-photo"></a><span data-ttu-id="efc84-103">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="efc84-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efc84-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="efc84-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="efc84-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="efc84-105">Permissions</span></span>
<span data-ttu-id="efc84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efc84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efc84-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efc84-108">Permission type</span></span>      | <span data-ttu-id="efc84-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efc84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efc84-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efc84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efc84-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="efc84-111">Files.Read</span></span>    |
|<span data-ttu-id="efc84-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efc84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efc84-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="efc84-113">Files.Read</span></span>    |
|<span data-ttu-id="efc84-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efc84-114">Application</span></span> | <span data-ttu-id="efc84-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efc84-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efc84-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efc84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efc84-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="efc84-117">Optional query parameters</span></span>
<span data-ttu-id="efc84-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efc84-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efc84-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="efc84-119">Request headers</span></span>
| <span data-ttu-id="efc84-120">Name</span><span class="sxs-lookup"><span data-stu-id="efc84-120">Name</span></span>       | <span data-ttu-id="efc84-121">Typ</span><span class="sxs-lookup"><span data-stu-id="efc84-121">Type</span></span> | <span data-ttu-id="efc84-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efc84-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="efc84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="efc84-123">Authorization</span></span>  | <span data-ttu-id="efc84-124">string</span><span class="sxs-lookup"><span data-stu-id="efc84-124">string</span></span>  | <span data-ttu-id="efc84-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="efc84-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efc84-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="efc84-127">Request body</span></span>
<span data-ttu-id="efc84-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="efc84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efc84-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="efc84-129">Response</span></span>

<span data-ttu-id="efc84-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efc84-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="efc84-131">Beispiele</span><span class="sxs-lookup"><span data-stu-id="efc84-131">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="efc84-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efc84-132">Request</span></span>
<span data-ttu-id="efc84-133">Dies ist ein Beispiel für die Anforderung von Foto-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="efc84-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="efc84-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="efc84-134">Response</span></span>
<span data-ttu-id="efc84-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efc84-135">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="efc84-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efc84-136">Request</span></span>
<span data-ttu-id="efc84-137">Hier ist ein Beispiel für die Anforderung der Fotobytes.</span><span class="sxs-lookup"><span data-stu-id="efc84-137">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="efc84-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="efc84-138">Response</span></span>
<span data-ttu-id="efc84-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efc84-139">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/photo-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

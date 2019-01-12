---
title: Geräte auflisten
description: Mit dieser API können Sie eine Liste der in einer Organisation registrierten Geräteobjekte abrufen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d6b67d883a834c6e36c8fdde91844cea15f4ce04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990467"
---
# <a name="list-devices"></a><span data-ttu-id="ec5ba-103">Geräte auflisten</span><span class="sxs-lookup"><span data-stu-id="ec5ba-103">List devices</span></span>

<span data-ttu-id="ec5ba-104">Mit dieser API können Sie eine Liste der in einer Organisation registrierten Geräteobjekte abrufen.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-104">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec5ba-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec5ba-105">Permissions</span></span>
<span data-ttu-id="ec5ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ec5ba-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec5ba-108">Permission type</span></span>      | <span data-ttu-id="ec5ba-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec5ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec5ba-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec5ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec5ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec5ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec5ba-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec5ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec5ba-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec5ba-113">Not supported.</span></span>    |
|<span data-ttu-id="ec5ba-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec5ba-114">Application</span></span> | <span data-ttu-id="ec5ba-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec5ba-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec5ba-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec5ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec5ba-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ec5ba-117">Optional query parameters</span></span>
<span data-ttu-id="ec5ba-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ec5ba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec5ba-119">Request headers</span></span>
| <span data-ttu-id="ec5ba-120">Name</span><span class="sxs-lookup"><span data-stu-id="ec5ba-120">Name</span></span>       | <span data-ttu-id="ec5ba-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ec5ba-121">Type</span></span> | <span data-ttu-id="ec5ba-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec5ba-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ec5ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec5ba-123">Authorization</span></span>  | <span data-ttu-id="ec5ba-124">string</span><span class="sxs-lookup"><span data-stu-id="ec5ba-124">string</span></span>  | <span data-ttu-id="ec5ba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec5ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec5ba-127">Request body</span></span>
<span data-ttu-id="ec5ba-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec5ba-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec5ba-129">Response</span></span>

<span data-ttu-id="ec5ba-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [device](../resources/device.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec5ba-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec5ba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec5ba-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec5ba-132">Request</span></span>
<span data-ttu-id="ec5ba-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="ec5ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec5ba-134">Response</span></span>
<span data-ttu-id="ec5ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec5ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

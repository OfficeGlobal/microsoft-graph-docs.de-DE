---
title: Gerät abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.
ms.openlocfilehash: 07ee10ccc6f3cfb7649df2cb3711bfff24115036
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019536"
---
# <a name="get-device"></a><span data-ttu-id="82cc3-103">Gerät abrufen</span><span class="sxs-lookup"><span data-stu-id="82cc3-103">Get device</span></span>

<span data-ttu-id="82cc3-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="82cc3-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="82cc3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82cc3-105">Permissions</span></span>
<span data-ttu-id="82cc3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="82cc3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82cc3-108">Permission type</span></span>      | <span data-ttu-id="82cc3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82cc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82cc3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82cc3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82cc3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82cc3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82cc3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82cc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cc3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82cc3-113">Not supported.</span></span>    |
|<span data-ttu-id="82cc3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82cc3-114">Application</span></span> | <span data-ttu-id="82cc3-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cc3-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82cc3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82cc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="82cc3-117">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="82cc3-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="82cc3-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="82cc3-118">Optional query parameters</span></span>
<span data-ttu-id="82cc3-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82cc3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82cc3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82cc3-120">Request headers</span></span>
| <span data-ttu-id="82cc3-121">Name</span><span class="sxs-lookup"><span data-stu-id="82cc3-121">Name</span></span>       | <span data-ttu-id="82cc3-122">Typ</span><span class="sxs-lookup"><span data-stu-id="82cc3-122">Type</span></span> | <span data-ttu-id="82cc3-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82cc3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82cc3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82cc3-124">Authorization</span></span>  | <span data-ttu-id="82cc3-125">string</span><span class="sxs-lookup"><span data-stu-id="82cc3-125">string</span></span>  | <span data-ttu-id="82cc3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82cc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82cc3-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82cc3-128">Request body</span></span>
<span data-ttu-id="82cc3-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="82cc3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82cc3-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="82cc3-130">Response</span></span>

<span data-ttu-id="82cc3-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82cc3-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82cc3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82cc3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82cc3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82cc3-133">Request</span></span>
<span data-ttu-id="82cc3-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82cc3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="82cc3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="82cc3-135">Response</span></span>
<span data-ttu-id="82cc3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82cc3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: Gerät erstellen
description: Mit dieser API können Sie ein neues Gerät in der Organisation registrieren.
ms.openlocfilehash: 7dd4ab48c66383990eb3fca4630717ba8063c67a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017687"
---
# <a name="create-device"></a><span data-ttu-id="c80ab-103">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="c80ab-103">Create device</span></span>

<span data-ttu-id="c80ab-104">Mit dieser API können Sie ein neues Gerät in der Organisation registrieren.</span><span class="sxs-lookup"><span data-stu-id="c80ab-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c80ab-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c80ab-105">Permissions</span></span>
<span data-ttu-id="c80ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c80ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c80ab-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c80ab-108">Permission type</span></span>      | <span data-ttu-id="c80ab-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c80ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c80ab-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c80ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c80ab-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c80ab-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c80ab-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c80ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c80ab-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c80ab-113">Not supported.</span></span>    |
|<span data-ttu-id="c80ab-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c80ab-114">Application</span></span> | <span data-ttu-id="c80ab-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c80ab-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c80ab-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c80ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="c80ab-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c80ab-117">Request headers</span></span>
| <span data-ttu-id="c80ab-118">Name</span><span class="sxs-lookup"><span data-stu-id="c80ab-118">Name</span></span>       | <span data-ttu-id="c80ab-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c80ab-119">Type</span></span> | <span data-ttu-id="c80ab-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c80ab-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c80ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c80ab-121">Authorization</span></span>  | <span data-ttu-id="c80ab-122">string</span><span class="sxs-lookup"><span data-stu-id="c80ab-122">string</span></span>  | <span data-ttu-id="c80ab-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c80ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c80ab-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="c80ab-125">Content-type</span></span> | <span data-ttu-id="c80ab-126">string</span><span class="sxs-lookup"><span data-stu-id="c80ab-126">string</span></span> | <span data-ttu-id="c80ab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c80ab-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c80ab-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c80ab-128">Request body</span></span>
<span data-ttu-id="c80ab-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c80ab-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c80ab-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c80ab-130">Response</span></span>

<span data-ttu-id="c80ab-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c80ab-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c80ab-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c80ab-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c80ab-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c80ab-133">Request</span></span>
<span data-ttu-id="c80ab-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c80ab-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
<span data-ttu-id="c80ab-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c80ab-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c80ab-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c80ab-136">Response</span></span>
<span data-ttu-id="c80ab-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c80ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type":2,
      "key":"base64Y3YxN2E1MWFlYw=="
    }
  ],
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
  "description": "Create device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

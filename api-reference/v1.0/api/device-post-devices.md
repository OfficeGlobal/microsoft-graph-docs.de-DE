---
title: Gerät erstellen
description: Mit dieser API können Sie ein neues Gerät in der Organisation registrieren.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e0dafeb56b6551070bc157ee53b4a9f7f6ac984e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811809"
---
# <a name="create-device"></a><span data-ttu-id="67b84-103">Gerät erstellen</span><span class="sxs-lookup"><span data-stu-id="67b84-103">Create device</span></span>

<span data-ttu-id="67b84-104">Mit dieser API können Sie ein neues Gerät in der Organisation registrieren.</span><span class="sxs-lookup"><span data-stu-id="67b84-104">Create and register a new device in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="67b84-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67b84-105">Permissions</span></span>
<span data-ttu-id="67b84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67b84-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67b84-108">Permission type</span></span>      | <span data-ttu-id="67b84-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67b84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b84-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67b84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67b84-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67b84-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67b84-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67b84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b84-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67b84-113">Not supported.</span></span>    |
|<span data-ttu-id="67b84-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67b84-114">Application</span></span> | <span data-ttu-id="67b84-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67b84-115">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b84-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67b84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices

```
## <a name="request-headers"></a><span data-ttu-id="67b84-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67b84-117">Request headers</span></span>
| <span data-ttu-id="67b84-118">Name</span><span class="sxs-lookup"><span data-stu-id="67b84-118">Name</span></span>       | <span data-ttu-id="67b84-119">Typ</span><span class="sxs-lookup"><span data-stu-id="67b84-119">Type</span></span> | <span data-ttu-id="67b84-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67b84-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67b84-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67b84-121">Authorization</span></span>  | <span data-ttu-id="67b84-122">string</span><span class="sxs-lookup"><span data-stu-id="67b84-122">string</span></span>  | <span data-ttu-id="67b84-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67b84-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67b84-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="67b84-125">Content-type</span></span> | <span data-ttu-id="67b84-126">string</span><span class="sxs-lookup"><span data-stu-id="67b84-126">string</span></span> | <span data-ttu-id="67b84-127">application/json</span><span class="sxs-lookup"><span data-stu-id="67b84-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="67b84-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67b84-128">Request body</span></span>
<span data-ttu-id="67b84-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="67b84-129">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="67b84-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="67b84-130">Response</span></span>

<span data-ttu-id="67b84-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67b84-131">If successful, this method returns `201 Created` response code and [device](../resources/device.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67b84-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67b84-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67b84-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67b84-133">Request</span></span>
<span data-ttu-id="67b84-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67b84-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="67b84-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [device](../resources/device.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="67b84-135">In the request body, supply a JSON representation of [device](../resources/device.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="67b84-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="67b84-136">Response</span></span>
<span data-ttu-id="67b84-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67b84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

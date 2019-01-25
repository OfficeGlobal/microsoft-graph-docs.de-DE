---
title: Gerät abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b0bc325620a27d9383b4a12d5f3da970c0c267
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515972"
---
# <a name="get-device"></a><span data-ttu-id="fcf31-103">Gerät abrufen</span><span class="sxs-lookup"><span data-stu-id="fcf31-103">Get device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf31-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="fcf31-104">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="fcf31-105">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine Instanz des **Geräts** .</span><span class="sxs-lookup"><span data-stu-id="fcf31-105">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf31-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fcf31-106">Permissions</span></span>
<span data-ttu-id="fcf31-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fcf31-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fcf31-109">Permission type</span></span>      | <span data-ttu-id="fcf31-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fcf31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcf31-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fcf31-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf31-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fcf31-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fcf31-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fcf31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf31-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fcf31-114">Not supported.</span></span>    |
|<span data-ttu-id="fcf31-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fcf31-115">Application</span></span> | <span data-ttu-id="fcf31-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf31-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcf31-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcf31-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fcf31-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fcf31-118">Optional query parameters</span></span>
<span data-ttu-id="fcf31-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fcf31-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fcf31-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fcf31-120">Request headers</span></span>
| <span data-ttu-id="fcf31-121">Name</span><span class="sxs-lookup"><span data-stu-id="fcf31-121">Name</span></span>       | <span data-ttu-id="fcf31-122">Typ</span><span class="sxs-lookup"><span data-stu-id="fcf31-122">Type</span></span> | <span data-ttu-id="fcf31-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcf31-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcf31-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcf31-124">Authorization</span></span>  | <span data-ttu-id="fcf31-125">string</span><span class="sxs-lookup"><span data-stu-id="fcf31-125">string</span></span>  | <span data-ttu-id="fcf31-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fcf31-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcf31-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fcf31-128">Request body</span></span>
<span data-ttu-id="fcf31-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fcf31-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf31-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcf31-130">Response</span></span>

<span data-ttu-id="fcf31-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcf31-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fcf31-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fcf31-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcf31-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fcf31-133">Request</span></span>
<span data-ttu-id="fcf31-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fcf31-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="fcf31-135">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="fcf31-135">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="fcf31-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fcf31-136">Response</span></span>
<span data-ttu-id="fcf31-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fcf31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="fcf31-140">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fcf31-140">See also</span></span>

- [<span data-ttu-id="fcf31-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="fcf31-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fcf31-142">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="fcf31-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fcf31-143">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="fcf31-143">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

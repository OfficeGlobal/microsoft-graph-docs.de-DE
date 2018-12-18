---
title: Gerät abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.
author: tfitzmac
ms.openlocfilehash: 632094db64cce86a965751d97b0ae9c92d439d5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348265"
---
# <a name="get-device"></a><span data-ttu-id="1019b-103">Gerät abrufen</span><span class="sxs-lookup"><span data-stu-id="1019b-103">Get device</span></span>

> <span data-ttu-id="1019b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1019b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1019b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1019b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1019b-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Geräteobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="1019b-106">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="1019b-107">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine Instanz des **Geräts** .</span><span class="sxs-lookup"><span data-stu-id="1019b-107">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="1019b-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1019b-108">Permissions</span></span>
<span data-ttu-id="1019b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1019b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1019b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1019b-111">Permission type</span></span>      | <span data-ttu-id="1019b-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1019b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1019b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1019b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1019b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1019b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1019b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1019b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1019b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1019b-116">Not supported.</span></span>    |
|<span data-ttu-id="1019b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1019b-117">Application</span></span> | <span data-ttu-id="1019b-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1019b-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1019b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1019b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1019b-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1019b-120">Optional query parameters</span></span>
<span data-ttu-id="1019b-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1019b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1019b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1019b-122">Request headers</span></span>
| <span data-ttu-id="1019b-123">Name</span><span class="sxs-lookup"><span data-stu-id="1019b-123">Name</span></span>       | <span data-ttu-id="1019b-124">Typ</span><span class="sxs-lookup"><span data-stu-id="1019b-124">Type</span></span> | <span data-ttu-id="1019b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1019b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1019b-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1019b-126">Authorization</span></span>  | <span data-ttu-id="1019b-127">string</span><span class="sxs-lookup"><span data-stu-id="1019b-127">string</span></span>  | <span data-ttu-id="1019b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1019b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1019b-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1019b-130">Request body</span></span>
<span data-ttu-id="1019b-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1019b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1019b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1019b-132">Response</span></span>

<span data-ttu-id="1019b-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [device](../resources/device.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1019b-133">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1019b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1019b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1019b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1019b-135">Request</span></span>
<span data-ttu-id="1019b-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1019b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="1019b-137">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="1019b-137">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="1019b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="1019b-138">Response</span></span>
<span data-ttu-id="1019b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1019b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1019b-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1019b-142">See also</span></span>

- [<span data-ttu-id="1019b-143">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1019b-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1019b-144">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="1019b-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1019b-145">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="1019b-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
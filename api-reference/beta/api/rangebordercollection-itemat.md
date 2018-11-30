---
title: 'RangeBorderCollection: ItemAt'
description: Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.
ms.openlocfilehash: e045f700e61301c5f0cf801827279b4b51b71b92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059424"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="b92c7-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="b92c7-103">RangeBorderCollection: ItemAt</span></span>

> <span data-ttu-id="b92c7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b92c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b92c7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b92c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b92c7-106">Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.</span><span class="sxs-lookup"><span data-stu-id="b92c7-106">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="b92c7-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b92c7-107">Permissions</span></span>
<span data-ttu-id="b92c7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b92c7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b92c7-110">Permission type</span></span>      | <span data-ttu-id="b92c7-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b92c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b92c7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b92c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b92c7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b92c7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b92c7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b92c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b92c7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b92c7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b92c7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b92c7-116">Application</span></span> | <span data-ttu-id="b92c7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b92c7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b92c7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b92c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="b92c7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b92c7-119">Request headers</span></span>
| <span data-ttu-id="b92c7-120">Name</span><span class="sxs-lookup"><span data-stu-id="b92c7-120">Name</span></span>       | <span data-ttu-id="b92c7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b92c7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b92c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b92c7-122">Authorization</span></span>  | <span data-ttu-id="b92c7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b92c7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b92c7-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b92c7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b92c7-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b92c7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b92c7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b92c7-128">Request body</span></span>
<span data-ttu-id="b92c7-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b92c7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b92c7-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="b92c7-130">Parameter</span></span>    | <span data-ttu-id="b92c7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b92c7-131">Type</span></span>   |<span data-ttu-id="b92c7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b92c7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b92c7-133">Index</span><span class="sxs-lookup"><span data-stu-id="b92c7-133">index</span></span>|<span data-ttu-id="b92c7-134">number</span><span class="sxs-lookup"><span data-stu-id="b92c7-134">number</span></span>|<span data-ttu-id="b92c7-p105">Index-Wert des abzurufenden Objekts. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="b92c7-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="b92c7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b92c7-137">Response</span></span>

<span data-ttu-id="b92c7-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b92c7-138">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b92c7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b92c7-139">Example</span></span>
<span data-ttu-id="b92c7-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b92c7-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b92c7-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b92c7-141">Request</span></span>
<span data-ttu-id="b92c7-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b92c7-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="b92c7-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b92c7-143">Response</span></span>
<span data-ttu-id="b92c7-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b92c7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
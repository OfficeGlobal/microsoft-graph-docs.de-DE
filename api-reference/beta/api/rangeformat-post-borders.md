---
title: RangeBorder erstellen
description: Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.
ms.openlocfilehash: 0c0d17efd41b3414275639152bc91d8785814524
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060365"
---
# <a name="create-rangeborder"></a><span data-ttu-id="081e2-103">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="081e2-103">Create RangeBorder</span></span>

> <span data-ttu-id="081e2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="081e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="081e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="081e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="081e2-106">Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="081e2-106">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="081e2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="081e2-107">Permissions</span></span>
<span data-ttu-id="081e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="081e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="081e2-110">Permission type</span></span>      | <span data-ttu-id="081e2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="081e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="081e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="081e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="081e2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="081e2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="081e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="081e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="081e2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="081e2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="081e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="081e2-116">Application</span></span> | <span data-ttu-id="081e2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="081e2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="081e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="081e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="081e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="081e2-119">Request headers</span></span>
| <span data-ttu-id="081e2-120">Name</span><span class="sxs-lookup"><span data-stu-id="081e2-120">Name</span></span>       | <span data-ttu-id="081e2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="081e2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="081e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="081e2-122">Authorization</span></span>  | <span data-ttu-id="081e2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="081e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="081e2-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="081e2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="081e2-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="081e2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="081e2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="081e2-128">Request body</span></span>
<span data-ttu-id="081e2-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [RangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="081e2-129">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="081e2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="081e2-130">Response</span></span>

<span data-ttu-id="081e2-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="081e2-131">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="081e2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="081e2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="081e2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="081e2-133">Request</span></span>
<span data-ttu-id="081e2-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="081e2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
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
<span data-ttu-id="081e2-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [RangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="081e2-135">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="081e2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="081e2-136">Response</span></span>
<span data-ttu-id="081e2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="081e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: 'NamedItem: Range'
description: Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.
ms.openlocfilehash: d446250b736ad8c5ac5eb65871eb024246813e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019901"
---
# <a name="nameditem-range"></a><span data-ttu-id="cd24c-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="cd24c-104">NamedItem: Range</span></span>

<span data-ttu-id="cd24c-p102">Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.</span><span class="sxs-lookup"><span data-stu-id="cd24c-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd24c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd24c-107">Permissions</span></span>
<span data-ttu-id="cd24c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd24c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd24c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd24c-110">Permission type</span></span>      | <span data-ttu-id="cd24c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd24c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd24c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd24c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd24c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd24c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd24c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd24c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd24c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd24c-115">Not supported.</span></span>    |
|<span data-ttu-id="cd24c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd24c-116">Application</span></span> | <span data-ttu-id="cd24c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd24c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd24c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd24c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="cd24c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd24c-119">Request headers</span></span>
| <span data-ttu-id="cd24c-120">Name</span><span class="sxs-lookup"><span data-stu-id="cd24c-120">Name</span></span>       | <span data-ttu-id="cd24c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd24c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd24c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd24c-122">Authorization</span></span>  | <span data-ttu-id="cd24c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd24c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd24c-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="cd24c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd24c-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="cd24c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd24c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd24c-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cd24c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd24c-129">Response</span></span>

<span data-ttu-id="cd24c-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd24c-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd24c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd24c-131">Example</span></span>
<span data-ttu-id="cd24c-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="cd24c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd24c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd24c-133">Request</span></span>
<span data-ttu-id="cd24c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd24c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```

##### <a name="response"></a><span data-ttu-id="cd24c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd24c-135">Response</span></span>
<span data-ttu-id="cd24c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd24c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
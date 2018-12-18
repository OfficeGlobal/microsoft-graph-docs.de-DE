---
title: 'Table: HeaderRowRange'
description: Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.
author: lumine2008
ms.openlocfilehash: 9abec04918f8944ebbafc238812e4f50c97a997f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336981"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="3b83f-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="3b83f-103">Table: HeaderRowRange</span></span>

> <span data-ttu-id="3b83f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b83f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b83f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b83f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b83f-106">Ruft das Bereichsobjekt ab, das mit der Kopfzeile der Tabelle verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="3b83f-106">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b83f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3b83f-107">Permissions</span></span>
<span data-ttu-id="3b83f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b83f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b83f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b83f-110">Permission type</span></span>      | <span data-ttu-id="3b83f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b83f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b83f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b83f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b83f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b83f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b83f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b83f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b83f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b83f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b83f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b83f-116">Application</span></span> | <span data-ttu-id="3b83f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b83f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b83f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b83f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="3b83f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b83f-119">Request headers</span></span>
| <span data-ttu-id="3b83f-120">Name</span><span class="sxs-lookup"><span data-stu-id="3b83f-120">Name</span></span>       | <span data-ttu-id="3b83f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b83f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b83f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b83f-122">Authorization</span></span>  | <span data-ttu-id="3b83f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b83f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b83f-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3b83f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b83f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3b83f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b83f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b83f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3b83f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b83f-129">Response</span></span>

<span data-ttu-id="3b83f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b83f-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b83f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b83f-131">Example</span></span>
<span data-ttu-id="3b83f-132">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3b83f-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3b83f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b83f-133">Request</span></span>
<span data-ttu-id="3b83f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b83f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="3b83f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b83f-135">Response</span></span>
<span data-ttu-id="3b83f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b83f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
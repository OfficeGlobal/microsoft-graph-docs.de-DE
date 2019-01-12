---
title: 'Table: convertToRange'
description: Wandelt die Tabelle in einen normalen Bereich von Zellen um. Alle Daten werden beibehalten.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f26306553ec731f9d946d1336937e5183a5b68a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979642"
---
# <a name="table-converttorange"></a><span data-ttu-id="9afc1-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="9afc1-104">Table: convertToRange</span></span>

> <span data-ttu-id="9afc1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9afc1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9afc1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9afc1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9afc1-p103">Wandelt die Tabelle in einen normalen Bereich von Zellen um. Alle Daten werden beibehalten.</span><span class="sxs-lookup"><span data-stu-id="9afc1-p103">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="9afc1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9afc1-109">Permissions</span></span>
<span data-ttu-id="9afc1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9afc1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9afc1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9afc1-112">Permission type</span></span>      | <span data-ttu-id="9afc1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9afc1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9afc1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9afc1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9afc1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9afc1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9afc1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9afc1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9afc1-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9afc1-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9afc1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9afc1-118">Application</span></span> | <span data-ttu-id="9afc1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9afc1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9afc1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9afc1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="9afc1-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9afc1-121">Request headers</span></span>
| <span data-ttu-id="9afc1-122">Name</span><span class="sxs-lookup"><span data-stu-id="9afc1-122">Name</span></span>       | <span data-ttu-id="9afc1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9afc1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9afc1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9afc1-124">Authorization</span></span>  | <span data-ttu-id="9afc1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9afc1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9afc1-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9afc1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="9afc1-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9afc1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9afc1-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9afc1-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9afc1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9afc1-131">Response</span></span>

<span data-ttu-id="9afc1-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9afc1-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9afc1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9afc1-133">Example</span></span>
<span data-ttu-id="9afc1-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9afc1-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9afc1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9afc1-135">Request</span></span>
<span data-ttu-id="9afc1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9afc1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="9afc1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9afc1-137">Response</span></span>
<span data-ttu-id="9afc1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9afc1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

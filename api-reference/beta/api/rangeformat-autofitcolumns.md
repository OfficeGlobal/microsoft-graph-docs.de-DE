---
title: 'RangeFormat: autofitColumns'
description: Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.
localization_priority: Normal
ms.openlocfilehash: 024475e606b6a94136e42eaa5dd2f32fcaf06b21
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872758"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="6a574-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="6a574-103">RangeFormat: autofitColumns</span></span>

> <span data-ttu-id="6a574-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a574-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a574-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a574-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a574-106">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="6a574-106">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a574-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a574-107">Permissions</span></span>
<span data-ttu-id="6a574-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a574-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a574-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a574-110">Permission type</span></span>      | <span data-ttu-id="6a574-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a574-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a574-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a574-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a574-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a574-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a574-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a574-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a574-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a574-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a574-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a574-116">Application</span></span> | <span data-ttu-id="6a574-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a574-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a574-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a574-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="6a574-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a574-119">Request headers</span></span>
| <span data-ttu-id="6a574-120">Name</span><span class="sxs-lookup"><span data-stu-id="6a574-120">Name</span></span>       | <span data-ttu-id="6a574-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a574-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a574-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a574-122">Authorization</span></span>  | <span data-ttu-id="6a574-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a574-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a574-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="6a574-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6a574-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="6a574-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a574-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a574-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6a574-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a574-129">Response</span></span>

<span data-ttu-id="6a574-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a574-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a574-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a574-132">Example</span></span>
<span data-ttu-id="6a574-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6a574-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6a574-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a574-134">Request</span></span>
<span data-ttu-id="6a574-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a574-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="6a574-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a574-136">Response</span></span>
<span data-ttu-id="6a574-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a574-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

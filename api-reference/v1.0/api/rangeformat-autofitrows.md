---
title: 'RangeFormat: autofitRows'
description: Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.
localization_priority: Normal
ms.openlocfilehash: 9bb515ef8f179392dc9214e0326e72c317e649ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840838"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="97714-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="97714-103">RangeFormat: autofitRows</span></span>

<span data-ttu-id="97714-104">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="97714-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="97714-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97714-105">Permissions</span></span>
<span data-ttu-id="97714-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97714-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97714-108">Permission type</span></span>      | <span data-ttu-id="97714-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97714-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97714-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97714-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97714-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97714-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97714-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97714-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97714-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97714-113">Not supported.</span></span>    |
|<span data-ttu-id="97714-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97714-114">Application</span></span> | <span data-ttu-id="97714-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97714-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97714-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97714-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="97714-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97714-117">Request headers</span></span>
| <span data-ttu-id="97714-118">Name</span><span class="sxs-lookup"><span data-stu-id="97714-118">Name</span></span>       | <span data-ttu-id="97714-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97714-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97714-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="97714-120">Authorization</span></span>  | <span data-ttu-id="97714-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97714-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97714-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="97714-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="97714-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="97714-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97714-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97714-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="97714-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="97714-127">Response</span></span>

<span data-ttu-id="97714-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97714-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97714-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97714-130">Example</span></span>
<span data-ttu-id="97714-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="97714-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="97714-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97714-132">Request</span></span>
<span data-ttu-id="97714-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97714-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="97714-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="97714-134">Response</span></span>
<span data-ttu-id="97714-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97714-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

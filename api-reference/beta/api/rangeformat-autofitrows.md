---
title: 'RangeFormat: autofitRows'
description: Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.
localization_priority: Normal
ms.openlocfilehash: 1a915a3af5a0d0300f957ebf27ef0415c0d00465
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894285"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="8c802-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="8c802-103">RangeFormat: autofitRows</span></span>

> <span data-ttu-id="8c802-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c802-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c802-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c802-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c802-106">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="8c802-106">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c802-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c802-107">Permissions</span></span>
<span data-ttu-id="8c802-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c802-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c802-110">Permission type</span></span>      | <span data-ttu-id="8c802-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c802-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c802-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c802-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c802-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c802-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c802-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c802-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c802-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c802-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c802-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c802-116">Application</span></span> | <span data-ttu-id="8c802-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c802-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c802-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c802-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="8c802-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c802-119">Request headers</span></span>
| <span data-ttu-id="8c802-120">Name</span><span class="sxs-lookup"><span data-stu-id="8c802-120">Name</span></span>       | <span data-ttu-id="8c802-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c802-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c802-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c802-122">Authorization</span></span>  | <span data-ttu-id="8c802-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c802-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c802-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8c802-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c802-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8c802-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c802-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c802-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8c802-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c802-129">Response</span></span>

<span data-ttu-id="8c802-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c802-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c802-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c802-132">Example</span></span>
<span data-ttu-id="8c802-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8c802-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c802-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c802-134">Request</span></span>
<span data-ttu-id="8c802-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c802-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="8c802-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c802-136">Response</span></span>
<span data-ttu-id="8c802-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8c802-137">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

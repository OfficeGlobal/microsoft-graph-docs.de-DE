---
title: 'RangeFormat: autofitRows'
description: Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.
ms.openlocfilehash: 428e405cad1464fad6e1e90940d9f9016fafdb48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060385"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="9d48a-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="9d48a-103">RangeFormat: autofitRows</span></span>

> <span data-ttu-id="9d48a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9d48a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d48a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d48a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d48a-106">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="9d48a-106">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d48a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d48a-107">Permissions</span></span>
<span data-ttu-id="9d48a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d48a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d48a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d48a-110">Permission type</span></span>      | <span data-ttu-id="9d48a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d48a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d48a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d48a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d48a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d48a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d48a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d48a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d48a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d48a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9d48a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d48a-116">Application</span></span> | <span data-ttu-id="9d48a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d48a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d48a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d48a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="9d48a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d48a-119">Request headers</span></span>
| <span data-ttu-id="9d48a-120">Name</span><span class="sxs-lookup"><span data-stu-id="9d48a-120">Name</span></span>       | <span data-ttu-id="9d48a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d48a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d48a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d48a-122">Authorization</span></span>  | <span data-ttu-id="9d48a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d48a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d48a-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9d48a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9d48a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9d48a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d48a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d48a-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9d48a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d48a-129">Response</span></span>

<span data-ttu-id="9d48a-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d48a-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d48a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d48a-132">Example</span></span>
<span data-ttu-id="9d48a-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9d48a-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d48a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d48a-134">Request</span></span>
<span data-ttu-id="9d48a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d48a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="9d48a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d48a-136">Response</span></span>
<span data-ttu-id="9d48a-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d48a-137">Here is an example of the response.</span></span> 
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
---
title: 'TableRow: delete'
description: Löscht die Zeile aus der Tabelle.
author: lumine2008
ms.openlocfilehash: ade0918ba9ad6fc23ff3becc33ba38024ee9894a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336918"
---
# <a name="tablerow-delete"></a><span data-ttu-id="09c21-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="09c21-103">TableRow: delete</span></span>

<span data-ttu-id="09c21-104">Löscht die Zeile aus der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="09c21-104">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="09c21-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09c21-105">Permissions</span></span>
<span data-ttu-id="09c21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09c21-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09c21-108">Permission type</span></span>      | <span data-ttu-id="09c21-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09c21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09c21-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09c21-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09c21-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09c21-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="09c21-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09c21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09c21-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09c21-113">Not supported.</span></span>    |
|<span data-ttu-id="09c21-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09c21-114">Application</span></span> | <span data-ttu-id="09c21-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09c21-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09c21-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09c21-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="09c21-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09c21-117">Request headers</span></span>
| <span data-ttu-id="09c21-118">Name</span><span class="sxs-lookup"><span data-stu-id="09c21-118">Name</span></span>       | <span data-ttu-id="09c21-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09c21-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="09c21-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="09c21-120">Authorization</span></span>  | <span data-ttu-id="09c21-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09c21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09c21-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="09c21-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="09c21-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="09c21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09c21-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09c21-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="09c21-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="09c21-127">Response</span></span>

<span data-ttu-id="09c21-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09c21-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c21-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09c21-130">Example</span></span>
<span data-ttu-id="09c21-131">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="09c21-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09c21-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09c21-132">Request</span></span>
<span data-ttu-id="09c21-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09c21-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="09c21-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="09c21-134">Response</span></span>
<span data-ttu-id="09c21-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09c21-135">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
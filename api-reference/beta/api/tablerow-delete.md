---
title: 'TableRow: delete'
description: Löscht die Zeile aus der Tabelle.
ms.openlocfilehash: a2202daf9a645a16a7ea6287edf468e12d829e9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063665"
---
# <a name="tablerow-delete"></a><span data-ttu-id="3c0bb-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="3c0bb-103">TableRow: delete</span></span>

> <span data-ttu-id="3c0bb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c0bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c0bb-106">Löscht die Zeile aus der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-106">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c0bb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3c0bb-107">Permissions</span></span>
<span data-ttu-id="3c0bb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c0bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c0bb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c0bb-110">Permission type</span></span>      | <span data-ttu-id="3c0bb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c0bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c0bb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c0bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c0bb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c0bb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c0bb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c0bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c0bb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c0bb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c0bb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-116">Application</span></span> | <span data-ttu-id="3c0bb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c0bb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c0bb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="3c0bb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c0bb-119">Request headers</span></span>
| <span data-ttu-id="3c0bb-120">Name</span><span class="sxs-lookup"><span data-stu-id="3c0bb-120">Name</span></span>       | <span data-ttu-id="3c0bb-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3c0bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c0bb-122">Authorization</span></span>  | <span data-ttu-id="3c0bb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c0bb-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3c0bb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3c0bb-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0bb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c0bb-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3c0bb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c0bb-129">Response</span></span>

<span data-ttu-id="3c0bb-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c0bb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c0bb-132">Example</span></span>
<span data-ttu-id="3c0bb-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3c0bb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-134">Request</span></span>
<span data-ttu-id="3c0bb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="3c0bb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c0bb-136">Response</span></span>
<span data-ttu-id="3c0bb-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-137">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
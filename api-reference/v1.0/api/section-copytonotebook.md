---
title: 'section: copyToNotebook'
description: Kopiert einen Abschnitt in ein bestimmtes Notizbuch.
ms.openlocfilehash: 365e4745f01c3d011cbf8cf0186a16b5eb580c5b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018540"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="f9ea2-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="f9ea2-103">section: copyToNotebook</span></span>
<span data-ttu-id="f9ea2-104">Kopiert einen Abschnitt in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="f9ea2-105">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9ea2-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9ea2-106">Permissions</span></span>
<span data-ttu-id="f9ea2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ea2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9ea2-109">Permission type</span></span>      | <span data-ttu-id="f9ea2-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9ea2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ea2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9ea2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ea2-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ea2-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9ea2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9ea2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ea2-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9ea2-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f9ea2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9ea2-115">Application</span></span> | <span data-ttu-id="f9ea2-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ea2-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ea2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9ea2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="f9ea2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9ea2-118">Request headers</span></span>
| <span data-ttu-id="f9ea2-119">Name</span><span class="sxs-lookup"><span data-stu-id="f9ea2-119">Name</span></span>       | <span data-ttu-id="f9ea2-120">Typ</span><span class="sxs-lookup"><span data-stu-id="f9ea2-120">Type</span></span> | <span data-ttu-id="f9ea2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ea2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9ea2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ea2-122">Authorization</span></span>  | <span data-ttu-id="f9ea2-123">string</span><span class="sxs-lookup"><span data-stu-id="f9ea2-123">string</span></span>  | <span data-ttu-id="f9ea2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9ea2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9ea2-126">Content-Type</span></span> | <span data-ttu-id="f9ea2-127">string</span><span class="sxs-lookup"><span data-stu-id="f9ea2-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f9ea2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9ea2-128">Request body</span></span>
<span data-ttu-id="f9ea2-129">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="f9ea2-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="f9ea2-130">Parameter</span></span>    | <span data-ttu-id="f9ea2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f9ea2-131">Type</span></span>   |<span data-ttu-id="f9ea2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9ea2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9ea2-133">groupId</span><span class="sxs-lookup"><span data-stu-id="f9ea2-133">groupId</span></span>|<span data-ttu-id="f9ea2-134">String</span><span class="sxs-lookup"><span data-stu-id="f9ea2-134">String</span></span>|<span data-ttu-id="f9ea2-p103">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="f9ea2-137">id</span><span class="sxs-lookup"><span data-stu-id="f9ea2-137">id</span></span>|<span data-ttu-id="f9ea2-138">String</span><span class="sxs-lookup"><span data-stu-id="f9ea2-138">String</span></span>|<span data-ttu-id="f9ea2-p104">Erforderlich. Die ID des Zielnotizbuchs.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p104">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="f9ea2-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="f9ea2-141">renameAs</span></span>|<span data-ttu-id="f9ea2-142">String</span><span class="sxs-lookup"><span data-stu-id="f9ea2-142">String</span></span>|<span data-ttu-id="f9ea2-p105">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="f9ea2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9ea2-145">Response</span></span>

<span data-ttu-id="f9ea2-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="f9ea2-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="f9ea2-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9ea2-148">Example</span></span>
<span data-ttu-id="f9ea2-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9ea2-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9ea2-150">Request</span></span>
<span data-ttu-id="f9ea2-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="f9ea2-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9ea2-152">Response</span></span>
<span data-ttu-id="f9ea2-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9ea2-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
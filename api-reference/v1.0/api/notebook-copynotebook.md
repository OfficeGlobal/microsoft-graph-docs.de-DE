---
title: 'notebook: copyNotebook'
description: Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.
localization_priority: Normal
ms.openlocfilehash: 927cdd95a1cf39b27ac18faeeae11ccc56cfff6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812768"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="4cbcb-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="4cbcb-104">notebook: copyNotebook</span></span>
<span data-ttu-id="4cbcb-p102">Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="4cbcb-107">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cbcb-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4cbcb-108">Permissions</span></span>
<span data-ttu-id="4cbcb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cbcb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cbcb-111">Permission type</span></span>      | <span data-ttu-id="4cbcb-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cbcb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cbcb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cbcb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4cbcb-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbcb-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cbcb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cbcb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cbcb-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cbcb-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4cbcb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cbcb-117">Application</span></span> | <span data-ttu-id="4cbcb-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbcb-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cbcb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cbcb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="4cbcb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cbcb-120">Request headers</span></span>
| <span data-ttu-id="4cbcb-121">Name</span><span class="sxs-lookup"><span data-stu-id="4cbcb-121">Name</span></span>       | <span data-ttu-id="4cbcb-122">Typ</span><span class="sxs-lookup"><span data-stu-id="4cbcb-122">Type</span></span> | <span data-ttu-id="4cbcb-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cbcb-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4cbcb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cbcb-124">Authorization</span></span>  | <span data-ttu-id="4cbcb-125">string</span><span class="sxs-lookup"><span data-stu-id="4cbcb-125">string</span></span>  | <span data-ttu-id="4cbcb-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cbcb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cbcb-128">Content-Type</span></span> | <span data-ttu-id="4cbcb-129">string</span><span class="sxs-lookup"><span data-stu-id="4cbcb-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4cbcb-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cbcb-130">Request body</span></span>
<span data-ttu-id="4cbcb-p105">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt. Es ist in Ordnung, senden Sie einen leeren Text senden, wenn keine erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="4cbcb-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="4cbcb-133">Parameter</span></span>    | <span data-ttu-id="4cbcb-134">Typ</span><span class="sxs-lookup"><span data-stu-id="4cbcb-134">Type</span></span>   |<span data-ttu-id="4cbcb-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cbcb-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cbcb-136">groupId</span><span class="sxs-lookup"><span data-stu-id="4cbcb-136">groupId</span></span>|<span data-ttu-id="4cbcb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cbcb-137">String</span></span>|<span data-ttu-id="4cbcb-p106">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="4cbcb-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="4cbcb-140">renameAs</span></span>|<span data-ttu-id="4cbcb-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cbcb-141">String</span></span>|<span data-ttu-id="4cbcb-p107">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="4cbcb-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cbcb-144">Response</span></span>

<span data-ttu-id="4cbcb-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="4cbcb-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="4cbcb-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cbcb-147">Example</span></span>
<span data-ttu-id="4cbcb-148">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4cbcb-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cbcb-149">Request</span></span>
<span data-ttu-id="4cbcb-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="4cbcb-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cbcb-151">Response</span></span>
<span data-ttu-id="4cbcb-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4cbcb-152">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: 'notebook: copyNotebook'
description: Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.
localization_priority: Normal
ms.openlocfilehash: ba9ed886ab0102a3ed66c31efbc420832e67d316
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833054"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="e6c19-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="e6c19-104">notebook: copyNotebook</span></span>

> <span data-ttu-id="e6c19-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e6c19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c19-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6c19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6c19-p103">Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="e6c19-p103">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="e6c19-109">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="e6c19-109">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6c19-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6c19-110">Permissions</span></span>
<span data-ttu-id="e6c19-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c19-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c19-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6c19-113">Permission type</span></span>      | <span data-ttu-id="e6c19-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6c19-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c19-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6c19-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c19-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c19-116">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e6c19-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6c19-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c19-118">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6c19-118">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e6c19-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6c19-119">Application</span></span> | <span data-ttu-id="e6c19-120">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c19-120">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c19-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6c19-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="e6c19-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6c19-122">Request headers</span></span>
| <span data-ttu-id="e6c19-123">Name</span><span class="sxs-lookup"><span data-stu-id="e6c19-123">Name</span></span>       | <span data-ttu-id="e6c19-124">Typ</span><span class="sxs-lookup"><span data-stu-id="e6c19-124">Type</span></span> | <span data-ttu-id="e6c19-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6c19-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6c19-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6c19-126">Authorization</span></span>  | <span data-ttu-id="e6c19-127">string</span><span class="sxs-lookup"><span data-stu-id="e6c19-127">string</span></span>  | <span data-ttu-id="e6c19-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6c19-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6c19-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6c19-130">Content-Type</span></span> | <span data-ttu-id="e6c19-131">string</span><span class="sxs-lookup"><span data-stu-id="e6c19-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e6c19-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6c19-132">Request body</span></span>
<span data-ttu-id="e6c19-p106">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt. Es ist in Ordnung, senden Sie einen leeren Text senden, wenn keine erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e6c19-p106">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="e6c19-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="e6c19-135">Parameter</span></span>    | <span data-ttu-id="e6c19-136">Typ</span><span class="sxs-lookup"><span data-stu-id="e6c19-136">Type</span></span>   |<span data-ttu-id="e6c19-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6c19-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6c19-138">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="e6c19-138">siteCollectionId</span></span>|<span data-ttu-id="e6c19-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6c19-139">String</span></span>|<span data-ttu-id="e6c19-140">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="e6c19-140">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="e6c19-141">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="e6c19-141">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="e6c19-142">siteId</span><span class="sxs-lookup"><span data-stu-id="e6c19-142">siteId</span></span>|<span data-ttu-id="e6c19-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6c19-143">String</span></span>|<span data-ttu-id="e6c19-144">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="e6c19-144">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="e6c19-145">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="e6c19-145">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="e6c19-146">groupId</span><span class="sxs-lookup"><span data-stu-id="e6c19-146">groupId</span></span>|<span data-ttu-id="e6c19-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6c19-147">String</span></span>|<span data-ttu-id="e6c19-p109">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e6c19-p109">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="e6c19-150">renameAs</span><span class="sxs-lookup"><span data-stu-id="e6c19-150">renameAs</span></span>|<span data-ttu-id="e6c19-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6c19-151">String</span></span>|<span data-ttu-id="e6c19-p110">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="e6c19-p110">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="e6c19-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6c19-154">Response</span></span>

<span data-ttu-id="e6c19-p111">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="e6c19-p111">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="e6c19-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6c19-157">Example</span></span>
<span data-ttu-id="e6c19-158">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e6c19-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6c19-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6c19-159">Request</span></span>
<span data-ttu-id="e6c19-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6c19-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="e6c19-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6c19-161">Response</span></span>
<span data-ttu-id="e6c19-162">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6c19-162">Here is an example of the response.</span></span>
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

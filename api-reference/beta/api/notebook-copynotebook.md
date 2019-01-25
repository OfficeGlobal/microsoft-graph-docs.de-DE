---
title: 'notebook: copyNotebook'
description: Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7100d768fb411aeab8ccbd0622de26aeae8a7133
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515601"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="1b753-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="1b753-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b753-p102">Kopiert ein Notizbuch in den Ordner „Notizbücher“ in der Dokumentzielbibliothek. Der Ordner wird erstellt, falls er nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="1b753-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="1b753-107">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="1b753-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b753-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1b753-108">Permissions</span></span>
<span data-ttu-id="1b753-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b753-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b753-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b753-111">Permission type</span></span>      | <span data-ttu-id="1b753-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b753-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b753-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b753-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1b753-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b753-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b753-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b753-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b753-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b753-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1b753-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b753-117">Application</span></span> | <span data-ttu-id="1b753-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b753-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b753-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b753-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="1b753-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b753-120">Request headers</span></span>
| <span data-ttu-id="1b753-121">Name</span><span class="sxs-lookup"><span data-stu-id="1b753-121">Name</span></span>       | <span data-ttu-id="1b753-122">Typ</span><span class="sxs-lookup"><span data-stu-id="1b753-122">Type</span></span> | <span data-ttu-id="1b753-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b753-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b753-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b753-124">Authorization</span></span>  | <span data-ttu-id="1b753-125">string</span><span class="sxs-lookup"><span data-stu-id="1b753-125">string</span></span>  | <span data-ttu-id="1b753-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b753-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b753-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b753-128">Content-Type</span></span> | <span data-ttu-id="1b753-129">string</span><span class="sxs-lookup"><span data-stu-id="1b753-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1b753-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b753-130">Request body</span></span>
<span data-ttu-id="1b753-p105">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt. Es ist in Ordnung, senden Sie einen leeren Text senden, wenn keine erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1b753-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="1b753-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="1b753-133">Parameter</span></span>    | <span data-ttu-id="1b753-134">Typ</span><span class="sxs-lookup"><span data-stu-id="1b753-134">Type</span></span>   |<span data-ttu-id="1b753-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b753-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b753-136">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="1b753-136">siteCollectionId</span></span>|<span data-ttu-id="1b753-137">String</span><span class="sxs-lookup"><span data-stu-id="1b753-137">String</span></span>|<span data-ttu-id="1b753-138">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1b753-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="1b753-139">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1b753-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="1b753-140">siteId</span><span class="sxs-lookup"><span data-stu-id="1b753-140">siteId</span></span>|<span data-ttu-id="1b753-141">String</span><span class="sxs-lookup"><span data-stu-id="1b753-141">String</span></span>|<span data-ttu-id="1b753-142">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1b753-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="1b753-143">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="1b753-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="1b753-144">groupId</span><span class="sxs-lookup"><span data-stu-id="1b753-144">groupId</span></span>|<span data-ttu-id="1b753-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b753-145">String</span></span>|<span data-ttu-id="1b753-p108">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1b753-p108">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="1b753-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="1b753-148">renameAs</span></span>|<span data-ttu-id="1b753-149">String</span><span class="sxs-lookup"><span data-stu-id="1b753-149">String</span></span>|<span data-ttu-id="1b753-p109">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="1b753-p109">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="1b753-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b753-152">Response</span></span>

<span data-ttu-id="1b753-p110">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="1b753-p110">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="1b753-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b753-155">Example</span></span>
<span data-ttu-id="1b753-156">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1b753-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b753-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b753-157">Request</span></span>
<span data-ttu-id="1b753-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b753-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1b753-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b753-159">Response</span></span>
<span data-ttu-id="1b753-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1b753-160">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

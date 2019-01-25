---
title: 'section: copyToNotebook'
description: Kopiert einen Abschnitt in ein bestimmtes Notizbuch.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523323"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="ee305-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="ee305-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee305-104">Kopiert einen Abschnitt in ein bestimmtes Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="ee305-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="ee305-105">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="ee305-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee305-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee305-106">Permissions</span></span>
<span data-ttu-id="ee305-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee305-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee305-109">Permission type</span></span>      | <span data-ttu-id="ee305-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee305-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee305-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee305-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee305-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee305-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee305-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee305-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee305-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee305-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ee305-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee305-115">Application</span></span> | <span data-ttu-id="ee305-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee305-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee305-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee305-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="ee305-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee305-118">Request headers</span></span>
| <span data-ttu-id="ee305-119">Name</span><span class="sxs-lookup"><span data-stu-id="ee305-119">Name</span></span>       | <span data-ttu-id="ee305-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ee305-120">Type</span></span> | <span data-ttu-id="ee305-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee305-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee305-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee305-122">Authorization</span></span>  | <span data-ttu-id="ee305-123">string</span><span class="sxs-lookup"><span data-stu-id="ee305-123">string</span></span>  | <span data-ttu-id="ee305-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee305-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee305-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee305-126">Content-Type</span></span> | <span data-ttu-id="ee305-127">string</span><span class="sxs-lookup"><span data-stu-id="ee305-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ee305-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee305-128">Request body</span></span>
<span data-ttu-id="ee305-129">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="ee305-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ee305-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="ee305-130">Parameter</span></span>    | <span data-ttu-id="ee305-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ee305-131">Type</span></span>   |<span data-ttu-id="ee305-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee305-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee305-133">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="ee305-133">siteCollectionId</span></span>|<span data-ttu-id="ee305-134">String</span><span class="sxs-lookup"><span data-stu-id="ee305-134">String</span></span>|<span data-ttu-id="ee305-135">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="ee305-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="ee305-136">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="ee305-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ee305-137">siteId</span><span class="sxs-lookup"><span data-stu-id="ee305-137">siteId</span></span>|<span data-ttu-id="ee305-138">String</span><span class="sxs-lookup"><span data-stu-id="ee305-138">String</span></span>|<span data-ttu-id="ee305-139">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="ee305-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="ee305-140">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="ee305-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="ee305-141">groupId</span><span class="sxs-lookup"><span data-stu-id="ee305-141">groupId</span></span>|<span data-ttu-id="ee305-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee305-142">String</span></span>|<span data-ttu-id="ee305-p105">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ee305-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ee305-145">id</span><span class="sxs-lookup"><span data-stu-id="ee305-145">id</span></span>|<span data-ttu-id="ee305-146">String</span><span class="sxs-lookup"><span data-stu-id="ee305-146">String</span></span>|<span data-ttu-id="ee305-p106">Erforderlich. Die ID des Zielnotizbuchs.</span><span class="sxs-lookup"><span data-stu-id="ee305-p106">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="ee305-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="ee305-149">renameAs</span></span>|<span data-ttu-id="ee305-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee305-150">String</span></span>|<span data-ttu-id="ee305-p107">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="ee305-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="ee305-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee305-153">Response</span></span>

<span data-ttu-id="ee305-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="ee305-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ee305-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee305-156">Example</span></span>
<span data-ttu-id="ee305-157">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ee305-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee305-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee305-158">Request</span></span>
<span data-ttu-id="ee305-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee305-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="ee305-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee305-160">Response</span></span>
<span data-ttu-id="ee305-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee305-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytonotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

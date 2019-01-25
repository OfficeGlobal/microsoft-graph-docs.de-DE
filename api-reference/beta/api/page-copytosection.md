---
title: 'page: copyToSection'
description: Kopiert eine Seite in einen bestimmten Abschnitt.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dd7abb016345195bd5a32e20a5623d6fca9fd6ff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516441"
---
# <a name="page-copytosection"></a><span data-ttu-id="25062-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="25062-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25062-104">Kopiert eine Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="25062-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="25062-105">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="25062-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="25062-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25062-106">Permissions</span></span>
<span data-ttu-id="25062-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25062-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25062-109">Permission type</span></span>      | <span data-ttu-id="25062-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25062-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25062-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25062-111">Delegated (work or school account)</span></span> | <span data-ttu-id="25062-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25062-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="25062-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25062-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25062-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25062-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="25062-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25062-115">Application</span></span> | <span data-ttu-id="25062-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25062-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25062-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25062-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="25062-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25062-118">Request headers</span></span>
| <span data-ttu-id="25062-119">Name</span><span class="sxs-lookup"><span data-stu-id="25062-119">Name</span></span>       | <span data-ttu-id="25062-120">Typ</span><span class="sxs-lookup"><span data-stu-id="25062-120">Type</span></span> | <span data-ttu-id="25062-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25062-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25062-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25062-122">Authorization</span></span>  | <span data-ttu-id="25062-123">string</span><span class="sxs-lookup"><span data-stu-id="25062-123">string</span></span>  | <span data-ttu-id="25062-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25062-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25062-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25062-126">Content-Type</span></span> | <span data-ttu-id="25062-127">string</span><span class="sxs-lookup"><span data-stu-id="25062-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="25062-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25062-128">Request body</span></span>
<span data-ttu-id="25062-129">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="25062-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="25062-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="25062-130">Parameter</span></span>    | <span data-ttu-id="25062-131">Typ</span><span class="sxs-lookup"><span data-stu-id="25062-131">Type</span></span>   |<span data-ttu-id="25062-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25062-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25062-133">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="25062-133">siteCollectionId</span></span>|<span data-ttu-id="25062-134">String</span><span class="sxs-lookup"><span data-stu-id="25062-134">String</span></span>|<span data-ttu-id="25062-135">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="25062-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="25062-136">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="25062-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="25062-137">siteId</span><span class="sxs-lookup"><span data-stu-id="25062-137">siteId</span></span>|<span data-ttu-id="25062-138">String</span><span class="sxs-lookup"><span data-stu-id="25062-138">String</span></span>|<span data-ttu-id="25062-139">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="25062-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="25062-140">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="25062-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="25062-141">groupId</span><span class="sxs-lookup"><span data-stu-id="25062-141">groupId</span></span>|<span data-ttu-id="25062-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="25062-142">String</span></span>|<span data-ttu-id="25062-p105">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="25062-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="25062-145">id</span><span class="sxs-lookup"><span data-stu-id="25062-145">id</span></span>|<span data-ttu-id="25062-146">String</span><span class="sxs-lookup"><span data-stu-id="25062-146">String</span></span>|<span data-ttu-id="25062-p106">Erforderlich. Die ID des Zielabschnitts.</span><span class="sxs-lookup"><span data-stu-id="25062-p106">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="25062-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="25062-149">Response</span></span>

<span data-ttu-id="25062-p107">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="25062-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="25062-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25062-152">Example</span></span>
<span data-ttu-id="25062-153">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="25062-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25062-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25062-154">Request</span></span>
<span data-ttu-id="25062-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25062-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="25062-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="25062-156">Response</span></span>
<span data-ttu-id="25062-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="25062-157">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

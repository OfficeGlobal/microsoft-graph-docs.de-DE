---
title: 'page: copyToSection'
description: Kopiert eine Seite in einen bestimmten Abschnitt.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 733f03bd04df31b79e84a7f8bbf5162ec1b023ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915200"
---
# <a name="page-copytosection"></a><span data-ttu-id="93eeb-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="93eeb-103">page: copyToSection</span></span>

> <span data-ttu-id="93eeb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93eeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93eeb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93eeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93eeb-106">Kopiert eine Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="93eeb-106">Copies a page to a specific section.</span></span>

<span data-ttu-id="93eeb-107">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="93eeb-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="93eeb-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="93eeb-108">Permissions</span></span>
<span data-ttu-id="93eeb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93eeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93eeb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93eeb-111">Permission type</span></span>      | <span data-ttu-id="93eeb-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93eeb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93eeb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93eeb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="93eeb-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93eeb-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="93eeb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93eeb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93eeb-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="93eeb-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="93eeb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93eeb-117">Application</span></span> | <span data-ttu-id="93eeb-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93eeb-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93eeb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93eeb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="93eeb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93eeb-120">Request headers</span></span>
| <span data-ttu-id="93eeb-121">Name</span><span class="sxs-lookup"><span data-stu-id="93eeb-121">Name</span></span>       | <span data-ttu-id="93eeb-122">Typ</span><span class="sxs-lookup"><span data-stu-id="93eeb-122">Type</span></span> | <span data-ttu-id="93eeb-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93eeb-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93eeb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="93eeb-124">Authorization</span></span>  | <span data-ttu-id="93eeb-125">string</span><span class="sxs-lookup"><span data-stu-id="93eeb-125">string</span></span>  | <span data-ttu-id="93eeb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93eeb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93eeb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93eeb-128">Content-Type</span></span> | <span data-ttu-id="93eeb-129">string</span><span class="sxs-lookup"><span data-stu-id="93eeb-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="93eeb-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93eeb-130">Request body</span></span>
<span data-ttu-id="93eeb-131">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="93eeb-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="93eeb-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="93eeb-132">Parameter</span></span>    | <span data-ttu-id="93eeb-133">Typ</span><span class="sxs-lookup"><span data-stu-id="93eeb-133">Type</span></span>   |<span data-ttu-id="93eeb-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93eeb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93eeb-135">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="93eeb-135">siteCollectionId</span></span>|<span data-ttu-id="93eeb-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93eeb-136">String</span></span>|<span data-ttu-id="93eeb-137">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="93eeb-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="93eeb-138">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="93eeb-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="93eeb-139">siteId</span><span class="sxs-lookup"><span data-stu-id="93eeb-139">siteId</span></span>|<span data-ttu-id="93eeb-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93eeb-140">String</span></span>|<span data-ttu-id="93eeb-141">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="93eeb-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="93eeb-142">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="93eeb-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="93eeb-143">groupId</span><span class="sxs-lookup"><span data-stu-id="93eeb-143">groupId</span></span>|<span data-ttu-id="93eeb-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93eeb-144">String</span></span>|<span data-ttu-id="93eeb-p106">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="93eeb-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="93eeb-147">id</span><span class="sxs-lookup"><span data-stu-id="93eeb-147">id</span></span>|<span data-ttu-id="93eeb-148">String</span><span class="sxs-lookup"><span data-stu-id="93eeb-148">String</span></span>|<span data-ttu-id="93eeb-p107">Erforderlich. Die ID des Zielabschnitts.</span><span class="sxs-lookup"><span data-stu-id="93eeb-p107">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="93eeb-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="93eeb-151">Response</span></span>

<span data-ttu-id="93eeb-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="93eeb-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="93eeb-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93eeb-154">Example</span></span>
<span data-ttu-id="93eeb-155">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="93eeb-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="93eeb-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93eeb-156">Request</span></span>
<span data-ttu-id="93eeb-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93eeb-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="93eeb-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="93eeb-158">Response</span></span>
<span data-ttu-id="93eeb-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93eeb-159">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

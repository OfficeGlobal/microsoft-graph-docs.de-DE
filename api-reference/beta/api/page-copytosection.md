---
title: 'page: copyToSection'
description: Kopiert eine Seite in einen bestimmten Abschnitt.
localization_priority: Normal
ms.openlocfilehash: 10d0eecd2f84a33e66209f8297b72b8a4630b100
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892505"
---
# <a name="page-copytosection"></a><span data-ttu-id="34281-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="34281-103">page: copyToSection</span></span>

> <span data-ttu-id="34281-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34281-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34281-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34281-106">Kopiert eine Seite in einen bestimmten Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="34281-106">Copies a page to a specific section.</span></span>

<span data-ttu-id="34281-107">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="34281-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="34281-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34281-108">Permissions</span></span>
<span data-ttu-id="34281-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34281-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34281-111">Permission type</span></span>      | <span data-ttu-id="34281-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34281-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34281-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34281-113">Delegated (work or school account)</span></span> | <span data-ttu-id="34281-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34281-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="34281-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34281-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34281-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34281-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="34281-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34281-117">Application</span></span> | <span data-ttu-id="34281-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34281-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34281-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34281-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="34281-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34281-120">Request headers</span></span>
| <span data-ttu-id="34281-121">Name</span><span class="sxs-lookup"><span data-stu-id="34281-121">Name</span></span>       | <span data-ttu-id="34281-122">Typ</span><span class="sxs-lookup"><span data-stu-id="34281-122">Type</span></span> | <span data-ttu-id="34281-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34281-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34281-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34281-124">Authorization</span></span>  | <span data-ttu-id="34281-125">string</span><span class="sxs-lookup"><span data-stu-id="34281-125">string</span></span>  | <span data-ttu-id="34281-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34281-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34281-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34281-128">Content-Type</span></span> | <span data-ttu-id="34281-129">string</span><span class="sxs-lookup"><span data-stu-id="34281-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="34281-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34281-130">Request body</span></span>
<span data-ttu-id="34281-131">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="34281-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="34281-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="34281-132">Parameter</span></span>    | <span data-ttu-id="34281-133">Typ</span><span class="sxs-lookup"><span data-stu-id="34281-133">Type</span></span>   |<span data-ttu-id="34281-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34281-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34281-135">siteSammlungId</span><span class="sxs-lookup"><span data-stu-id="34281-135">siteCollectionId</span></span>|<span data-ttu-id="34281-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34281-136">String</span></span>|<span data-ttu-id="34281-137">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="34281-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="34281-138">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="34281-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="34281-139">siteId</span><span class="sxs-lookup"><span data-stu-id="34281-139">siteId</span></span>|<span data-ttu-id="34281-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34281-140">String</span></span>|<span data-ttu-id="34281-141">Die Id der SharePoint-Website zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="34281-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="34281-142">Verwenden Sie nur, wenn für ein Office 365-Teamwebsite zu kopieren.</span><span class="sxs-lookup"><span data-stu-id="34281-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="34281-143">groupId</span><span class="sxs-lookup"><span data-stu-id="34281-143">groupId</span></span>|<span data-ttu-id="34281-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34281-144">String</span></span>|<span data-ttu-id="34281-p106">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="34281-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="34281-147">id</span><span class="sxs-lookup"><span data-stu-id="34281-147">id</span></span>|<span data-ttu-id="34281-148">String</span><span class="sxs-lookup"><span data-stu-id="34281-148">String</span></span>|<span data-ttu-id="34281-p107">Erforderlich. Die ID des Zielabschnitts.</span><span class="sxs-lookup"><span data-stu-id="34281-p107">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="34281-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="34281-151">Response</span></span>

<span data-ttu-id="34281-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="34281-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="34281-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34281-154">Example</span></span>
<span data-ttu-id="34281-155">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="34281-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34281-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34281-156">Request</span></span>
<span data-ttu-id="34281-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34281-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="34281-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="34281-158">Response</span></span>
<span data-ttu-id="34281-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34281-159">Here is an example of the response.</span></span>
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

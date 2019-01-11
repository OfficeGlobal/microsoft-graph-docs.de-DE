---
title: 'section: copyToSectionGroup'
description: Kopiert einen Abschnitt in eine bestimmte Abschnittsgruppe.
localization_priority: Normal
ms.openlocfilehash: 671cd28db66517b0b04d8b9d99cc1dccba17206e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846571"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="ae9a4-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="ae9a4-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="ae9a4-104">Kopiert einen Abschnitt in eine bestimmte Abschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="ae9a4-105">Für Kopiervorgänge gilt ein asynchrones Aufrufmuster:  Rufen Sie zunächst die Kopieraktion auf, und fragen Sie dann den Vorgangsendpunkt nach dem Ergebnis ab.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae9a4-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae9a4-106">Permissions</span></span>
<span data-ttu-id="ae9a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae9a4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae9a4-109">Permission type</span></span>      | <span data-ttu-id="ae9a4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae9a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae9a4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae9a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae9a4-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae9a4-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae9a4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae9a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae9a4-114">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae9a4-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ae9a4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae9a4-115">Application</span></span> | <span data-ttu-id="ae9a4-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae9a4-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae9a4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="ae9a4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae9a4-118">Request headers</span></span>
| <span data-ttu-id="ae9a4-119">Name</span><span class="sxs-lookup"><span data-stu-id="ae9a4-119">Name</span></span>       | <span data-ttu-id="ae9a4-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ae9a4-120">Type</span></span> | <span data-ttu-id="ae9a4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae9a4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae9a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae9a4-122">Authorization</span></span>  | <span data-ttu-id="ae9a4-123">string</span><span class="sxs-lookup"><span data-stu-id="ae9a4-123">string</span></span>  | <span data-ttu-id="ae9a4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae9a4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae9a4-126">Content-Type</span></span> | <span data-ttu-id="ae9a4-127">string</span><span class="sxs-lookup"><span data-stu-id="ae9a4-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ae9a4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae9a4-128">Request body</span></span>
<span data-ttu-id="ae9a4-129">Geben Sie im Anforderungstext ein JSON-Objekt an, das die vom Vorgang benötigten Parameter bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="ae9a4-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="ae9a4-130">Parameter</span></span>    | <span data-ttu-id="ae9a4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ae9a4-131">Type</span></span>   |<span data-ttu-id="ae9a4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae9a4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae9a4-133">groupId</span><span class="sxs-lookup"><span data-stu-id="ae9a4-133">groupId</span></span>|<span data-ttu-id="ae9a4-134">String</span><span class="sxs-lookup"><span data-stu-id="ae9a4-134">String</span></span>|<span data-ttu-id="ae9a4-p103">Die ID der Gruppe, in die kopiert werden soll. Verwenden Sie diesen Parameter nur beim Kopieren in eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="ae9a4-137">id</span><span class="sxs-lookup"><span data-stu-id="ae9a4-137">id</span></span>|<span data-ttu-id="ae9a4-138">String</span><span class="sxs-lookup"><span data-stu-id="ae9a4-138">String</span></span>|<span data-ttu-id="ae9a4-p104">Erforderlich. Die ID der Zielabschnittsgruppe.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="ae9a4-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="ae9a4-141">renameAs</span></span>|<span data-ttu-id="ae9a4-142">String</span><span class="sxs-lookup"><span data-stu-id="ae9a4-142">String</span></span>|<span data-ttu-id="ae9a4-p105">Der Name der Kopie. Standardmäßig der Name des vorhandenen Elements.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="ae9a4-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9a4-145">Response</span></span>

<span data-ttu-id="ae9a4-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `202 Accepted` und der Header `Operation-Location` zurückgegeben. Fragen Sie den Operation-Location-Endpunkt ab, um [den Status des Kopiervorgangs abzurufen](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="ae9a4-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="ae9a4-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae9a4-148">Example</span></span>
<span data-ttu-id="ae9a4-149">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae9a4-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae9a4-150">Request</span></span>
<span data-ttu-id="ae9a4-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="ae9a4-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae9a4-152">Response</span></span>
<span data-ttu-id="ae9a4-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ae9a4-153">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

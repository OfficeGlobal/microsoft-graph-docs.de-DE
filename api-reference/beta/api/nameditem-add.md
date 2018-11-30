---
title: Benanntes Element hinzufügen
description: Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.
ms.openlocfilehash: 1592ec4706b4a73f24f6205aaedd29df15725355
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065030"
---
# <a name="add-named-item"></a><span data-ttu-id="70c3f-103">Benanntes Element hinzufügen</span><span class="sxs-lookup"><span data-stu-id="70c3f-103">Add Named Item</span></span>

> <span data-ttu-id="70c3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="70c3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70c3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70c3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70c3f-106">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="70c3f-106">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="70c3f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="70c3f-107">Permissions</span></span>
<span data-ttu-id="70c3f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c3f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70c3f-110">Permission type</span></span>      | <span data-ttu-id="70c3f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70c3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70c3f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70c3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70c3f-113">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c3f-113">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="70c3f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70c3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70c3f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70c3f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70c3f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70c3f-116">Application</span></span> | <span data-ttu-id="70c3f-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="70c3f-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70c3f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="70c3f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70c3f-119">Request headers</span></span>
| <span data-ttu-id="70c3f-120">Name</span><span class="sxs-lookup"><span data-stu-id="70c3f-120">Name</span></span>       | <span data-ttu-id="70c3f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c3f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70c3f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70c3f-122">Authorization</span></span>  | <span data-ttu-id="70c3f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="70c3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70c3f-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="70c3f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="70c3f-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="70c3f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c3f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70c3f-128">Request body</span></span>
<span data-ttu-id="70c3f-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="70c3f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70c3f-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="70c3f-130">Parameter</span></span>    | <span data-ttu-id="70c3f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="70c3f-131">Type</span></span>   |<span data-ttu-id="70c3f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c3f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70c3f-133">name</span><span class="sxs-lookup"><span data-stu-id="70c3f-133">name</span></span>|<span data-ttu-id="70c3f-134">string</span><span class="sxs-lookup"><span data-stu-id="70c3f-134">string</span></span>|<span data-ttu-id="70c3f-135">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="70c3f-135">The name of the named item.</span></span>|
|<span data-ttu-id="70c3f-136">Referenz</span><span class="sxs-lookup"><span data-stu-id="70c3f-136">reference</span></span>|<span data-ttu-id="70c3f-137">string</span><span class="sxs-lookup"><span data-stu-id="70c3f-137">string</span></span>|<span data-ttu-id="70c3f-138">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="70c3f-138">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="70c3f-139">Kommentar</span><span class="sxs-lookup"><span data-stu-id="70c3f-139">comment</span></span>|<span data-ttu-id="70c3f-140">string</span><span class="sxs-lookup"><span data-stu-id="70c3f-140">string</span></span>|<span data-ttu-id="70c3f-141">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="70c3f-141">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="70c3f-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c3f-142">Response</span></span>

<span data-ttu-id="70c3f-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/nameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70c3f-143">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c3f-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70c3f-144">Example</span></span>
<span data-ttu-id="70c3f-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="70c3f-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="70c3f-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c3f-146">Request</span></span>
<span data-ttu-id="70c3f-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70c3f-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="70c3f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c3f-148">Response</span></span>
<span data-ttu-id="70c3f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70c3f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

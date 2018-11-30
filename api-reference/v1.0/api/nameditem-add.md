---
title: Benanntes Element hinzufügen
description: Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.
ms.openlocfilehash: f97d9589cc29203d660eedf6b323d1ba90794b22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018738"
---
# <a name="add-named-item"></a><span data-ttu-id="64c1d-103">Benanntes Element hinzufügen</span><span class="sxs-lookup"><span data-stu-id="64c1d-103">Add Named Item</span></span>

<span data-ttu-id="64c1d-104">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="64c1d-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c1d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64c1d-105">Permissions</span></span>
<span data-ttu-id="64c1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c1d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64c1d-108">Permission type</span></span>      | <span data-ttu-id="64c1d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64c1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c1d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64c1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64c1d-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c1d-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="64c1d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64c1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c1d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64c1d-113">Not supported.</span></span>    |
|<span data-ttu-id="64c1d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64c1d-114">Application</span></span> | <span data-ttu-id="64c1d-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="64c1d-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64c1d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64c1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="64c1d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="64c1d-117">Request headers</span></span>
| <span data-ttu-id="64c1d-118">Name</span><span class="sxs-lookup"><span data-stu-id="64c1d-118">Name</span></span>       | <span data-ttu-id="64c1d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c1d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64c1d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="64c1d-120">Authorization</span></span>  | <span data-ttu-id="64c1d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="64c1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64c1d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="64c1d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="64c1d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="64c1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c1d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="64c1d-126">Request body</span></span>
<span data-ttu-id="64c1d-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="64c1d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="64c1d-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="64c1d-128">Parameter</span></span>    | <span data-ttu-id="64c1d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="64c1d-129">Type</span></span>   |<span data-ttu-id="64c1d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64c1d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64c1d-131">name</span><span class="sxs-lookup"><span data-stu-id="64c1d-131">name</span></span>|<span data-ttu-id="64c1d-132">string</span><span class="sxs-lookup"><span data-stu-id="64c1d-132">string</span></span>|<span data-ttu-id="64c1d-133">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="64c1d-133">The name of the named item.</span></span>|
|<span data-ttu-id="64c1d-134">Referenz</span><span class="sxs-lookup"><span data-stu-id="64c1d-134">reference</span></span>|<span data-ttu-id="64c1d-135">Json</span><span class="sxs-lookup"><span data-stu-id="64c1d-135">Json</span></span>|<span data-ttu-id="64c1d-136">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="64c1d-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="64c1d-137">Kommentar</span><span class="sxs-lookup"><span data-stu-id="64c1d-137">comment</span></span>|<span data-ttu-id="64c1d-138">string</span><span class="sxs-lookup"><span data-stu-id="64c1d-138">string</span></span>|<span data-ttu-id="64c1d-139">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="64c1d-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="64c1d-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="64c1d-140">Response</span></span>

<span data-ttu-id="64c1d-141">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookNamedItem](../resources/nameditem.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="64c1d-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="64c1d-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64c1d-142">Example</span></span>
<span data-ttu-id="64c1d-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="64c1d-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="64c1d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64c1d-144">Request</span></span>
<span data-ttu-id="64c1d-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="64c1d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="64c1d-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="64c1d-146">Response</span></span>
<span data-ttu-id="64c1d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="64c1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem"
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
  "suppressions": [
    "Warning: NamedItemcollection_add/value:
      Schemas type was 'Custom' which is not supported. Add a resource type to the definition of property: value"
  ],
  "tocPath": ""
}-->

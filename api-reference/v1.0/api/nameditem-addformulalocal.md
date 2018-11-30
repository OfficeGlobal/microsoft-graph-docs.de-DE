---
title: Benanntes Element „FormulaLocal“ hinzufügen
description: Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.
ms.openlocfilehash: 5e4279447143e1b004d468bdcaa9f7b4c2bf8c8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018826"
---
# <a name="add-named-item-formulalocal"></a><span data-ttu-id="ce77b-103">Benanntes Element „FormulaLocal“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ce77b-103">Add Named Item FormulaLocal</span></span>
<span data-ttu-id="ce77b-104">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="ce77b-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce77b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce77b-105">Permissions</span></span>
<span data-ttu-id="ce77b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce77b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce77b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce77b-108">Permission type</span></span>      | <span data-ttu-id="ce77b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce77b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce77b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce77b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce77b-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce77b-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="ce77b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce77b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce77b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce77b-113">Not supported.</span></span>    |
|<span data-ttu-id="ce77b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce77b-114">Application</span></span> | <span data-ttu-id="ce77b-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce77b-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce77b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce77b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="ce77b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce77b-117">Request headers</span></span>
| <span data-ttu-id="ce77b-118">Name</span><span class="sxs-lookup"><span data-stu-id="ce77b-118">Name</span></span>       | <span data-ttu-id="ce77b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce77b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ce77b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce77b-120">Authorization</span></span>  | <span data-ttu-id="ce77b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce77b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce77b-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ce77b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ce77b-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="ce77b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce77b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce77b-126">Request body</span></span>
<span data-ttu-id="ce77b-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ce77b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ce77b-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="ce77b-128">Parameter</span></span>    | <span data-ttu-id="ce77b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ce77b-129">Type</span></span>   |<span data-ttu-id="ce77b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce77b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce77b-131">name</span><span class="sxs-lookup"><span data-stu-id="ce77b-131">name</span></span>|<span data-ttu-id="ce77b-132">string</span><span class="sxs-lookup"><span data-stu-id="ce77b-132">string</span></span>|<span data-ttu-id="ce77b-133">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="ce77b-133">The name of the named item.</span></span>|
|<span data-ttu-id="ce77b-134">Formel</span><span class="sxs-lookup"><span data-stu-id="ce77b-134">formula</span></span>|<span data-ttu-id="ce77b-135">string</span><span class="sxs-lookup"><span data-stu-id="ce77b-135">string</span></span>|<span data-ttu-id="ce77b-136">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="ce77b-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="ce77b-137">Kommentar</span><span class="sxs-lookup"><span data-stu-id="ce77b-137">comment</span></span>|<span data-ttu-id="ce77b-138">string</span><span class="sxs-lookup"><span data-stu-id="ce77b-138">string</span></span>|<span data-ttu-id="ce77b-139">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="ce77b-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="ce77b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce77b-140">Response</span></span>

<span data-ttu-id="ce77b-141">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookNamedItem](../resources/nameditem.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ce77b-141">If successful, this method returns `200 OK` response code and [WorkbookNamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce77b-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce77b-142">Example</span></span>
<span data-ttu-id="ce77b-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ce77b-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ce77b-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce77b-144">Request</span></span>
<span data-ttu-id="ce77b-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce77b-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/addFormulaLocal
Content-type: application/json
Content-length: 54

{
  "name": "test7",
  "formula": "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a><span data-ttu-id="ce77b-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce77b-146">Response</span></span>
<span data-ttu-id="ce77b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce77b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test7%27)",
    "comment": "Comment for the named item",
    "name": "test7",
    "scope": "Workbook",
    "type": "String",
    "value": "0",
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
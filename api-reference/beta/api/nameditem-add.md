---
title: Benanntes Element hinzufügen
description: Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.
localization_priority: Normal
ms.openlocfilehash: 57ae84505327f2afbe2936b2671b655e76a85bd4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836701"
---
# <a name="add-named-item"></a><span data-ttu-id="6e3fe-103">Benanntes Element hinzufügen</span><span class="sxs-lookup"><span data-stu-id="6e3fe-103">Add Named Item</span></span>

> <span data-ttu-id="6e3fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e3fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e3fe-106">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-106">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e3fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e3fe-107">Permissions</span></span>
<span data-ttu-id="6e3fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e3fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e3fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e3fe-110">Permission type</span></span>      | <span data-ttu-id="6e3fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e3fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e3fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e3fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e3fe-113">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3fe-113">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="6e3fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e3fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3fe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e3fe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e3fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e3fe-116">Application</span></span> | <span data-ttu-id="6e3fe-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e3fe-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e3fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e3fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="6e3fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e3fe-119">Request headers</span></span>
| <span data-ttu-id="6e3fe-120">Name</span><span class="sxs-lookup"><span data-stu-id="6e3fe-120">Name</span></span>       | <span data-ttu-id="6e3fe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e3fe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e3fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e3fe-122">Authorization</span></span>  | <span data-ttu-id="6e3fe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e3fe-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="6e3fe-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6e3fe-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e3fe-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e3fe-128">Request body</span></span>
<span data-ttu-id="6e3fe-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e3fe-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="6e3fe-130">Parameter</span></span>    | <span data-ttu-id="6e3fe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6e3fe-131">Type</span></span>   |<span data-ttu-id="6e3fe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e3fe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e3fe-133">name</span><span class="sxs-lookup"><span data-stu-id="6e3fe-133">name</span></span>|<span data-ttu-id="6e3fe-134">string</span><span class="sxs-lookup"><span data-stu-id="6e3fe-134">string</span></span>|<span data-ttu-id="6e3fe-135">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-135">The name of the named item.</span></span>|
|<span data-ttu-id="6e3fe-136">Referenz</span><span class="sxs-lookup"><span data-stu-id="6e3fe-136">reference</span></span>|<span data-ttu-id="6e3fe-137">string</span><span class="sxs-lookup"><span data-stu-id="6e3fe-137">string</span></span>|<span data-ttu-id="6e3fe-138">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-138">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="6e3fe-139">Kommentar</span><span class="sxs-lookup"><span data-stu-id="6e3fe-139">comment</span></span>|<span data-ttu-id="6e3fe-140">string</span><span class="sxs-lookup"><span data-stu-id="6e3fe-140">string</span></span>|<span data-ttu-id="6e3fe-141">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="6e3fe-141">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="6e3fe-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e3fe-142">Response</span></span>

<span data-ttu-id="6e3fe-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/nameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-143">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e3fe-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e3fe-144">Example</span></span>
<span data-ttu-id="6e3fe-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6e3fe-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e3fe-146">Request</span></span>
<span data-ttu-id="6e3fe-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6e3fe-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e3fe-148">Response</span></span>
<span data-ttu-id="6e3fe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e3fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

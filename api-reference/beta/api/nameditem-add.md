---
title: Benanntes Element hinzufügen
description: Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.
localization_priority: Normal
ms.openlocfilehash: 6d27f081c4f8327e02acf4b3004c771848a5a5e0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575485"
---
# <a name="add-named-item"></a><span data-ttu-id="a8a52-103">Benanntes Element hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a8a52-103">Add Named Item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a52-104">Fügt einen neuen Namen zu der Auflistung des angegebenen Bereichs unter Verwendung des Gebietsschemas des Benutzers für die Formel hinzu.</span><span class="sxs-lookup"><span data-stu-id="a8a52-104">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8a52-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8a52-105">Permissions</span></span>
<span data-ttu-id="a8a52-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a52-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8a52-108">Permission type</span></span>      | <span data-ttu-id="a8a52-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8a52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a52-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8a52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a52-111">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8a52-111">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="a8a52-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8a52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a52-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8a52-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8a52-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8a52-114">Application</span></span> | <span data-ttu-id="a8a52-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8a52-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8a52-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a52-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="a8a52-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8a52-117">Request headers</span></span>
| <span data-ttu-id="a8a52-118">Name</span><span class="sxs-lookup"><span data-stu-id="a8a52-118">Name</span></span>       | <span data-ttu-id="a8a52-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8a52-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8a52-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8a52-120">Authorization</span></span>  | <span data-ttu-id="a8a52-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8a52-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8a52-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a8a52-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a8a52-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a8a52-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a52-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8a52-126">Request body</span></span>
<span data-ttu-id="a8a52-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a8a52-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8a52-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8a52-128">Parameter</span></span>    | <span data-ttu-id="a8a52-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a8a52-129">Type</span></span>   |<span data-ttu-id="a8a52-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8a52-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8a52-131">name</span><span class="sxs-lookup"><span data-stu-id="a8a52-131">name</span></span>|<span data-ttu-id="a8a52-132">string</span><span class="sxs-lookup"><span data-stu-id="a8a52-132">string</span></span>|<span data-ttu-id="a8a52-133">Der Name des benannten Elements.</span><span class="sxs-lookup"><span data-stu-id="a8a52-133">The name of the named item.</span></span>|
|<span data-ttu-id="a8a52-134">Referenz</span><span class="sxs-lookup"><span data-stu-id="a8a52-134">reference</span></span>|<span data-ttu-id="a8a52-135">string</span><span class="sxs-lookup"><span data-stu-id="a8a52-135">string</span></span>|<span data-ttu-id="a8a52-136">Die Formel oder der Bereich, auf die bzw. den der Name verweist.</span><span class="sxs-lookup"><span data-stu-id="a8a52-136">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="a8a52-137">Kommentar</span><span class="sxs-lookup"><span data-stu-id="a8a52-137">comment</span></span>|<span data-ttu-id="a8a52-138">string</span><span class="sxs-lookup"><span data-stu-id="a8a52-138">string</span></span>|<span data-ttu-id="a8a52-139">Der Kommentar, der mit dem benannten Element verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="a8a52-139">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="a8a52-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a52-140">Response</span></span>

<span data-ttu-id="a8a52-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/workbooknameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8a52-141">If successful, this method returns `200 OK` response code and [NamedItem](../resources/workbooknameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a52-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8a52-142">Example</span></span>
<span data-ttu-id="a8a52-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a8a52-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a8a52-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8a52-144">Request</span></span>
<span data-ttu-id="a8a52-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8a52-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a8a52-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8a52-146">Response</span></span>
<span data-ttu-id="a8a52-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8a52-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

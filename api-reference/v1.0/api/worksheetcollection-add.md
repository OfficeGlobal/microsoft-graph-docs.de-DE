---
title: 'WorksheetCollection: Hinzufügen'
description: .Activate() darauf.
ms.openlocfilehash: 992524aae6dfca0619c043eb0ddb7a4100f50206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017609"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="f24fa-103">WorksheetCollection: Hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f24fa-103">WorksheetCollection: add</span></span>

<span data-ttu-id="f24fa-p101">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblättern hinzugefügt. Wenn Sie das neu hinzugefügte Arbeitsblatt aktivieren möchten, rufen Sie „.activate()“ dazu auf.</span><span class="sxs-lookup"><span data-stu-id="f24fa-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="f24fa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f24fa-107">Permissions</span></span>
<span data-ttu-id="f24fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f24fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24fa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f24fa-110">Permission type</span></span>      | <span data-ttu-id="f24fa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f24fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f24fa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f24fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f24fa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f24fa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f24fa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f24fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f24fa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24fa-115">Not supported.</span></span>    |
|<span data-ttu-id="f24fa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f24fa-116">Application</span></span> | <span data-ttu-id="f24fa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24fa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f24fa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24fa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="f24fa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f24fa-119">Request headers</span></span>
| <span data-ttu-id="f24fa-120">Name</span><span class="sxs-lookup"><span data-stu-id="f24fa-120">Name</span></span>       | <span data-ttu-id="f24fa-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f24fa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f24fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f24fa-122">Authorization</span></span>  | <span data-ttu-id="f24fa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f24fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f24fa-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f24fa-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f24fa-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f24fa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f24fa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f24fa-128">Request body</span></span>
<span data-ttu-id="f24fa-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f24fa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f24fa-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="f24fa-130">Parameter</span></span>    | <span data-ttu-id="f24fa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f24fa-131">Type</span></span>   |<span data-ttu-id="f24fa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f24fa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f24fa-133">name</span><span class="sxs-lookup"><span data-stu-id="f24fa-133">name</span></span>|<span data-ttu-id="f24fa-134">string</span><span class="sxs-lookup"><span data-stu-id="f24fa-134">string</span></span>|<span data-ttu-id="f24fa-p105">Optional. Der Name des hinzuzufügenden Arbeitsblatts. Falls angegeben, sollte der Name eindeutig sein. Falls nicht angegeben, bestimmt Excel den Namen des neuen Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="f24fa-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="f24fa-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24fa-139">Response</span></span>

<span data-ttu-id="f24fa-140">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [WorkbookWorksheet](../resources/worksheet.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f24fa-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f24fa-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f24fa-141">Example</span></span>
<span data-ttu-id="f24fa-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f24fa-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f24fa-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24fa-143">Request</span></span>
<span data-ttu-id="f24fa-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f24fa-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="f24fa-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24fa-145">Response</span></span>
<span data-ttu-id="f24fa-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f24fa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
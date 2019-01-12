---
title: 'WorksheetCollection: Hinzufügen'
description: .Activate() darauf.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9f18d181aa756e01ae5439fcf44526dc825be40
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985004"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="8c020-103">WorksheetCollection: Hinzufügen</span><span class="sxs-lookup"><span data-stu-id="8c020-103">WorksheetCollection: add</span></span>

> <span data-ttu-id="8c020-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c020-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c020-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c020-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c020-p102">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblättern hinzugefügt. Wenn Sie das neu hinzugefügte Arbeitsblatt aktivieren möchten, rufen Sie „.activate()“ dazu auf.</span><span class="sxs-lookup"><span data-stu-id="8c020-p102">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c020-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8c020-109">Permissions</span></span>
<span data-ttu-id="8c020-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c020-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c020-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c020-112">Permission type</span></span>      | <span data-ttu-id="8c020-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c020-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c020-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c020-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8c020-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c020-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c020-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c020-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c020-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c020-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c020-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c020-118">Application</span></span> | <span data-ttu-id="8c020-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c020-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c020-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c020-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="8c020-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c020-121">Request headers</span></span>
| <span data-ttu-id="8c020-122">Name</span><span class="sxs-lookup"><span data-stu-id="8c020-122">Name</span></span>       | <span data-ttu-id="8c020-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c020-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c020-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c020-124">Authorization</span></span>  | <span data-ttu-id="8c020-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8c020-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c020-127">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8c020-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c020-p105">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8c020-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c020-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c020-130">Request body</span></span>
<span data-ttu-id="8c020-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8c020-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c020-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="8c020-132">Parameter</span></span>    | <span data-ttu-id="8c020-133">Typ</span><span class="sxs-lookup"><span data-stu-id="8c020-133">Type</span></span>   |<span data-ttu-id="8c020-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c020-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c020-135">name</span><span class="sxs-lookup"><span data-stu-id="8c020-135">name</span></span>|<span data-ttu-id="8c020-136">string</span><span class="sxs-lookup"><span data-stu-id="8c020-136">string</span></span>|<span data-ttu-id="8c020-p106">Optional. Der Name des hinzuzufügenden Arbeitsblatts. Falls angegeben, sollte der Name eindeutig sein. Falls nicht angegeben, bestimmt Excel den Namen des neuen Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="8c020-p106">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="8c020-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c020-141">Response</span></span>

<span data-ttu-id="8c020-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Worksheet](../resources/worksheet.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c020-142">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c020-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c020-143">Example</span></span>
<span data-ttu-id="8c020-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8c020-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c020-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c020-145">Request</span></span>
<span data-ttu-id="8c020-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c020-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="8c020-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c020-147">Response</span></span>
<span data-ttu-id="8c020-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c020-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
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

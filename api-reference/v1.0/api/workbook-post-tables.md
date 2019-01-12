---
title: Tabelle erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Tabelle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 220c0b1e9b21c609009616d75567c0469b276cd4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986985"
---
# <a name="create-table"></a><span data-ttu-id="d056d-103">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="d056d-103">Create table</span></span>

<span data-ttu-id="d056d-104">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="d056d-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d056d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d056d-105">Permissions</span></span>
<span data-ttu-id="d056d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d056d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d056d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d056d-108">Permission type</span></span>      | <span data-ttu-id="d056d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d056d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d056d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d056d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d056d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d056d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d056d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d056d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d056d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d056d-113">Not supported.</span></span>    |
|<span data-ttu-id="d056d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d056d-114">Application</span></span> | <span data-ttu-id="d056d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d056d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d056d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d056d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{table-id}/add

```
## <a name="request-headers"></a><span data-ttu-id="d056d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d056d-117">Request headers</span></span>
| <span data-ttu-id="d056d-118">Name</span><span class="sxs-lookup"><span data-stu-id="d056d-118">Name</span></span>       | <span data-ttu-id="d056d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d056d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d056d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d056d-120">Authorization</span></span>  | <span data-ttu-id="d056d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d056d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d056d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="d056d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d056d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="d056d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d056d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d056d-126">Request body</span></span>
<span data-ttu-id="d056d-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="d056d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d056d-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="d056d-128">Parameter</span></span>           | <span data-ttu-id="d056d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d056d-129">Type</span></span>      |<span data-ttu-id="d056d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d056d-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="d056d-131">Address</span><span class="sxs-lookup"><span data-stu-id="d056d-131">Address</span></span>  | <span data-ttu-id="d056d-132">string</span><span class="sxs-lookup"><span data-stu-id="d056d-132">string</span></span>| <span data-ttu-id="d056d-p104">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="d056d-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="d056d-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d056d-136">hasHeaders</span></span>  | <span data-ttu-id="d056d-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d056d-137">boolean</span></span>|<span data-ttu-id="d056d-p105">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="d056d-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="d056d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d056d-141">Response</span></span>

<span data-ttu-id="d056d-142">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und [WorkbookTable](../resources/table.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d056d-142">If successful, this method returns `201 Created` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d056d-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d056d-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d056d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d056d-144">Request</span></span>
<span data-ttu-id="d056d-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d056d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{table-id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="d056d-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="d056d-146">Response</span></span>
<span data-ttu-id="d056d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d056d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

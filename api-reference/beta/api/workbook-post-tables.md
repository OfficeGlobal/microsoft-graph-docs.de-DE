---
title: Tabelle erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Tabelle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 67f34a0310fcfd0ba6641eeecbbb8c3e6fc2a05f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643636"
---
# <a name="create-table"></a><span data-ttu-id="9e1ee-103">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="9e1ee-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e1ee-104">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e1ee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9e1ee-105">Permissions</span></span>
<span data-ttu-id="9e1ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e1ee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e1ee-108">Permission type</span></span>      | <span data-ttu-id="9e1ee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e1ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e1ee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e1ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e1ee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e1ee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9e1ee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e1ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e1ee-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e1ee-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9e1ee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e1ee-114">Application</span></span> | <span data-ttu-id="9e1ee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e1ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e1ee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e1ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="9e1ee-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e1ee-117">Request headers</span></span>
| <span data-ttu-id="9e1ee-118">Name</span><span class="sxs-lookup"><span data-stu-id="9e1ee-118">Name</span></span>       | <span data-ttu-id="9e1ee-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e1ee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e1ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e1ee-120">Authorization</span></span>  | <span data-ttu-id="9e1ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e1ee-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9e1ee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9e1ee-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e1ee-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e1ee-126">Request body</span></span>
<span data-ttu-id="9e1ee-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9e1ee-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="9e1ee-128">Parameter</span></span>           | <span data-ttu-id="9e1ee-129">Typ</span><span class="sxs-lookup"><span data-stu-id="9e1ee-129">Type</span></span>      |<span data-ttu-id="9e1ee-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e1ee-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="9e1ee-131">Address</span><span class="sxs-lookup"><span data-stu-id="9e1ee-131">Address</span></span>  | <span data-ttu-id="9e1ee-132">string</span><span class="sxs-lookup"><span data-stu-id="9e1ee-132">string</span></span>| <span data-ttu-id="9e1ee-p104">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="9e1ee-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="9e1ee-136">hasHeaders</span></span>  | <span data-ttu-id="9e1ee-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9e1ee-137">boolean</span></span>|<span data-ttu-id="9e1ee-p105">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="9e1ee-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e1ee-141">Response</span></span>

<span data-ttu-id="9e1ee-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-142">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e1ee-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e1ee-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e1ee-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e1ee-144">Request</span></span>
<span data-ttu-id="9e1ee-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="9e1ee-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e1ee-146">Response</span></span>
<span data-ttu-id="9e1ee-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e1ee-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-post-tables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

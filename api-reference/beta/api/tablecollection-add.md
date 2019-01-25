---
title: 'TableCollection: add'
description: Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a4d96ba219ffe10d0bb0a4e5d414fd474490e84a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522903"
---
# <a name="tablecollection-add"></a><span data-ttu-id="49168-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="49168-105">TableCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49168-p102">Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="49168-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="49168-109">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="49168-109">Error Handling</span></span>

<span data-ttu-id="49168-110">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="49168-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="49168-111">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49168-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="49168-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49168-112">Permissions</span></span>
<span data-ttu-id="49168-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49168-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49168-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49168-115">Permission type</span></span>      | <span data-ttu-id="49168-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49168-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49168-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49168-117">Delegated (work or school account)</span></span> | <span data-ttu-id="49168-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49168-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49168-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49168-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49168-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49168-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49168-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49168-121">Application</span></span> | <span data-ttu-id="49168-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49168-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49168-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49168-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="49168-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49168-124">Request headers</span></span>
| <span data-ttu-id="49168-125">Name</span><span class="sxs-lookup"><span data-stu-id="49168-125">Name</span></span>       | <span data-ttu-id="49168-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49168-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49168-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="49168-127">Authorization</span></span>  | <span data-ttu-id="49168-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49168-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49168-130">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="49168-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="49168-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="49168-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49168-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49168-133">Request body</span></span>
<span data-ttu-id="49168-134">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="49168-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49168-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="49168-135">Parameter</span></span>    | <span data-ttu-id="49168-136">Typ</span><span class="sxs-lookup"><span data-stu-id="49168-136">Type</span></span>   |<span data-ttu-id="49168-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49168-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49168-138">address</span><span class="sxs-lookup"><span data-stu-id="49168-138">address</span></span>|<span data-ttu-id="49168-139">string</span><span class="sxs-lookup"><span data-stu-id="49168-139">string</span></span>|<span data-ttu-id="49168-p107">Adresse oder der Name des Bereichobjekts, das die Datenquelle darstellt. Wenn die Adresse keinen Arbeitsblattnamen enthält, wird das aktuell aktive Blatt verwendet.</span><span class="sxs-lookup"><span data-stu-id="49168-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="49168-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="49168-142">hasHeaders</span></span>|<span data-ttu-id="49168-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="49168-143">boolean</span></span>|<span data-ttu-id="49168-p108">Boolescher Wert, der angibt, ob die importierten Daten Spaltenüberschriften besitzen. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf falsch festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="49168-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="49168-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="49168-147">Response</span></span>

<span data-ttu-id="49168-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49168-148">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49168-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49168-149">Example</span></span>
<span data-ttu-id="49168-150">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="49168-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49168-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49168-151">Request</span></span>
<span data-ttu-id="49168-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49168-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="49168-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="49168-153">Response</span></span>
<span data-ttu-id="49168-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49168-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

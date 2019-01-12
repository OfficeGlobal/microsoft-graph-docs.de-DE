---
title: 'TableCollection: add'
description: Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 75d39b32c651ad1633b48aa91514d4b2e118b136
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912925"
---
# <a name="tablecollection-add"></a><span data-ttu-id="79822-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="79822-105">TableCollection: add</span></span>

> <span data-ttu-id="79822-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79822-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79822-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79822-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79822-p103">Erstellen Sie eine neue Tabelle. Die Bereichsquelladresse bestimmt das Arbeitsblatt, unter dem die Tabelle hinzugefügt wird. Wenn die Tabelle nicht hinzugefügt werden kann, (z. B. da die Adresse ungültig ist oder sich die Tabelle mit einer anderen Tabelle überlappen würde), wird ein Fehler ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="79822-p103">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="79822-111">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="79822-111">Error Handling</span></span>

<span data-ttu-id="79822-112">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="79822-112">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="79822-113">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79822-113">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="79822-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79822-114">Permissions</span></span>
<span data-ttu-id="79822-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79822-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79822-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79822-117">Permission type</span></span>      | <span data-ttu-id="79822-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79822-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79822-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79822-119">Delegated (work or school account)</span></span> | <span data-ttu-id="79822-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79822-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79822-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79822-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79822-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79822-122">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79822-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79822-123">Application</span></span> | <span data-ttu-id="79822-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79822-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79822-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79822-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="79822-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79822-126">Request headers</span></span>
| <span data-ttu-id="79822-127">Name</span><span class="sxs-lookup"><span data-stu-id="79822-127">Name</span></span>       | <span data-ttu-id="79822-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79822-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79822-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="79822-129">Authorization</span></span>  | <span data-ttu-id="79822-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79822-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79822-132">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="79822-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="79822-p107">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="79822-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79822-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79822-135">Request body</span></span>
<span data-ttu-id="79822-136">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="79822-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79822-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="79822-137">Parameter</span></span>    | <span data-ttu-id="79822-138">Typ</span><span class="sxs-lookup"><span data-stu-id="79822-138">Type</span></span>   |<span data-ttu-id="79822-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79822-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79822-140">address</span><span class="sxs-lookup"><span data-stu-id="79822-140">address</span></span>|<span data-ttu-id="79822-141">string</span><span class="sxs-lookup"><span data-stu-id="79822-141">string</span></span>|<span data-ttu-id="79822-p108">Adresse oder der Name des Bereichobjekts, das die Datenquelle darstellt. Wenn die Adresse keinen Arbeitsblattnamen enthält, wird das aktuell aktive Blatt verwendet.</span><span class="sxs-lookup"><span data-stu-id="79822-p108">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="79822-144">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="79822-144">hasHeaders</span></span>|<span data-ttu-id="79822-145">boolean</span><span class="sxs-lookup"><span data-stu-id="79822-145">boolean</span></span>|<span data-ttu-id="79822-p109">Boolescher Wert, der angibt, ob die importierten Daten Spaltenüberschriften besitzen. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf falsch festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="79822-p109">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="79822-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="79822-149">Response</span></span>

<span data-ttu-id="79822-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79822-150">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79822-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79822-151">Example</span></span>
<span data-ttu-id="79822-152">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="79822-152">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79822-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79822-153">Request</span></span>
<span data-ttu-id="79822-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79822-154">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="79822-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="79822-155">Response</span></span>
<span data-ttu-id="79822-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79822-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

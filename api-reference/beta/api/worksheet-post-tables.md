---
title: Tabelle erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Tabelle.
ms.openlocfilehash: a56091ca2ed5e3bad69b3d618fe760db5b350c9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062745"
---
# <a name="create-table"></a><span data-ttu-id="00ea8-103">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="00ea8-103">Create table</span></span>

> <span data-ttu-id="00ea8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="00ea8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ea8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00ea8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00ea8-106">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="00ea8-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="00ea8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="00ea8-107">Permissions</span></span>
<span data-ttu-id="00ea8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ea8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ea8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00ea8-110">Permission type</span></span>      | <span data-ttu-id="00ea8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00ea8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ea8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00ea8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00ea8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ea8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00ea8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00ea8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ea8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ea8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00ea8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00ea8-116">Application</span></span> | <span data-ttu-id="00ea8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00ea8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ea8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ea8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="00ea8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00ea8-119">Request headers</span></span>
| <span data-ttu-id="00ea8-120">Name</span><span class="sxs-lookup"><span data-stu-id="00ea8-120">Name</span></span>       | <span data-ttu-id="00ea8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ea8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00ea8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00ea8-122">Authorization</span></span>  | <span data-ttu-id="00ea8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="00ea8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00ea8-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="00ea8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="00ea8-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="00ea8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ea8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00ea8-128">Request body</span></span>
<span data-ttu-id="00ea8-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="00ea8-129">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="00ea8-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="00ea8-130">Parameter</span></span>       | <span data-ttu-id="00ea8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="00ea8-131">Type</span></span>|<span data-ttu-id="00ea8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00ea8-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="00ea8-133">Address</span><span class="sxs-lookup"><span data-stu-id="00ea8-133">Address</span></span>  | <span data-ttu-id="00ea8-134">string</span><span class="sxs-lookup"><span data-stu-id="00ea8-134">string</span></span>| <span data-ttu-id="00ea8-p105">Bereichsadresse. Wenn Sie diese API über den Pfad „worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="00ea8-p105">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="00ea8-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span><span class="sxs-lookup"><span data-stu-id="00ea8-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="00ea8-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="00ea8-138">hasHeaders</span></span>  | <span data-ttu-id="00ea8-139">boolean</span><span class="sxs-lookup"><span data-stu-id="00ea8-139">boolean</span></span>|<span data-ttu-id="00ea8-p106">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="00ea8-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="00ea8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ea8-143">Response</span></span>

<span data-ttu-id="00ea8-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00ea8-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ea8-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00ea8-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00ea8-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00ea8-146">Request</span></span>
<span data-ttu-id="00ea8-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00ea8-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="00ea8-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="00ea8-148">Response</span></span>
<span data-ttu-id="00ea8-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00ea8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

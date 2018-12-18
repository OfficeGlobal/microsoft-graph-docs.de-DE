---
title: Tabelle erstellen
description: Verwenden Sie diese API zum Erstellen einer neuen Tabelle.
author: lumine2008
ms.openlocfilehash: 75d4199b4c5cefcb17acccfedfb5c45a3f296de0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321623"
---
# <a name="create-table"></a><span data-ttu-id="53ede-103">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="53ede-103">Create table</span></span>

> <span data-ttu-id="53ede-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="53ede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53ede-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53ede-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53ede-106">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="53ede-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="53ede-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53ede-107">Permissions</span></span>
<span data-ttu-id="53ede-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53ede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53ede-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53ede-110">Permission type</span></span>      | <span data-ttu-id="53ede-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53ede-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53ede-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53ede-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53ede-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ede-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53ede-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53ede-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53ede-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ede-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53ede-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53ede-116">Application</span></span> | <span data-ttu-id="53ede-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53ede-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53ede-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53ede-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="53ede-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53ede-119">Request headers</span></span>
| <span data-ttu-id="53ede-120">Name</span><span class="sxs-lookup"><span data-stu-id="53ede-120">Name</span></span>       | <span data-ttu-id="53ede-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53ede-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53ede-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ede-122">Authorization</span></span>  | <span data-ttu-id="53ede-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="53ede-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53ede-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="53ede-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="53ede-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="53ede-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53ede-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53ede-128">Request body</span></span>
<span data-ttu-id="53ede-129">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="53ede-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53ede-130">Parameter</span><span class="sxs-lookup"><span data-stu-id="53ede-130">Parameter</span></span>           | <span data-ttu-id="53ede-131">Typ</span><span class="sxs-lookup"><span data-stu-id="53ede-131">Type</span></span>      |<span data-ttu-id="53ede-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53ede-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="53ede-133">Address</span><span class="sxs-lookup"><span data-stu-id="53ede-133">Address</span></span>  | <span data-ttu-id="53ede-134">string</span><span class="sxs-lookup"><span data-stu-id="53ede-134">string</span></span>| <span data-ttu-id="53ede-p105">Bereichsadresse. Wenn Sie diese API abseits des `worksheets/{id or name}/tables/add`-Pfads aufrufen, müssen Sie das Präfix für den Blattnamen nicht in der Adresse angeben. Wenn Sie diese jedoch abseits des `workbook/tables/add`-Pfads aufrufen, müssen Sie den Blattnamen angeben, auf dem die Tabelle erstellt werden muss (Beispiel: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="53ede-p105">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="53ede-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="53ede-138">hasHeaders</span></span>  | <span data-ttu-id="53ede-139">boolean</span><span class="sxs-lookup"><span data-stu-id="53ede-139">boolean</span></span>|<span data-ttu-id="53ede-p106">Boolescher Wert, der angibt, ob der Bereich Spaltenbeschriftungen hat. Wenn die Quelle keine Überschriften enthält (d. h. wenn diese Eigenschaft auf „false“ festgelegt ist), generiert Excel automatisch eine Überschriftenänderung der Daten nach einer Zeile.</span><span class="sxs-lookup"><span data-stu-id="53ede-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="53ede-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="53ede-143">Response</span></span>

<span data-ttu-id="53ede-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53ede-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53ede-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53ede-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53ede-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53ede-146">Request</span></span>
<span data-ttu-id="53ede-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53ede-147">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="53ede-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="53ede-148">Response</span></span>
<span data-ttu-id="53ede-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53ede-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

---
title: tablerow aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des tablerow-Objekts.
author: lumine2008
ms.openlocfilehash: cdc0049db5455891f844d2955554c73f5e77bb4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311550"
---
# <a name="update-tablerow"></a><span data-ttu-id="5c7d2-103">tablerow aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5c7d2-103">Update tablerow</span></span>

> <span data-ttu-id="5c7d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c7d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c7d2-106">Dient zum Aktualisieren der Eigenschaften des tablerow-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-106">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5c7d2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5c7d2-107">Permissions</span></span>
<span data-ttu-id="5c7d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c7d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c7d2-110">Permission type</span></span>      | <span data-ttu-id="5c7d2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c7d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c7d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c7d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c7d2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c7d2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c7d2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c7d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c7d2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c7d2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5c7d2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c7d2-116">Application</span></span> | <span data-ttu-id="5c7d2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c7d2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c7d2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c7d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="5c7d2-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c7d2-119">Optional request headers</span></span>
| <span data-ttu-id="5c7d2-120">Name</span><span class="sxs-lookup"><span data-stu-id="5c7d2-120">Name</span></span>       | <span data-ttu-id="5c7d2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c7d2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5c7d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c7d2-122">Authorization</span></span>  | <span data-ttu-id="5c7d2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c7d2-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5c7d2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5c7d2-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c7d2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c7d2-128">Request body</span></span>
<span data-ttu-id="5c7d2-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5c7d2-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c7d2-132">Property</span></span>     | <span data-ttu-id="5c7d2-133">Typ</span><span class="sxs-lookup"><span data-stu-id="5c7d2-133">Type</span></span>   |<span data-ttu-id="5c7d2-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c7d2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c7d2-135">values</span><span class="sxs-lookup"><span data-stu-id="5c7d2-135">values</span></span>|<span data-ttu-id="5c7d2-136">json</span><span class="sxs-lookup"><span data-stu-id="5c7d2-136">json</span></span>|<span data-ttu-id="5c7d2-p106">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="5c7d2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c7d2-140">Response</span></span>

<span data-ttu-id="5c7d2-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-141">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c7d2-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c7d2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c7d2-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c7d2-143">Request</span></span>
<span data-ttu-id="5c7d2-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="5c7d2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c7d2-145">Response</span></span>
<span data-ttu-id="5c7d2-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c7d2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
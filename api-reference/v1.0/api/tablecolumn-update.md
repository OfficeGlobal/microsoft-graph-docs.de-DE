---
title: tablecolumn aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des tablecolumn-Objekts.
ms.openlocfilehash: bdf7414186d62f6875488af4f83e302118de3e08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016051"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="3e44a-103">tablecolumn aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3e44a-103">Update tablecolumn</span></span>

<span data-ttu-id="3e44a-104">Dient zum Aktualisieren der Eigenschaften des tablecolumn-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e44a-104">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e44a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e44a-105">Permissions</span></span>
<span data-ttu-id="3e44a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e44a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e44a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e44a-108">Permission type</span></span>      | <span data-ttu-id="3e44a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e44a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e44a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e44a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e44a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e44a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e44a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e44a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e44a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e44a-113">Not supported.</span></span>    |
|<span data-ttu-id="3e44a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e44a-114">Application</span></span> | <span data-ttu-id="3e44a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e44a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e44a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e44a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3e44a-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e44a-117">Optional request headers</span></span>
| <span data-ttu-id="3e44a-118">Name</span><span class="sxs-lookup"><span data-stu-id="3e44a-118">Name</span></span>       | <span data-ttu-id="3e44a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e44a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e44a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e44a-120">Authorization</span></span>  | <span data-ttu-id="3e44a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e44a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e44a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="3e44a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e44a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="3e44a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e44a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e44a-126">Request body</span></span>
<span data-ttu-id="3e44a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="3e44a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e44a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e44a-130">Property</span></span>     | <span data-ttu-id="3e44a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3e44a-131">Type</span></span>   |<span data-ttu-id="3e44a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e44a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e44a-133">values</span><span class="sxs-lookup"><span data-stu-id="3e44a-133">values</span></span>|<span data-ttu-id="3e44a-134">Json</span><span class="sxs-lookup"><span data-stu-id="3e44a-134">Json</span></span>|<span data-ttu-id="3e44a-p105">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="3e44a-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="3e44a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e44a-138">Response</span></span>

<span data-ttu-id="3e44a-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookTableColumn](../resources/tablecolumn.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e44a-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e44a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e44a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e44a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e44a-141">Request</span></span>
<span data-ttu-id="3e44a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e44a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="3e44a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e44a-143">Response</span></span>
<span data-ttu-id="3e44a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e44a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
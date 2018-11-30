---
title: formatprotection aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.
ms.openlocfilehash: 691715a921ae98f725f26566fb144530f27330b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020056"
---
# <a name="update-formatprotection"></a><span data-ttu-id="0f53a-103">formatprotection aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0f53a-103">Update formatprotection</span></span>

<span data-ttu-id="0f53a-104">Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f53a-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f53a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f53a-105">Permissions</span></span>
<span data-ttu-id="0f53a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f53a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f53a-108">Permission type</span></span>      | <span data-ttu-id="0f53a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f53a-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0f53a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f53a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f53a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f53a-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="0f53a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f53a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f53a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f53a-113">Not supported.</span></span>    | 
|<span data-ttu-id="0f53a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f53a-114">Application</span></span> | <span data-ttu-id="0f53a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f53a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0f53a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f53a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="0f53a-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f53a-117">Optional request headers</span></span>
| <span data-ttu-id="0f53a-118">Name</span><span class="sxs-lookup"><span data-stu-id="0f53a-118">Name</span></span>       | <span data-ttu-id="0f53a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f53a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0f53a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f53a-120">Authorization</span></span>  | <span data-ttu-id="0f53a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f53a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0f53a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f53a-123">Request body</span></span>
<span data-ttu-id="0f53a-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0f53a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0f53a-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f53a-127">Property</span></span>     | <span data-ttu-id="0f53a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="0f53a-128">Type</span></span>   |<span data-ttu-id="0f53a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f53a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f53a-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="0f53a-130">formulaHidden</span></span>|<span data-ttu-id="0f53a-131">boolean</span><span class="sxs-lookup"><span data-stu-id="0f53a-131">boolean</span></span>|<span data-ttu-id="0f53a-p104">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="0f53a-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="0f53a-134">locked</span><span class="sxs-lookup"><span data-stu-id="0f53a-134">locked</span></span>|<span data-ttu-id="0f53a-135">boolean</span><span class="sxs-lookup"><span data-stu-id="0f53a-135">boolean</span></span>|<span data-ttu-id="0f53a-p105">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="0f53a-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="0f53a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f53a-138">Response</span></span>

<span data-ttu-id="0f53a-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f53a-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f53a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f53a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f53a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f53a-141">Request</span></span>
<span data-ttu-id="0f53a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f53a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="0f53a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f53a-143">Response</span></span>
<span data-ttu-id="0f53a-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f53a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
---
title: formatprotection aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.
localization_priority: Normal
ms.openlocfilehash: f1ee62cf4c483c821d80de42dc8645f9cda2bdeb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520529"
---
# <a name="update-formatprotection"></a><span data-ttu-id="8a9d5-103">formatprotection aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8a9d5-103">Update formatprotection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a9d5-104">Dient zum Aktualisieren der Eigenschaften des formatprotection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a9d5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a9d5-105">Permissions</span></span>
<span data-ttu-id="8a9d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a9d5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a9d5-108">Permission type</span></span>      | <span data-ttu-id="8a9d5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a9d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a9d5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a9d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a9d5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a9d5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a9d5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a9d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a9d5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a9d5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a9d5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a9d5-114">Application</span></span> | <span data-ttu-id="8a9d5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a9d5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a9d5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a9d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="8a9d5-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a9d5-117">Optional request headers</span></span>
| <span data-ttu-id="8a9d5-118">Name</span><span class="sxs-lookup"><span data-stu-id="8a9d5-118">Name</span></span>       | <span data-ttu-id="8a9d5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a9d5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8a9d5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a9d5-120">Authorization</span></span>  | <span data-ttu-id="8a9d5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a9d5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a9d5-123">Request body</span></span>
<span data-ttu-id="8a9d5-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a9d5-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a9d5-127">Property</span></span>     | <span data-ttu-id="8a9d5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="8a9d5-128">Type</span></span>   |<span data-ttu-id="8a9d5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a9d5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a9d5-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="8a9d5-130">formulaHidden</span></span>|<span data-ttu-id="8a9d5-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8a9d5-131">boolean</span></span>|<span data-ttu-id="8a9d5-p104">Zeigt an, ob Excel die Formel für die Zellen im Bereich ausblendet. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zur Formelausblendung hat.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="8a9d5-134">locked</span><span class="sxs-lookup"><span data-stu-id="8a9d5-134">locked</span></span>|<span data-ttu-id="8a9d5-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8a9d5-135">boolean</span></span>|<span data-ttu-id="8a9d5-p105">Gibt an, ob Excel die Zellen im Objekt sperrt. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Einstellung zum Sperren hat.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="8a9d5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a9d5-138">Response</span></span>

<span data-ttu-id="8a9d5-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a9d5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a9d5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a9d5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a9d5-141">Request</span></span>
<span data-ttu-id="8a9d5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="8a9d5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a9d5-143">Response</span></span>
<span data-ttu-id="8a9d5-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a9d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/formatprotection-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

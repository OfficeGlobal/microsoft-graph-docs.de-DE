---
title: Arbeitsblatt aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.
ms.openlocfilehash: 893bfb8ea9f5f6852550f072ea43421709705e2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016069"
---
# <a name="update-worksheet"></a><span data-ttu-id="61e57-103">Arbeitsblatt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61e57-103">Update worksheet</span></span>

<span data-ttu-id="61e57-104">Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.</span><span class="sxs-lookup"><span data-stu-id="61e57-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="61e57-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61e57-105">Permissions</span></span>
<span data-ttu-id="61e57-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61e57-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61e57-108">Permission type</span></span>      | <span data-ttu-id="61e57-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61e57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61e57-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61e57-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61e57-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61e57-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="61e57-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61e57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61e57-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61e57-113">Not supported.</span></span>    |
|<span data-ttu-id="61e57-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61e57-114">Application</span></span> | <span data-ttu-id="61e57-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61e57-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61e57-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61e57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="61e57-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61e57-117">Optional request headers</span></span>
| <span data-ttu-id="61e57-118">Name</span><span class="sxs-lookup"><span data-stu-id="61e57-118">Name</span></span>       | <span data-ttu-id="61e57-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61e57-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="61e57-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="61e57-120">Authorization</span></span>  | <span data-ttu-id="61e57-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61e57-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61e57-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="61e57-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="61e57-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="61e57-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61e57-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61e57-126">Request body</span></span>
<span data-ttu-id="61e57-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="61e57-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="61e57-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61e57-130">Property</span></span>     | <span data-ttu-id="61e57-131">Typ</span><span class="sxs-lookup"><span data-stu-id="61e57-131">Type</span></span>   |<span data-ttu-id="61e57-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61e57-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61e57-133">name</span><span class="sxs-lookup"><span data-stu-id="61e57-133">name</span></span>|<span data-ttu-id="61e57-134">string</span><span class="sxs-lookup"><span data-stu-id="61e57-134">string</span></span>|<span data-ttu-id="61e57-135">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="61e57-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="61e57-136">position</span><span class="sxs-lookup"><span data-stu-id="61e57-136">position</span></span>|<span data-ttu-id="61e57-137">int</span><span class="sxs-lookup"><span data-stu-id="61e57-137">int</span></span>|<span data-ttu-id="61e57-138">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="61e57-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="61e57-139">visibility</span><span class="sxs-lookup"><span data-stu-id="61e57-139">visibility</span></span>|<span data-ttu-id="61e57-140">string</span><span class="sxs-lookup"><span data-stu-id="61e57-140">string</span></span>|<span data-ttu-id="61e57-141">Die Sichtbarkeit des Arbeitsblatts ein.</span><span class="sxs-lookup"><span data-stu-id="61e57-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="61e57-142">Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="61e57-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="61e57-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="61e57-143">Response</span></span>

<span data-ttu-id="61e57-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookWorksheet](../resources/worksheet.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="61e57-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61e57-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61e57-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61e57-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61e57-146">Request</span></span>
<span data-ttu-id="61e57-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="61e57-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="61e57-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="61e57-148">Response</span></span>
<span data-ttu-id="61e57-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61e57-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
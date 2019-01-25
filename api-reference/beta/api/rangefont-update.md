---
title: rangefont aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5857941f8c08c9090ba05098ae1d69a34dead791
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529698"
---
# <a name="update-rangefont"></a><span data-ttu-id="1c8d6-103">rangefont aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1c8d6-103">Update rangefont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c8d6-104">Dient zum Aktualisieren der Eigenschaften des rangefont-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-104">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c8d6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1c8d6-105">Permissions</span></span>
<span data-ttu-id="1c8d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c8d6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c8d6-108">Permission type</span></span>      | <span data-ttu-id="1c8d6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c8d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c8d6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c8d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c8d6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c8d6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c8d6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c8d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c8d6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c8d6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c8d6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c8d6-114">Application</span></span> | <span data-ttu-id="1c8d6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c8d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c8d6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c8d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="1c8d6-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c8d6-117">Optional request headers</span></span>
| <span data-ttu-id="1c8d6-118">Name</span><span class="sxs-lookup"><span data-stu-id="1c8d6-118">Name</span></span>       | <span data-ttu-id="1c8d6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c8d6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1c8d6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c8d6-120">Authorization</span></span>  | <span data-ttu-id="1c8d6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c8d6-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1c8d6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c8d6-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c8d6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c8d6-126">Request body</span></span>
<span data-ttu-id="1c8d6-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c8d6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c8d6-130">Property</span></span>     | <span data-ttu-id="1c8d6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1c8d6-131">Type</span></span>   |<span data-ttu-id="1c8d6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c8d6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c8d6-133">bold</span><span class="sxs-lookup"><span data-stu-id="1c8d6-133">bold</span></span>|<span data-ttu-id="1c8d6-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1c8d6-134">boolean</span></span>|<span data-ttu-id="1c8d6-135">Stellt den Fett-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-135">Represents the bold status of font.</span></span>|
|<span data-ttu-id="1c8d6-136">color</span><span class="sxs-lookup"><span data-stu-id="1c8d6-136">color</span></span>|<span data-ttu-id="1c8d6-137">string</span><span class="sxs-lookup"><span data-stu-id="1c8d6-137">string</span></span>|<span data-ttu-id="1c8d6-p105">HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p105">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="1c8d6-141">italic</span><span class="sxs-lookup"><span data-stu-id="1c8d6-141">italic</span></span>|<span data-ttu-id="1c8d6-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1c8d6-142">boolean</span></span>|<span data-ttu-id="1c8d6-143">Stellt den Kursiv-Status der Schriftart dar.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-143">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="1c8d6-144">name</span><span class="sxs-lookup"><span data-stu-id="1c8d6-144">name</span></span>|<span data-ttu-id="1c8d6-145">string</span><span class="sxs-lookup"><span data-stu-id="1c8d6-145">string</span></span>|<span data-ttu-id="1c8d6-146">Schriftartname (z. B. "Calibri")</span><span class="sxs-lookup"><span data-stu-id="1c8d6-146">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="1c8d6-147">size</span><span class="sxs-lookup"><span data-stu-id="1c8d6-147">size</span></span>|<span data-ttu-id="1c8d6-148">double</span><span class="sxs-lookup"><span data-stu-id="1c8d6-148">double</span></span>|<span data-ttu-id="1c8d6-149">Schriftgrad</span><span class="sxs-lookup"><span data-stu-id="1c8d6-149">Font size.</span></span>|
|<span data-ttu-id="1c8d6-150">underline</span><span class="sxs-lookup"><span data-stu-id="1c8d6-150">underline</span></span>|<span data-ttu-id="1c8d6-151">string</span><span class="sxs-lookup"><span data-stu-id="1c8d6-151">string</span></span>|<span data-ttu-id="1c8d6-p106">Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p106">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="1c8d6-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c8d6-154">Response</span></span>

<span data-ttu-id="1c8d6-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFont](../resources/rangefont.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-155">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c8d6-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c8d6-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c8d6-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c8d6-157">Request</span></span>
<span data-ttu-id="1c8d6-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="1c8d6-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c8d6-159">Response</span></span>
<span data-ttu-id="1c8d6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c8d6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangefont-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

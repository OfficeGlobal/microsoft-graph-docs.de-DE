---
title: Arbeitsblatt aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.
ms.openlocfilehash: 16db37919009dbd935bcd8959111f888ffa97d2e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061943"
---
# <a name="update-worksheet"></a><span data-ttu-id="34a97-103">Arbeitsblatt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="34a97-103">Update worksheet</span></span>

> <span data-ttu-id="34a97-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34a97-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34a97-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a97-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34a97-106">Dient zum Aktualisieren der Eigenschaften des Arbeitsblattobjekts.</span><span class="sxs-lookup"><span data-stu-id="34a97-106">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34a97-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34a97-107">Permissions</span></span>
<span data-ttu-id="34a97-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a97-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34a97-110">Permission type</span></span>      | <span data-ttu-id="34a97-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34a97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34a97-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34a97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34a97-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a97-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34a97-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34a97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34a97-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34a97-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34a97-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34a97-116">Application</span></span> | <span data-ttu-id="34a97-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34a97-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34a97-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34a97-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="34a97-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34a97-119">Optional request headers</span></span>
| <span data-ttu-id="34a97-120">Name</span><span class="sxs-lookup"><span data-stu-id="34a97-120">Name</span></span>       | <span data-ttu-id="34a97-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34a97-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="34a97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34a97-122">Authorization</span></span>  | <span data-ttu-id="34a97-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34a97-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34a97-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="34a97-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="34a97-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="34a97-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a97-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34a97-128">Request body</span></span>
<span data-ttu-id="34a97-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="34a97-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34a97-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34a97-132">Property</span></span>     | <span data-ttu-id="34a97-133">Typ</span><span class="sxs-lookup"><span data-stu-id="34a97-133">Type</span></span>   |<span data-ttu-id="34a97-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34a97-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34a97-135">name</span><span class="sxs-lookup"><span data-stu-id="34a97-135">name</span></span>|<span data-ttu-id="34a97-136">string</span><span class="sxs-lookup"><span data-stu-id="34a97-136">string</span></span>|<span data-ttu-id="34a97-137">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="34a97-137">The display name of the worksheet.</span></span>|
|<span data-ttu-id="34a97-138">position</span><span class="sxs-lookup"><span data-stu-id="34a97-138">position</span></span>|<span data-ttu-id="34a97-139">int</span><span class="sxs-lookup"><span data-stu-id="34a97-139">int</span></span>|<span data-ttu-id="34a97-140">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="34a97-140">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="34a97-141">visibility</span><span class="sxs-lookup"><span data-stu-id="34a97-141">visibility</span></span>|<span data-ttu-id="34a97-142">string</span><span class="sxs-lookup"><span data-stu-id="34a97-142">string</span></span>|<span data-ttu-id="34a97-p106">Die Sichtbarkeit des Arbeitsblatts. Mögliche Werte: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="34a97-p106">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="34a97-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="34a97-145">Response</span></span>

<span data-ttu-id="34a97-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Worksheet](../resources/worksheet.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34a97-146">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34a97-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34a97-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34a97-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34a97-148">Request</span></span>
<span data-ttu-id="34a97-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34a97-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="34a97-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="34a97-150">Response</span></span>
<span data-ttu-id="34a97-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34a97-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
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
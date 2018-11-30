---
title: nameditem aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des nameditem-Objekts.
ms.openlocfilehash: 2b298cfe567903e7f470b78021efc34bb379ba35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059151"
---
# <a name="update-nameditem"></a><span data-ttu-id="1d71d-103">nameditem aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1d71d-103">Update nameditem</span></span>

> <span data-ttu-id="1d71d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d71d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d71d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d71d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d71d-106">Dient zum Aktualisieren der Eigenschaften des nameditem-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1d71d-106">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d71d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d71d-107">Permissions</span></span>
<span data-ttu-id="1d71d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d71d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d71d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d71d-110">Permission type</span></span>      | <span data-ttu-id="1d71d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d71d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d71d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d71d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d71d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d71d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d71d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d71d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d71d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d71d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d71d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d71d-116">Application</span></span> | <span data-ttu-id="1d71d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d71d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d71d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d71d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="1d71d-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d71d-119">Optional request headers</span></span>
| <span data-ttu-id="1d71d-120">Name</span><span class="sxs-lookup"><span data-stu-id="1d71d-120">Name</span></span>       | <span data-ttu-id="1d71d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d71d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1d71d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d71d-122">Authorization</span></span>  | <span data-ttu-id="1d71d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d71d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d71d-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1d71d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d71d-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1d71d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d71d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d71d-128">Request body</span></span>
<span data-ttu-id="1d71d-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1d71d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d71d-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d71d-132">Property</span></span>     | <span data-ttu-id="1d71d-133">Typ</span><span class="sxs-lookup"><span data-stu-id="1d71d-133">Type</span></span>   |<span data-ttu-id="1d71d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d71d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d71d-135">visible</span><span class="sxs-lookup"><span data-stu-id="1d71d-135">visible</span></span>|<span data-ttu-id="1d71d-136">boolean</span><span class="sxs-lookup"><span data-stu-id="1d71d-136">boolean</span></span>|<span data-ttu-id="1d71d-137">Gibt an, ob das Objekt sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="1d71d-137">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="1d71d-138">comment</span><span class="sxs-lookup"><span data-stu-id="1d71d-138">comment</span></span>|   <span data-ttu-id="1d71d-139">string</span><span class="sxs-lookup"><span data-stu-id="1d71d-139">string</span></span>  |<span data-ttu-id="1d71d-140">Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="1d71d-140">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="1d71d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d71d-141">Response</span></span>

<span data-ttu-id="1d71d-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [NamedItem](../resources/nameditem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d71d-142">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d71d-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d71d-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d71d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d71d-144">Request</span></span>
<span data-ttu-id="1d71d-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d71d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="1d71d-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d71d-146">Response</span></span>
<span data-ttu-id="1d71d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d71d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

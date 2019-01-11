---
title: Foto aktualisieren
description: Mit dieser API können Sie die Eigenschaften von Fotoobjekten aktualisieren.
localization_priority: Normal
ms.openlocfilehash: 56a8d892ae92f92f5103dc3d88a2f95a5bbb262b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818382"
---
# <a name="update-photo"></a><span data-ttu-id="a6425-103">Foto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6425-103">Update photo</span></span>

> <span data-ttu-id="a6425-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6425-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6425-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6425-106">Mit dieser API können Sie die Eigenschaften von Fotoobjekten aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="a6425-106">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6425-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a6425-107">Permissions</span></span>
<span data-ttu-id="a6425-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6425-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6425-110">Permission type</span></span>      | <span data-ttu-id="a6425-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6425-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6425-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6425-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6425-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6425-113">Not supported.</span></span>    |
|<span data-ttu-id="a6425-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6425-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6425-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6425-115">Not supported.</span></span>    |
|<span data-ttu-id="a6425-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6425-116">Application</span></span> | <span data-ttu-id="a6425-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6425-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6425-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6425-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="a6425-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6425-119">Request headers</span></span>
| <span data-ttu-id="a6425-120">Name</span><span class="sxs-lookup"><span data-stu-id="a6425-120">Name</span></span>       | <span data-ttu-id="a6425-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a6425-121">Type</span></span> | <span data-ttu-id="a6425-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6425-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a6425-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6425-123">Authorization</span></span>  | <span data-ttu-id="a6425-124">string</span><span class="sxs-lookup"><span data-stu-id="a6425-124">string</span></span>  | <span data-ttu-id="a6425-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6425-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6425-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6425-127">Request body</span></span>
<span data-ttu-id="a6425-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a6425-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6425-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6425-131">Property</span></span>     | <span data-ttu-id="a6425-132">Typ</span><span class="sxs-lookup"><span data-stu-id="a6425-132">Type</span></span>   |<span data-ttu-id="a6425-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6425-133">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="a6425-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6425-134">Response</span></span>

<span data-ttu-id="a6425-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6425-135">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6425-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6425-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6425-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6425-137">Request</span></span>
<span data-ttu-id="a6425-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6425-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="a6425-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6425-139">Response</span></span>
<span data-ttu-id="a6425-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6425-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Foto aktualisieren
description: Mit dieser API können Sie die Eigenschaften von Fotoobjekten aktualisieren.
ms.openlocfilehash: 0b062372ac12ec86f3035af276680310191818d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017297"
---
# <a name="update-photo"></a><span data-ttu-id="fac30-103">Foto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fac30-103">Update photo</span></span>

<span data-ttu-id="fac30-104">Mit dieser API können Sie die Eigenschaften von Fotoobjekten aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fac30-104">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fac30-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fac30-105">Permissions</span></span>
<span data-ttu-id="fac30-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fac30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fac30-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fac30-108">Permission type</span></span>      | <span data-ttu-id="fac30-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fac30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fac30-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fac30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fac30-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fac30-111">Not supported.</span></span>    |
|<span data-ttu-id="fac30-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fac30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fac30-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fac30-113">Not supported.</span></span>    |
|<span data-ttu-id="fac30-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fac30-114">Application</span></span> | <span data-ttu-id="fac30-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fac30-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fac30-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fac30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="fac30-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fac30-117">Request headers</span></span>
| <span data-ttu-id="fac30-118">Name</span><span class="sxs-lookup"><span data-stu-id="fac30-118">Name</span></span>       | <span data-ttu-id="fac30-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fac30-119">Type</span></span> | <span data-ttu-id="fac30-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fac30-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fac30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fac30-121">Authorization</span></span>  | <span data-ttu-id="fac30-122">string</span><span class="sxs-lookup"><span data-stu-id="fac30-122">string</span></span>  | <span data-ttu-id="fac30-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fac30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fac30-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fac30-125">Request body</span></span>
<span data-ttu-id="fac30-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="fac30-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fac30-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fac30-129">Property</span></span>     | <span data-ttu-id="fac30-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fac30-130">Type</span></span>   |<span data-ttu-id="fac30-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fac30-131">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="fac30-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fac30-132">Response</span></span>

<span data-ttu-id="fac30-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fac30-133">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fac30-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fac30-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fac30-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fac30-135">Request</span></span>
<span data-ttu-id="fac30-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fac30-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="fac30-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="fac30-137">Response</span></span>
<span data-ttu-id="fac30-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fac30-138">Here is an example of the response.</span></span>
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

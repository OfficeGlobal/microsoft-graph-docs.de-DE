---
title: Vereinbarung aktualisieren
description: Aktualisieren Sie die Eigenschaften eines Objekts zu.
localization_priority: Normal
ms.openlocfilehash: fc6e4718a026f78a6e892dc13095492099b654cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520067"
---
# <a name="update-agreement"></a><span data-ttu-id="38804-103">Vereinbarung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="38804-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38804-104">Aktualisieren Sie die Eigenschaften eines Objekts [zu](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="38804-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38804-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38804-105">Permissions</span></span>
<span data-ttu-id="38804-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38804-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38804-108">Permission type</span></span>                        | <span data-ttu-id="38804-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38804-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38804-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38804-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38804-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38804-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="38804-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38804-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38804-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38804-113">Not supported.</span></span> |
|<span data-ttu-id="38804-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38804-114">Application</span></span>                            | <span data-ttu-id="38804-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38804-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38804-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38804-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="38804-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38804-117">Request headers</span></span>
| <span data-ttu-id="38804-118">Name</span><span class="sxs-lookup"><span data-stu-id="38804-118">Name</span></span>         | <span data-ttu-id="38804-119">Typ</span><span class="sxs-lookup"><span data-stu-id="38804-119">Type</span></span>        | <span data-ttu-id="38804-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38804-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="38804-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38804-121">Authorization</span></span> | <span data-ttu-id="38804-122">string</span><span class="sxs-lookup"><span data-stu-id="38804-122">string</span></span> | <span data-ttu-id="38804-123">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="38804-123">Bearer \{token\}.</span></span> <span data-ttu-id="38804-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38804-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38804-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38804-125">Request body</span></span>
<span data-ttu-id="38804-126">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="38804-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="38804-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="38804-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="38804-128">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="38804-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38804-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38804-129">Property</span></span>     | <span data-ttu-id="38804-130">Typ</span><span class="sxs-lookup"><span data-stu-id="38804-130">Type</span></span>        | <span data-ttu-id="38804-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38804-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38804-132">displayName</span><span class="sxs-lookup"><span data-stu-id="38804-132">displayName</span></span>|<span data-ttu-id="38804-133">String</span><span class="sxs-lookup"><span data-stu-id="38804-133">String</span></span>|<span data-ttu-id="38804-134">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="38804-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="38804-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="38804-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="38804-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="38804-136">Boolean</span></span>|<span data-ttu-id="38804-137">Gibt an, ob der Benutzer hat zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="38804-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="38804-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="38804-138">Response</span></span>
<span data-ttu-id="38804-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [Vereinbarung](../resources/agreement.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="38804-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38804-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38804-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38804-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38804-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="38804-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="38804-142">Response</span></span>
><span data-ttu-id="38804-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="38804-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

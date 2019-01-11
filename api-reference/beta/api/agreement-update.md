---
title: Vereinbarung aktualisieren
description: Aktualisieren Sie die Eigenschaften eines Objekts zu.
localization_priority: Normal
ms.openlocfilehash: b16a503b33193fa453ca52481854879ae4dcd121
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838731"
---
# <a name="update-agreement"></a><span data-ttu-id="08e7a-103">Vereinbarung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="08e7a-103">Update agreement</span></span>

> <span data-ttu-id="08e7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08e7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08e7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08e7a-106">Aktualisieren Sie die Eigenschaften eines Objekts [zu](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="08e7a-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08e7a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="08e7a-107">Permissions</span></span>
<span data-ttu-id="08e7a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e7a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08e7a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08e7a-110">Permission type</span></span>                        | <span data-ttu-id="08e7a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08e7a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="08e7a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08e7a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="08e7a-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e7a-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="08e7a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08e7a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e7a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e7a-115">Not supported.</span></span> |
|<span data-ttu-id="08e7a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08e7a-116">Application</span></span>                            | <span data-ttu-id="08e7a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e7a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08e7a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e7a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="08e7a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08e7a-119">Request headers</span></span>
| <span data-ttu-id="08e7a-120">Name</span><span class="sxs-lookup"><span data-stu-id="08e7a-120">Name</span></span>         | <span data-ttu-id="08e7a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="08e7a-121">Type</span></span>        | <span data-ttu-id="08e7a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e7a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="08e7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08e7a-123">Authorization</span></span> | <span data-ttu-id="08e7a-124">string</span><span class="sxs-lookup"><span data-stu-id="08e7a-124">string</span></span> | <span data-ttu-id="08e7a-125">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="08e7a-125">Bearer \{token\}.</span></span> <span data-ttu-id="08e7a-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08e7a-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08e7a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08e7a-127">Request body</span></span>
<span data-ttu-id="08e7a-128">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="08e7a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="08e7a-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="08e7a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="08e7a-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="08e7a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="08e7a-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08e7a-131">Property</span></span>     | <span data-ttu-id="08e7a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="08e7a-132">Type</span></span>        | <span data-ttu-id="08e7a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e7a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08e7a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="08e7a-134">displayName</span></span>|<span data-ttu-id="08e7a-135">String</span><span class="sxs-lookup"><span data-stu-id="08e7a-135">String</span></span>|<span data-ttu-id="08e7a-136">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="08e7a-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="08e7a-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="08e7a-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="08e7a-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e7a-138">Boolean</span></span>|<span data-ttu-id="08e7a-139">Gibt an, ob der Benutzer hat zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="08e7a-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="08e7a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e7a-140">Response</span></span>
<span data-ttu-id="08e7a-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [Vereinbarung](../resources/agreement.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="08e7a-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08e7a-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08e7a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08e7a-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e7a-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="08e7a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e7a-144">Response</span></span>
><span data-ttu-id="08e7a-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="08e7a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

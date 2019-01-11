---
title: plannerplandetails aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerplandetails**-Objekts.
localization_priority: Normal
ms.openlocfilehash: 15f811d4dccbfbcfee84f16179ebdb6ea6d3ef37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888396"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="8a0fb-103">plannerplandetails aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8a0fb-103">Update plannerplandetails</span></span>

<span data-ttu-id="8a0fb-104">Dient zum Aktualisieren der Eigenschaften eines **plannerplandetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-104">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a0fb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a0fb-105">Permissions</span></span>
<span data-ttu-id="8a0fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a0fb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a0fb-108">Permission type</span></span>      | <span data-ttu-id="8a0fb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a0fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a0fb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a0fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a0fb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a0fb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a0fb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a0fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a0fb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a0fb-113">Not supported.</span></span>    |
|<span data-ttu-id="8a0fb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a0fb-114">Application</span></span> | <span data-ttu-id="8a0fb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a0fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a0fb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a0fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="8a0fb-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a0fb-117">Optional request headers</span></span>
| <span data-ttu-id="8a0fb-118">Name</span><span class="sxs-lookup"><span data-stu-id="8a0fb-118">Name</span></span>       | <span data-ttu-id="8a0fb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a0fb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8a0fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a0fb-120">Authorization</span></span>  | <span data-ttu-id="8a0fb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a0fb-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="8a0fb-123">If-Match</span></span>  | <span data-ttu-id="8a0fb-p103">Letzter bekannter ETag-Wert für das zu aktualisierende plannerPlanDetails-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a0fb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a0fb-126">Request body</span></span>
<span data-ttu-id="8a0fb-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a0fb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a0fb-130">Property</span></span>     | <span data-ttu-id="8a0fb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8a0fb-131">Type</span></span>   |<span data-ttu-id="8a0fb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a0fb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a0fb-133">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8a0fb-133">categoryDescriptions</span></span>|[<span data-ttu-id="8a0fb-134">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8a0fb-134">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="8a0fb-135">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-135">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="8a0fb-136">sharedWith</span><span class="sxs-lookup"><span data-stu-id="8a0fb-136">sharedWith</span></span>|[<span data-ttu-id="8a0fb-137">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="8a0fb-137">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="8a0fb-p105">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](../resources/group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="8a0fb-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a0fb-141">Response</span></span>

<span data-ttu-id="8a0fb-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlanDetails](../resources/plannerplandetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-142">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="8a0fb-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8a0fb-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a0fb-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a0fb-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a0fb-147">Request</span></span>
<span data-ttu-id="8a0fb-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/details
Content-type: application/json
Content-length: 212
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "sharedWith": {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category3": null,
  }
}
```
##### <a name="response"></a><span data-ttu-id="8a0fb-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a0fb-149">Response</span></span>
<span data-ttu-id="8a0fb-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a0fb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplandetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

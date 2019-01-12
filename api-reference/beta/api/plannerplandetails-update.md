---
title: plannerplandetails aktualisieren
description: Dient zum Aktualisieren der Eigenschaften eines **plannerplandetails**-Objekts.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd42196238fb103021debf8a4fee2f658053a255
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950137"
---
# <a name="update-plannerplandetails"></a><span data-ttu-id="86b05-103">plannerplandetails aktualisieren</span><span class="sxs-lookup"><span data-stu-id="86b05-103">Update plannerplandetails</span></span>

> <span data-ttu-id="86b05-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="86b05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86b05-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86b05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86b05-106">Dient zum Aktualisieren der Eigenschaften eines **plannerplandetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="86b05-106">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86b05-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86b05-107">Permissions</span></span>
<span data-ttu-id="86b05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86b05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86b05-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86b05-110">Permission type</span></span>      | <span data-ttu-id="86b05-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86b05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86b05-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86b05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="86b05-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b05-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86b05-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86b05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86b05-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86b05-115">Not supported.</span></span>    |
|<span data-ttu-id="86b05-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86b05-116">Application</span></span> | <span data-ttu-id="86b05-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86b05-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86b05-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86b05-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="86b05-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86b05-119">Optional request headers</span></span>
| <span data-ttu-id="86b05-120">Name</span><span class="sxs-lookup"><span data-stu-id="86b05-120">Name</span></span>       | <span data-ttu-id="86b05-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86b05-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86b05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86b05-122">Authorization</span></span>  | <span data-ttu-id="86b05-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86b05-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86b05-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="86b05-125">If-Match</span></span>  | <span data-ttu-id="86b05-p104">Letzter bekannter ETag-Wert für das zu aktualisierende plannerPlanDetails-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86b05-p104">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86b05-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86b05-128">Request body</span></span>
<span data-ttu-id="86b05-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="86b05-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86b05-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86b05-132">Property</span></span>     | <span data-ttu-id="86b05-133">Typ</span><span class="sxs-lookup"><span data-stu-id="86b05-133">Type</span></span>   |<span data-ttu-id="86b05-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86b05-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86b05-135">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="86b05-135">categoryDescriptions</span></span>|[<span data-ttu-id="86b05-136">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="86b05-136">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="86b05-137">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="86b05-137">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="86b05-138">sharedWith</span><span class="sxs-lookup"><span data-stu-id="86b05-138">sharedWith</span></span>|[<span data-ttu-id="86b05-139">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="86b05-139">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="86b05-p106">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](../resources/group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="86b05-p106">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="86b05-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="86b05-143">Response</span></span>

<span data-ttu-id="86b05-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlanDetails](../resources/plannerplandetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86b05-144">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="86b05-p107">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="86b05-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="86b05-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86b05-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86b05-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86b05-149">Request</span></span>
<span data-ttu-id="86b05-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86b05-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
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
##### <a name="response"></a><span data-ttu-id="86b05-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="86b05-151">Response</span></span>
<span data-ttu-id="86b05-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86b05-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

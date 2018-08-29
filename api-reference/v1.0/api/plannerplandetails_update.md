# <a name="update-plannerplandetails"></a><span data-ttu-id="174f1-101">plannerplandetails aktualisieren</span><span class="sxs-lookup"><span data-stu-id="174f1-101">Update plannerplandetails</span></span>

<span data-ttu-id="174f1-102">Dient zum Aktualisieren der Eigenschaften eines **plannerplandetails**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="174f1-102">Update the properties of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="174f1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="174f1-103">Permissions</span></span>
<span data-ttu-id="174f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="174f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="174f1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="174f1-106">Permission type</span></span>      | <span data-ttu-id="174f1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="174f1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="174f1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="174f1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="174f1-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="174f1-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="174f1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="174f1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="174f1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="174f1-111">Not supported.</span></span>    |
|<span data-ttu-id="174f1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="174f1-112">Application</span></span> | <span data-ttu-id="174f1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="174f1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="174f1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="174f1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}/details
```
## <a name="optional-request-headers"></a><span data-ttu-id="174f1-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="174f1-115">Optional request headers</span></span>
| <span data-ttu-id="174f1-116">Name</span><span class="sxs-lookup"><span data-stu-id="174f1-116">Name</span></span>       | <span data-ttu-id="174f1-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="174f1-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="174f1-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="174f1-118">Authorization</span></span>  | <span data-ttu-id="174f1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="174f1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="174f1-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="174f1-121">If-Match</span></span>  | <span data-ttu-id="174f1-p103">Letzter bekannter ETag-Wert für das zu aktualisierende plannerPlanDetails-Objekt. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="174f1-p103">Last known ETag value for the plannerPlanDetails to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="174f1-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="174f1-124">Request body</span></span>
<span data-ttu-id="174f1-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="174f1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="174f1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="174f1-128">Property</span></span>     | <span data-ttu-id="174f1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="174f1-129">Type</span></span>   |<span data-ttu-id="174f1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="174f1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="174f1-131">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="174f1-131">categoryDescriptions</span></span>|[<span data-ttu-id="174f1-132">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="174f1-132">plannerCategoryDescriptions</span></span>](../resources/plannercategorydescriptions.md)|<span data-ttu-id="174f1-133">Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.</span><span class="sxs-lookup"><span data-stu-id="174f1-133">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="174f1-134">sharedWith</span><span class="sxs-lookup"><span data-stu-id="174f1-134">sharedWith</span></span>|[<span data-ttu-id="174f1-135">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="174f1-135">plannerUserIds</span></span>](../resources/planneruserids.md)|<span data-ttu-id="174f1-p105">Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](../resources/group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="174f1-p105">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](../resources/group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>|

## <a name="response"></a><span data-ttu-id="174f1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="174f1-139">Response</span></span>

<span data-ttu-id="174f1-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [plannerPlanDetails](../resources/plannerplandetails.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="174f1-140">If successful, this method returns a `200 OK` response code and updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="174f1-p106">Diese Methode kann einen beliebigen [HTTP-Statuscode](../../../concepts/errors.md) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 400, 403, 404, 409 und 412. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="174f1-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="174f1-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="174f1-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="174f1-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="174f1-145">Request</span></span>
<span data-ttu-id="174f1-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="174f1-146">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="174f1-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="174f1-147">Response</span></span>
<span data-ttu-id="174f1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="174f1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
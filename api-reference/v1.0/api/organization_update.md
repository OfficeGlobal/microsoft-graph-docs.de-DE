# <a name="update-organization"></a><span data-ttu-id="f79a9-101">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f79a9-101">Update organization</span></span>

<span data-ttu-id="f79a9-102">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f79a9-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f79a9-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f79a9-103">Permissions</span></span>

<span data-ttu-id="f79a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f79a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f79a9-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f79a9-106">Permission type</span></span>      | <span data-ttu-id="f79a9-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f79a9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f79a9-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f79a9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f79a9-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f79a9-109">Not supported.</span></span>    |
|<span data-ttu-id="f79a9-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f79a9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f79a9-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f79a9-111">Not supported.</span></span>    |
|<span data-ttu-id="f79a9-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f79a9-112">Application</span></span> | <span data-ttu-id="f79a9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f79a9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f79a9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f79a9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="f79a9-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f79a9-115">Request headers</span></span>

| <span data-ttu-id="f79a9-116">Name</span><span class="sxs-lookup"><span data-stu-id="f79a9-116">Name</span></span>       | <span data-ttu-id="f79a9-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f79a9-117">Type</span></span> | <span data-ttu-id="f79a9-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f79a9-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f79a9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f79a9-119">Authorization</span></span>  | <span data-ttu-id="f79a9-120">string</span><span class="sxs-lookup"><span data-stu-id="f79a9-120">string</span></span>  | <span data-ttu-id="f79a9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f79a9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f79a9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f79a9-123">Request body</span></span>
<span data-ttu-id="f79a9-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f79a9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f79a9-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="f79a9-125">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="f79a9-126">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f79a9-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f79a9-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f79a9-127">Property</span></span>     | <span data-ttu-id="f79a9-128">Typ</span><span class="sxs-lookup"><span data-stu-id="f79a9-128">Type</span></span>   |<span data-ttu-id="f79a9-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f79a9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f79a9-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="f79a9-130">assignedPlans</span></span>|<span data-ttu-id="f79a9-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="f79a9-131">AssignedPlan</span></span>|<span data-ttu-id="f79a9-132">Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="f79a9-132">The collection of service plans associated with the tenant. Not nullable.</span></span> <span data-ttu-id="f79a9-133">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-133">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f79a9-134">Ort</span><span class="sxs-lookup"><span data-stu-id="f79a9-134">city</span></span>|<span data-ttu-id="f79a9-135">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-135">String</span></span>|            |
|<span data-ttu-id="f79a9-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="f79a9-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="f79a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f79a9-137">DateTimeOffset</span></span>|<span data-ttu-id="f79a9-138">Uhrzeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="f79a9-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="f79a9-139">country</span><span class="sxs-lookup"><span data-stu-id="f79a9-139">country</span></span>|<span data-ttu-id="f79a9-140">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-140">String</span></span>|            |
|<span data-ttu-id="f79a9-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="f79a9-141">countryLetterCode</span></span>|<span data-ttu-id="f79a9-142">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-142">String</span></span>|            |
|<span data-ttu-id="f79a9-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="f79a9-143">deletionTimestamp</span></span>|<span data-ttu-id="f79a9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f79a9-144">DateTimeOffset</span></span>||
|<span data-ttu-id="f79a9-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="f79a9-145">dirSyncEnabled</span></span>|<span data-ttu-id="f79a9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f79a9-146">Boolean</span></span>|<span data-ttu-id="f79a9-147">**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).</span><span class="sxs-lookup"><span data-stu-id="f79a9-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="f79a9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f79a9-148">displayName</span></span>|<span data-ttu-id="f79a9-149">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-149">String</span></span>|<span data-ttu-id="f79a9-150">Der Anzeigename für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f79a9-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="f79a9-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f79a9-151">marketingNotificationEmails</span></span>|<span data-ttu-id="f79a9-152">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-152">String</span></span>|                                        <span data-ttu-id="f79a9-153">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f79a9-154">objectType</span><span class="sxs-lookup"><span data-stu-id="f79a9-154">objectType</span></span>|<span data-ttu-id="f79a9-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f79a9-155">String</span></span>|<span data-ttu-id="f79a9-156">Eine Zeichenfolge, die den Objekttyp identifiziert.</span><span class="sxs-lookup"><span data-stu-id="f79a9-156">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="f79a9-157">Für Mandanten ist der Wert immer „Unternehmen“.</span><span class="sxs-lookup"><span data-stu-id="f79a9-157">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="f79a9-158">Geerbt von [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f79a9-158">Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="f79a9-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="f79a9-159">postalCode</span></span>|<span data-ttu-id="f79a9-160">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-160">String</span></span>|            |
|<span data-ttu-id="f79a9-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="f79a9-161">preferredLanguage</span></span>|<span data-ttu-id="f79a9-162">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-162">String</span></span>|            |
|<span data-ttu-id="f79a9-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="f79a9-163">provisionedPlans</span></span>|<span data-ttu-id="f79a9-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="f79a9-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="f79a9-165">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f79a9-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="f79a9-166">provisioningErrors</span></span>|<span data-ttu-id="f79a9-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="f79a9-167">ProvisioningError</span></span>|                                        <span data-ttu-id="f79a9-168">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f79a9-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f79a9-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="f79a9-170">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-170">String</span></span>||
|<span data-ttu-id="f79a9-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="f79a9-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="f79a9-172">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-172">String</span></span>||
|<span data-ttu-id="f79a9-173">state</span><span class="sxs-lookup"><span data-stu-id="f79a9-173">state</span></span>|<span data-ttu-id="f79a9-174">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-174">String</span></span>|            |
|<span data-ttu-id="f79a9-175">street</span><span class="sxs-lookup"><span data-stu-id="f79a9-175">street</span></span>|<span data-ttu-id="f79a9-176">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-176">String</span></span>|            |
|<span data-ttu-id="f79a9-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f79a9-177">technicalNotificationMails</span></span>|<span data-ttu-id="f79a9-178">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-178">String</span></span>|                                        <span data-ttu-id="f79a9-179">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f79a9-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="f79a9-180">telephoneNumber</span></span>|<span data-ttu-id="f79a9-181">String</span><span class="sxs-lookup"><span data-stu-id="f79a9-181">String</span></span>|            |
|<span data-ttu-id="f79a9-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="f79a9-182">verifiedDomains</span></span>|<span data-ttu-id="f79a9-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="f79a9-183">VerifiedDomain</span></span>|<span data-ttu-id="f79a9-184">Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="f79a9-184">The collection of domains associated with this tenant. Not nullable.</span></span> <span data-ttu-id="f79a9-185">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f79a9-185">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="f79a9-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="f79a9-186">Response</span></span>

<span data-ttu-id="f79a9-187">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f79a9-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f79a9-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f79a9-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="f79a9-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f79a9-189">Request</span></span>

<span data-ttu-id="f79a9-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f79a9-190">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

### <a name="response"></a><span data-ttu-id="f79a9-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="f79a9-191">Response</span></span>

<span data-ttu-id="f79a9-192">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f79a9-192">Here is an example of the response.</span></span> <span data-ttu-id="f79a9-193">**Hinweis**: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="f79a9-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f79a9-194">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f79a9-194">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

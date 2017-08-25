# <a name="update-organization"></a><span data-ttu-id="f6efc-101">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6efc-101">Update organization</span></span>

<span data-ttu-id="f6efc-102">Mit dieser API können Sie die Eigenschaften der aktuell authentifizierten Organisation aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f6efc-102">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6efc-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f6efc-103">Permissions</span></span>
<span data-ttu-id="f6efc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6efc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6efc-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6efc-106">Permission type</span></span>      | <span data-ttu-id="f6efc-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6efc-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f6efc-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6efc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f6efc-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6efc-109">Not supported.</span></span>    | 
|<span data-ttu-id="f6efc-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6efc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6efc-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6efc-111">Not supported.</span></span>    | 
|<span data-ttu-id="f6efc-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6efc-112">Application</span></span> | <span data-ttu-id="f6efc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6efc-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f6efc-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6efc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="f6efc-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6efc-115">Request headers</span></span>
| <span data-ttu-id="f6efc-116">Name</span><span class="sxs-lookup"><span data-stu-id="f6efc-116">Name</span></span>       | <span data-ttu-id="f6efc-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f6efc-117">Type</span></span> | <span data-ttu-id="f6efc-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6efc-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6efc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6efc-119">Authorization</span></span>  | <span data-ttu-id="f6efc-120">string</span><span class="sxs-lookup"><span data-stu-id="f6efc-120">string</span></span>  | <span data-ttu-id="f6efc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6efc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6efc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6efc-123">Request body</span></span>
<span data-ttu-id="f6efc-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f6efc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f6efc-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6efc-127">Property</span></span>     | <span data-ttu-id="f6efc-128">Typ</span><span class="sxs-lookup"><span data-stu-id="f6efc-128">Type</span></span>   |<span data-ttu-id="f6efc-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6efc-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6efc-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="f6efc-130">assignedPlans</span></span>|<span data-ttu-id="f6efc-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="f6efc-131">AssignedPlan</span></span>|<span data-ttu-id="f6efc-p104">Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind.                            **Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-p104">The collection of service plans associated with the tenant.                            **Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f6efc-134">city</span><span class="sxs-lookup"><span data-stu-id="f6efc-134">city</span></span>|<span data-ttu-id="f6efc-135">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-135">String</span></span>|            |
|<span data-ttu-id="f6efc-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="f6efc-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="f6efc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6efc-137">DateTimeOffset</span></span>|<span data-ttu-id="f6efc-138">Uhrzeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="f6efc-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="f6efc-139">country</span><span class="sxs-lookup"><span data-stu-id="f6efc-139">country</span></span>|<span data-ttu-id="f6efc-140">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-140">String</span></span>|            |
|<span data-ttu-id="f6efc-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="f6efc-141">countryLetterCode</span></span>|<span data-ttu-id="f6efc-142">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-142">String</span></span>|            |
|<span data-ttu-id="f6efc-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="f6efc-143">deletionTimestamp</span></span>|<span data-ttu-id="f6efc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6efc-144">DateTimeOffset</span></span>||
|<span data-ttu-id="f6efc-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="f6efc-145">dirSyncEnabled</span></span>|<span data-ttu-id="f6efc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6efc-146">Boolean</span></span>|<span data-ttu-id="f6efc-147">**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).</span><span class="sxs-lookup"><span data-stu-id="f6efc-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="f6efc-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f6efc-148">displayName</span></span>|<span data-ttu-id="f6efc-149">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-149">String</span></span>|<span data-ttu-id="f6efc-150">Der Anzeigename für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6efc-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="f6efc-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f6efc-151">marketingNotificationEmails</span></span>|<span data-ttu-id="f6efc-152">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-152">String</span></span>|                                        <span data-ttu-id="f6efc-153">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f6efc-154">objectType</span><span class="sxs-lookup"><span data-stu-id="f6efc-154">objectType</span></span>|<span data-ttu-id="f6efc-155">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-155">String</span></span>|<span data-ttu-id="f6efc-p105">Eine Zeichenfolge, die den Objekttyp identifiziert. Für Mandanten ist der Wert immer „Unternehmen“. Geerbt von [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f6efc-p105">A string that identifies the object type. For tenants the value is always “Company”. Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="f6efc-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="f6efc-159">postalCode</span></span>|<span data-ttu-id="f6efc-160">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-160">String</span></span>|            |
|<span data-ttu-id="f6efc-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="f6efc-161">preferredLanguage</span></span>|<span data-ttu-id="f6efc-162">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-162">String</span></span>|            |
|<span data-ttu-id="f6efc-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="f6efc-163">provisionedPlans</span></span>|<span data-ttu-id="f6efc-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="f6efc-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="f6efc-165">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f6efc-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="f6efc-166">provisioningErrors</span></span>|<span data-ttu-id="f6efc-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="f6efc-167">ProvisioningError</span></span>|                                        <span data-ttu-id="f6efc-168">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f6efc-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f6efc-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="f6efc-170">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-170">String</span></span>||
|<span data-ttu-id="f6efc-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="f6efc-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="f6efc-172">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-172">String</span></span>||
|<span data-ttu-id="f6efc-173">state</span><span class="sxs-lookup"><span data-stu-id="f6efc-173">state</span></span>|<span data-ttu-id="f6efc-174">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-174">String</span></span>|            |
|<span data-ttu-id="f6efc-175">street</span><span class="sxs-lookup"><span data-stu-id="f6efc-175">street</span></span>|<span data-ttu-id="f6efc-176">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-176">String</span></span>|            |
|<span data-ttu-id="f6efc-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f6efc-177">technicalNotificationMails</span></span>|<span data-ttu-id="f6efc-178">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-178">String</span></span>|                                        <span data-ttu-id="f6efc-179">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f6efc-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="f6efc-180">telephoneNumber</span></span>|<span data-ttu-id="f6efc-181">String</span><span class="sxs-lookup"><span data-stu-id="f6efc-181">String</span></span>|            |
|<span data-ttu-id="f6efc-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="f6efc-182">verifiedDomains</span></span>|<span data-ttu-id="f6efc-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="f6efc-183">VerifiedDomain</span></span>|<span data-ttu-id="f6efc-p106">Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind.                            **Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6efc-p106">The collection of domains associated with this tenant.                            **Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="f6efc-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6efc-186">Response</span></span>

<span data-ttu-id="f6efc-187">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [organization](../resources/organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6efc-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6efc-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6efc-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6efc-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6efc-189">Request</span></span>
<span data-ttu-id="f6efc-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6efc-190">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f6efc-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6efc-191">Response</span></span>
<span data-ttu-id="f6efc-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6efc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

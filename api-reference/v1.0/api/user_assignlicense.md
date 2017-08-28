# <a name="assignlicense"></a><span data-ttu-id="e0bc8-101">assignLicense</span><span class="sxs-lookup"><span data-stu-id="e0bc8-101">assignLicense</span></span>
<span data-ttu-id="e0bc8-p101">Fügt Abonnements für den Benutzer hinzu bzw. entfernt sie. Sie können auch bestimmte Pläne aktivieren oder deaktivieren, die mit einem Abonnement verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-p101">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0bc8-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0bc8-104">Permissions</span></span>
<span data-ttu-id="e0bc8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e0bc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0bc8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0bc8-107">Permission type</span></span>      | <span data-ttu-id="e0bc8-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0bc8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0bc8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0bc8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e0bc8-110">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0bc8-110">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0bc8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0bc8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0bc8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0bc8-112">Not supported.</span></span>    |
|<span data-ttu-id="e0bc8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0bc8-113">Application</span></span> | <span data-ttu-id="e0bc8-114">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0bc8-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0bc8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0bc8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="e0bc8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0bc8-116">Request headers</span></span>
| <span data-ttu-id="e0bc8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e0bc8-117">Header</span></span>       | <span data-ttu-id="e0bc8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e0bc8-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0bc8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0bc8-119">Authorization</span></span>  | <span data-ttu-id="e0bc8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0bc8-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0bc8-122">Content-Type</span></span>  | <span data-ttu-id="e0bc8-123">application/json</span><span class="sxs-lookup"><span data-stu-id="e0bc8-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0bc8-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0bc8-124">Request body</span></span>
<span data-ttu-id="e0bc8-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e0bc8-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="e0bc8-126">Parameter</span></span>    | <span data-ttu-id="e0bc8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e0bc8-127">Type</span></span>   |<span data-ttu-id="e0bc8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0bc8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0bc8-129">addLicenses</span><span class="sxs-lookup"><span data-stu-id="e0bc8-129">addLicenses</span></span>|<span data-ttu-id="e0bc8-130">AssignedLicense</span><span class="sxs-lookup"><span data-stu-id="e0bc8-130">AssignedLicense</span></span>|<span data-ttu-id="e0bc8-p104">Eine Sammlung von [assignedLicense](../resources/assignedlicense.md)-Objekten, die die hinzuzufügenden Lizenzen angeben. Sie können Pläne deaktivieren, die einer Lizenz zugeordnet sind, indem Sie die **disabledPlans**-Eigenschaft für ein [assignedLicense](../resources/assignedlicense.md)-Objekt festlegen.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-p104">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add. You can disable plans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="e0bc8-133">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="e0bc8-133">removeLicenses</span></span>|<span data-ttu-id="e0bc8-134">Guid</span><span class="sxs-lookup"><span data-stu-id="e0bc8-134">Guid</span></span>|<span data-ttu-id="e0bc8-135">Eine Auflistung von GUIDs, die die zu entfernenden Lizenzen identifizieren.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-135">A collection of GUIDs that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="e0bc8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0bc8-136">Response</span></span>

<span data-ttu-id="e0bc8-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-137">If successful, this method returns `200, OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0bc8-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0bc8-138">Example</span></span>
<span data-ttu-id="e0bc8-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0bc8-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0bc8-140">Request</span></span>
<span data-ttu-id="e0bc8-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "removeLicenses": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ]
}
```

##### <a name="response"></a><span data-ttu-id="e0bc8-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0bc8-142">Response</span></span>
<span data-ttu-id="e0bc8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0bc8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="update-device"></a><span data-ttu-id="48692-101">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="48692-101">Update device</span></span>

<span data-ttu-id="48692-102">Mit dieser API können Sie die Eigenschaften eines registrierten Geräts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="48692-102">Update the properties of a registered device.</span></span>

<span data-ttu-id="48692-103">Nur bestimmte Eigenschaften eines Geräts können über genehmigte Geräteverwaltungs-App (Mobile Device Management, MDM) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="48692-103">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="48692-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48692-104">Permissions</span></span>
<span data-ttu-id="48692-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48692-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48692-107">Permission type</span></span>      | <span data-ttu-id="48692-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48692-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48692-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48692-109">Delegated (work or school account)</span></span> | <span data-ttu-id="48692-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48692-110">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="48692-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48692-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48692-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48692-112">Not supported.</span></span> |
|<span data-ttu-id="48692-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48692-113">Application</span></span> | <span data-ttu-id="48692-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48692-114">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="48692-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48692-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="48692-116">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="48692-116">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48692-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48692-117">Request headers</span></span>
| <span data-ttu-id="48692-118">Name</span><span class="sxs-lookup"><span data-stu-id="48692-118">Name</span></span>       | <span data-ttu-id="48692-119">Typ</span><span class="sxs-lookup"><span data-stu-id="48692-119">Type</span></span> | <span data-ttu-id="48692-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48692-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="48692-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48692-121">Authorization</span></span>  | <span data-ttu-id="48692-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48692-122">string</span></span>  | <span data-ttu-id="48692-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48692-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48692-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48692-125">Request body</span></span>

<span data-ttu-id="48692-126">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="48692-126">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="48692-127">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="48692-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="48692-128">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="48692-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="48692-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48692-129">Property</span></span>     | <span data-ttu-id="48692-130">Typ</span><span class="sxs-lookup"><span data-stu-id="48692-130">Type</span></span>   |<span data-ttu-id="48692-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48692-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48692-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="48692-132">accountEnabled</span></span>|<span data-ttu-id="48692-133">Boolesch</span><span class="sxs-lookup"><span data-stu-id="48692-133">Boolean</span></span>| <span data-ttu-id="48692-134">**true**, wenn das Konto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="48692-134">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="48692-135">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="48692-135">operatingSystem</span></span>|<span data-ttu-id="48692-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48692-136">String</span></span>|<span data-ttu-id="48692-137">Der Typ des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="48692-137">The type of operating system on the device.</span></span>|
|<span data-ttu-id="48692-138">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="48692-138">operatingSystemVersion</span></span>|<span data-ttu-id="48692-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48692-139">String</span></span>|<span data-ttu-id="48692-140">Die Version des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="48692-140">The version of the operating system on the device</span></span>|
|<span data-ttu-id="48692-141">displayName</span><span class="sxs-lookup"><span data-stu-id="48692-141">displayName</span></span>|<span data-ttu-id="48692-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48692-142">String</span></span>|<span data-ttu-id="48692-143">Der Anzeigename für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="48692-143">The display name for the device.</span></span>|
|<span data-ttu-id="48692-144">isCompliant</span><span class="sxs-lookup"><span data-stu-id="48692-144">isCompliant</span></span>|<span data-ttu-id="48692-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="48692-145">Boolean</span></span>|<span data-ttu-id="48692-146">**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="48692-146">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="48692-147">Die Aktualisierung kann für ein beliebiges Geräte-Betriebssystem nur durch Intune oder für Geräte mit Windows-Betriebssystem durch eine [genehmigte MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) erfolgen.</span><span class="sxs-lookup"><span data-stu-id="48692-147">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="48692-148">isManaged</span><span class="sxs-lookup"><span data-stu-id="48692-148">isManaged</span></span>|<span data-ttu-id="48692-149">Boolesch</span><span class="sxs-lookup"><span data-stu-id="48692-149">Boolean</span></span>|<span data-ttu-id="48692-150">**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="48692-150">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="48692-151">Die Aktualisierung kann für ein beliebiges Geräte-Betriebssystem nur durch Intune oder für Geräte mit Windows-Betriebssystem durch eine [genehmigte MDM-App](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) erfolgen.</span><span class="sxs-lookup"><span data-stu-id="48692-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="48692-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="48692-152">Response</span></span>

<span data-ttu-id="48692-153">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48692-153">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48692-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48692-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48692-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48692-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="48692-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="48692-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

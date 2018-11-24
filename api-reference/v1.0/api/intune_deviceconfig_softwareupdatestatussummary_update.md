# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="9015c-101">softwareUpdateStatusSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9015c-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="9015c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9015c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9015c-103">Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9015c-103">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9015c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9015c-104">Prerequisites</span></span>
<span data-ttu-id="9015c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9015c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9015c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9015c-107">Permission type</span></span>|<span data-ttu-id="9015c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9015c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9015c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9015c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9015c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9015c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9015c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9015c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9015c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9015c-112">Not supported.</span></span>|
|<span data-ttu-id="9015c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9015c-113">Application</span></span>|<span data-ttu-id="9015c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9015c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9015c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9015c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="9015c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9015c-116">Request headers</span></span>
|<span data-ttu-id="9015c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9015c-117">Header</span></span>|<span data-ttu-id="9015c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9015c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9015c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9015c-119">Authorization</span></span>|<span data-ttu-id="9015c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9015c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9015c-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9015c-121">Accept</span></span>|<span data-ttu-id="9015c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9015c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9015c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9015c-123">Request body</span></span>
<span data-ttu-id="9015c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="9015c-124">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="9015c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9015c-125">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="9015c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9015c-126">Property</span></span>|<span data-ttu-id="9015c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9015c-127">Type</span></span>|<span data-ttu-id="9015c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9015c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9015c-129">id</span><span class="sxs-lookup"><span data-stu-id="9015c-129">id</span></span>|<span data-ttu-id="9015c-130">String</span><span class="sxs-lookup"><span data-stu-id="9015c-130">String</span></span>|<span data-ttu-id="9015c-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9015c-131">Key of the entity.</span></span>|
|<span data-ttu-id="9015c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9015c-132">displayName</span></span>|<span data-ttu-id="9015c-133">String</span><span class="sxs-lookup"><span data-stu-id="9015c-133">String</span></span>|<span data-ttu-id="9015c-134">Der Name der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9015c-134">The name of the policy.</span></span>|
|<span data-ttu-id="9015c-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-135">compliantDeviceCount</span></span>|<span data-ttu-id="9015c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-136">Int32</span></span>|<span data-ttu-id="9015c-137">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="9015c-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="9015c-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9015c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-139">Int32</span></span>|<span data-ttu-id="9015c-140">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="9015c-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="9015c-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-141">remediatedDeviceCount</span></span>|<span data-ttu-id="9015c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-142">Int32</span></span>|<span data-ttu-id="9015c-143">Anzahl korrigierter Geräte</span><span class="sxs-lookup"><span data-stu-id="9015c-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="9015c-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-144">errorDeviceCount</span></span>|<span data-ttu-id="9015c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-145">Int32</span></span>|<span data-ttu-id="9015c-146">Anzahl der Geräte mit Fehler</span><span class="sxs-lookup"><span data-stu-id="9015c-146">Number of devices had error.</span></span>|
|<span data-ttu-id="9015c-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-147">unknownDeviceCount</span></span>|<span data-ttu-id="9015c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-148">Int32</span></span>|<span data-ttu-id="9015c-149">Anzahl unbekannter Geräte</span><span class="sxs-lookup"><span data-stu-id="9015c-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="9015c-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-150">conflictDeviceCount</span></span>|<span data-ttu-id="9015c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-151">Int32</span></span>|<span data-ttu-id="9015c-152">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="9015c-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="9015c-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9015c-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="9015c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-154">Int32</span></span>|<span data-ttu-id="9015c-155">Anzahl nicht anwendbarer Geräte</span><span class="sxs-lookup"><span data-stu-id="9015c-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="9015c-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-156">compliantUserCount</span></span>|<span data-ttu-id="9015c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-157">Int32</span></span>|<span data-ttu-id="9015c-158">Anzahl der kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="9015c-158">Number of compliant users.</span></span>|
|<span data-ttu-id="9015c-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-159">nonCompliantUserCount</span></span>|<span data-ttu-id="9015c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-160">Int32</span></span>|<span data-ttu-id="9015c-161">Anzahl der nicht kompatiblen Benutzer</span><span class="sxs-lookup"><span data-stu-id="9015c-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="9015c-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-162">remediatedUserCount</span></span>|<span data-ttu-id="9015c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-163">Int32</span></span>|<span data-ttu-id="9015c-164">Anzahl der korrigierten Benutzer</span><span class="sxs-lookup"><span data-stu-id="9015c-164">Number of remediated users.</span></span>|
|<span data-ttu-id="9015c-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-165">errorUserCount</span></span>|<span data-ttu-id="9015c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-166">Int32</span></span>|<span data-ttu-id="9015c-167">Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="9015c-167">Number of users had error.</span></span>|
|<span data-ttu-id="9015c-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-168">unknownUserCount</span></span>|<span data-ttu-id="9015c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-169">Int32</span></span>|<span data-ttu-id="9015c-170">Anzahl der unbekannten Benutzer</span><span class="sxs-lookup"><span data-stu-id="9015c-170">Number of unknown users.</span></span>|
|<span data-ttu-id="9015c-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-171">conflictUserCount</span></span>|<span data-ttu-id="9015c-172">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-172">Int32</span></span>|<span data-ttu-id="9015c-173">Anzahl der Benutzer mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="9015c-173">Number of conflict users.</span></span>|
|<span data-ttu-id="9015c-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="9015c-174">notApplicableUserCount</span></span>|<span data-ttu-id="9015c-175">Int32</span><span class="sxs-lookup"><span data-stu-id="9015c-175">Int32</span></span>|<span data-ttu-id="9015c-176">Anzahl der nicht anwendbaren Benutzer.</span><span class="sxs-lookup"><span data-stu-id="9015c-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="9015c-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="9015c-177">Response</span></span>
<span data-ttu-id="9015c-178">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9015c-178">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9015c-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9015c-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="9015c-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9015c-180">Request</span></span>
<span data-ttu-id="9015c-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9015c-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="9015c-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="9015c-182">Response</span></span>
<span data-ttu-id="9015c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9015c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```




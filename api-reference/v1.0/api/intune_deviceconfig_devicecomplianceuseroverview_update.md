# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="f5716-101">Aktualisieren von „deviceComplianceUserOverview“</span><span class="sxs-lookup"><span data-stu-id="f5716-101">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="f5716-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f5716-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5716-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f5716-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5716-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f5716-104">Prerequisites</span></span>
<span data-ttu-id="f5716-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f5716-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f5716-107">Permission type</span></span>|<span data-ttu-id="f5716-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f5716-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5716-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f5716-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f5716-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5716-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5716-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f5716-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5716-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5716-112">Not supported.</span></span>|
|<span data-ttu-id="f5716-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f5716-113">Application</span></span>|<span data-ttu-id="f5716-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f5716-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5716-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5716-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f5716-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f5716-116">Request headers</span></span>
|<span data-ttu-id="f5716-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f5716-117">Header</span></span>|<span data-ttu-id="f5716-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f5716-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5716-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5716-119">Authorization</span></span>|<span data-ttu-id="f5716-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f5716-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f5716-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f5716-121">Accept</span></span>|<span data-ttu-id="f5716-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f5716-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5716-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f5716-123">Request body</span></span>
<span data-ttu-id="f5716-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="f5716-124">In the request body, supply a JSON representation of [message](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="f5716-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f5716-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f5716-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f5716-126">Property</span></span>|<span data-ttu-id="f5716-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f5716-127">Type</span></span>|<span data-ttu-id="f5716-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5716-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5716-129">id</span><span class="sxs-lookup"><span data-stu-id="f5716-129">id</span></span>|<span data-ttu-id="f5716-130">String</span><span class="sxs-lookup"><span data-stu-id="f5716-130">String</span></span>|<span data-ttu-id="f5716-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f5716-131">Key of the setting.</span></span>|
|<span data-ttu-id="f5716-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f5716-132">pendingCount</span></span>|<span data-ttu-id="f5716-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-133">Int32</span></span>|<span data-ttu-id="f5716-134">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="f5716-134">Number of pending Users</span></span>|
|<span data-ttu-id="f5716-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f5716-135">notApplicableCount</span></span>|<span data-ttu-id="f5716-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-136">Int32</span></span>|<span data-ttu-id="f5716-137">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="f5716-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="f5716-138">successCount</span><span class="sxs-lookup"><span data-stu-id="f5716-138">successCount</span></span>|<span data-ttu-id="f5716-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-139">Int32</span></span>|<span data-ttu-id="f5716-140">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="f5716-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="f5716-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="f5716-141">errorCount</span></span>|<span data-ttu-id="f5716-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-142">Int32</span></span>|<span data-ttu-id="f5716-143">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="f5716-143">Number of error Users</span></span>|
|<span data-ttu-id="f5716-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="f5716-144">failedCount</span></span>|<span data-ttu-id="f5716-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-145">Int32</span></span>|<span data-ttu-id="f5716-146">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="f5716-146">Number of failed Users</span></span>|
|<span data-ttu-id="f5716-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f5716-147">lastUpdateDateTime</span></span>|<span data-ttu-id="f5716-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5716-148">DateTimeOffset</span></span>|<span data-ttu-id="f5716-149">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="f5716-149">Last update time</span></span>|
|<span data-ttu-id="f5716-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f5716-150">configurationVersion</span></span>|<span data-ttu-id="f5716-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f5716-151">Int32</span></span>|<span data-ttu-id="f5716-152">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="f5716-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f5716-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5716-153">Response</span></span>
<span data-ttu-id="f5716-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f5716-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5716-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5716-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5716-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5716-156">Request</span></span>
<span data-ttu-id="f5716-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5716-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="f5716-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5716-158">Response</span></span>
<span data-ttu-id="f5716-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5716-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="e75ff-101">Aktualisieren von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="e75ff-101">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="e75ff-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e75ff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e75ff-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e75ff-103">Update the properties of a [calendar](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e75ff-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e75ff-104">Prerequisites</span></span>
<span data-ttu-id="e75ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e75ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e75ff-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e75ff-107">Permission type</span></span>|<span data-ttu-id="e75ff-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e75ff-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e75ff-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e75ff-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e75ff-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e75ff-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e75ff-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e75ff-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e75ff-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e75ff-112">Not supported.</span></span>|
|<span data-ttu-id="e75ff-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e75ff-113">Application</span></span>|<span data-ttu-id="e75ff-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e75ff-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e75ff-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e75ff-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="e75ff-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e75ff-116">Request headers</span></span>
|<span data-ttu-id="e75ff-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e75ff-117">Header</span></span>|<span data-ttu-id="e75ff-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e75ff-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e75ff-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e75ff-119">Authorization</span></span>|<span data-ttu-id="e75ff-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e75ff-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e75ff-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e75ff-121">Accept</span></span>|<span data-ttu-id="e75ff-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e75ff-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e75ff-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e75ff-123">Request body</span></span>
<span data-ttu-id="e75ff-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="e75ff-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="e75ff-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e75ff-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="e75ff-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e75ff-126">Property</span></span>|<span data-ttu-id="e75ff-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e75ff-127">Type</span></span>|<span data-ttu-id="e75ff-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e75ff-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75ff-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e75ff-129">displayName</span></span>|<span data-ttu-id="e75ff-130">String</span><span class="sxs-lookup"><span data-stu-id="e75ff-130">String</span></span>|<span data-ttu-id="e75ff-131">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e75ff-131">Not yet documented</span></span>|
|<span data-ttu-id="e75ff-132">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="e75ff-132">configurationDeployedUserCount</span></span>|<span data-ttu-id="e75ff-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e75ff-133">Int32</span></span>|<span data-ttu-id="e75ff-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e75ff-134">Not yet documented</span></span>|
|<span data-ttu-id="e75ff-135">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="e75ff-135">lastRefreshTime</span></span>|<span data-ttu-id="e75ff-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75ff-136">DateTimeOffset</span></span>|<span data-ttu-id="e75ff-137">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e75ff-137">Not yet documented</span></span>|
|<span data-ttu-id="e75ff-138">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="e75ff-138">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="e75ff-139">Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="e75ff-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="e75ff-140">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e75ff-140">Not yet documented</span></span>|
|<span data-ttu-id="e75ff-141">id</span><span class="sxs-lookup"><span data-stu-id="e75ff-141">id</span></span>|<span data-ttu-id="e75ff-142">String</span><span class="sxs-lookup"><span data-stu-id="e75ff-142">String</span></span>|<span data-ttu-id="e75ff-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e75ff-143">Key of the setting.</span></span>|
|<span data-ttu-id="e75ff-144">version</span><span class="sxs-lookup"><span data-stu-id="e75ff-144">version</span></span>|<span data-ttu-id="e75ff-145">String</span><span class="sxs-lookup"><span data-stu-id="e75ff-145">String</span></span>|<span data-ttu-id="e75ff-146">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="e75ff-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e75ff-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="e75ff-147">Response</span></span>
<span data-ttu-id="e75ff-148">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e75ff-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e75ff-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e75ff-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="e75ff-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e75ff-150">Request</span></span>
<span data-ttu-id="e75ff-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e75ff-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="e75ff-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="e75ff-152">Response</span></span>
<span data-ttu-id="e75ff-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e75ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```




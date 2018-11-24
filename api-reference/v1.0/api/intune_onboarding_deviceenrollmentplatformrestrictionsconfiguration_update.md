# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="e39bb-101">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e39bb-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="e39bb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e39bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e39bb-103">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e39bb-103">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e39bb-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e39bb-104">Prerequisites</span></span>
<span data-ttu-id="e39bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e39bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e39bb-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e39bb-107">Permission type</span></span>|<span data-ttu-id="e39bb-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e39bb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e39bb-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e39bb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e39bb-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39bb-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e39bb-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e39bb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e39bb-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e39bb-112">Not supported.</span></span>|
|<span data-ttu-id="e39bb-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e39bb-113">Application</span></span>|<span data-ttu-id="e39bb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e39bb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e39bb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39bb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e39bb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e39bb-116">Request headers</span></span>
|<span data-ttu-id="e39bb-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e39bb-117">Header</span></span>|<span data-ttu-id="e39bb-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e39bb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e39bb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e39bb-119">Authorization</span></span>|<span data-ttu-id="e39bb-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e39bb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e39bb-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e39bb-121">Accept</span></span>|<span data-ttu-id="e39bb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e39bb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e39bb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e39bb-123">Request body</span></span>
<span data-ttu-id="e39bb-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e39bb-124">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="e39bb-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e39bb-125">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="e39bb-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e39bb-126">Property</span></span>|<span data-ttu-id="e39bb-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e39bb-127">Type</span></span>|<span data-ttu-id="e39bb-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e39bb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39bb-129">id</span><span class="sxs-lookup"><span data-stu-id="e39bb-129">id</span></span>|<span data-ttu-id="e39bb-130">String</span><span class="sxs-lookup"><span data-stu-id="e39bb-130">String</span></span>|<span data-ttu-id="e39bb-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e39bb-132">displayName</span></span>|<span data-ttu-id="e39bb-133">String</span><span class="sxs-lookup"><span data-stu-id="e39bb-133">String</span></span>|<span data-ttu-id="e39bb-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-135">description</span><span class="sxs-lookup"><span data-stu-id="e39bb-135">description</span></span>|<span data-ttu-id="e39bb-136">String</span><span class="sxs-lookup"><span data-stu-id="e39bb-136">String</span></span>|<span data-ttu-id="e39bb-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="e39bb-138">priority</span></span>|<span data-ttu-id="e39bb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e39bb-139">Int32</span></span>|<span data-ttu-id="e39bb-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e39bb-141">createdDateTime</span></span>|<span data-ttu-id="e39bb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39bb-142">DateTimeOffset</span></span>|<span data-ttu-id="e39bb-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e39bb-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e39bb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39bb-145">DateTimeOffset</span></span>|<span data-ttu-id="e39bb-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-147">Version</span><span class="sxs-lookup"><span data-stu-id="e39bb-147">version</span></span>|<span data-ttu-id="e39bb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e39bb-148">Int32</span></span>|<span data-ttu-id="e39bb-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e39bb-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e39bb-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-150">iosRestriction</span></span>|[<span data-ttu-id="e39bb-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e39bb-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e39bb-152">Not yet documented</span></span>|
|<span data-ttu-id="e39bb-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-153">windowsRestriction</span></span>|[<span data-ttu-id="e39bb-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e39bb-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e39bb-155">Not yet documented</span></span>|
|<span data-ttu-id="e39bb-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="e39bb-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e39bb-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e39bb-158">Not yet documented</span></span>|
|<span data-ttu-id="e39bb-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-159">androidRestriction</span></span>|[<span data-ttu-id="e39bb-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e39bb-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e39bb-161">Not yet documented</span></span>|
|<span data-ttu-id="e39bb-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-162">macOSRestriction</span></span>|[<span data-ttu-id="e39bb-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e39bb-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e39bb-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e39bb-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e39bb-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39bb-165">Response</span></span>
<span data-ttu-id="e39bb-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e39bb-166">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e39bb-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e39bb-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="e39bb-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39bb-168">Request</span></span>
<span data-ttu-id="e39bb-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e39bb-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1650

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="e39bb-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39bb-170">Response</span></span>
<span data-ttu-id="e39bb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e39bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




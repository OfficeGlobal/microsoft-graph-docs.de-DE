# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="af6c3-101">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="af6c3-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="af6c3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af6c3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af6c3-103">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="af6c3-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af6c3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af6c3-104">Prerequisites</span></span>
<span data-ttu-id="af6c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af6c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af6c3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af6c3-107">Permission type</span></span>|<span data-ttu-id="af6c3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af6c3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af6c3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af6c3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af6c3-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af6c3-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af6c3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af6c3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af6c3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af6c3-112">Not supported.</span></span>|
|<span data-ttu-id="af6c3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af6c3-113">Application</span></span>|<span data-ttu-id="af6c3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af6c3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af6c3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af6c3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="af6c3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af6c3-116">Request headers</span></span>
|<span data-ttu-id="af6c3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="af6c3-117">Header</span></span>|<span data-ttu-id="af6c3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="af6c3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af6c3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="af6c3-119">Authorization</span></span>|<span data-ttu-id="af6c3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af6c3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af6c3-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af6c3-121">Accept</span></span>|<span data-ttu-id="af6c3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af6c3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af6c3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af6c3-123">Request body</span></span>
<span data-ttu-id="af6c3-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="af6c3-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="af6c3-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="af6c3-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="af6c3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af6c3-126">Property</span></span>|<span data-ttu-id="af6c3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="af6c3-127">Type</span></span>|<span data-ttu-id="af6c3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af6c3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af6c3-129">id</span><span class="sxs-lookup"><span data-stu-id="af6c3-129">id</span></span>|<span data-ttu-id="af6c3-130">String</span><span class="sxs-lookup"><span data-stu-id="af6c3-130">String</span></span>|<span data-ttu-id="af6c3-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="af6c3-132">displayName</span></span>|<span data-ttu-id="af6c3-133">String</span><span class="sxs-lookup"><span data-stu-id="af6c3-133">String</span></span>|<span data-ttu-id="af6c3-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-135">description</span><span class="sxs-lookup"><span data-stu-id="af6c3-135">description</span></span>|<span data-ttu-id="af6c3-136">String</span><span class="sxs-lookup"><span data-stu-id="af6c3-136">String</span></span>|<span data-ttu-id="af6c3-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="af6c3-138">priority</span></span>|<span data-ttu-id="af6c3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="af6c3-139">Int32</span></span>|<span data-ttu-id="af6c3-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af6c3-141">createdDateTime</span></span>|<span data-ttu-id="af6c3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af6c3-142">DateTimeOffset</span></span>|<span data-ttu-id="af6c3-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af6c3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="af6c3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af6c3-145">DateTimeOffset</span></span>|<span data-ttu-id="af6c3-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-147">Version</span><span class="sxs-lookup"><span data-stu-id="af6c3-147">version</span></span>|<span data-ttu-id="af6c3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="af6c3-148">Int32</span></span>|<span data-ttu-id="af6c3-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="af6c3-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="af6c3-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-150">iosRestriction</span></span>|[<span data-ttu-id="af6c3-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="af6c3-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="af6c3-152">Not yet documented</span></span>|
|<span data-ttu-id="af6c3-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-153">windowsRestriction</span></span>|[<span data-ttu-id="af6c3-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="af6c3-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="af6c3-155">Not yet documented</span></span>|
|<span data-ttu-id="af6c3-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="af6c3-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="af6c3-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="af6c3-158">Not yet documented</span></span>|
|<span data-ttu-id="af6c3-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-159">androidRestriction</span></span>|[<span data-ttu-id="af6c3-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="af6c3-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="af6c3-161">Not yet documented</span></span>|
|<span data-ttu-id="af6c3-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-162">macOSRestriction</span></span>|[<span data-ttu-id="af6c3-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="af6c3-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="af6c3-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="af6c3-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="af6c3-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="af6c3-165">Response</span></span>
<span data-ttu-id="af6c3-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af6c3-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af6c3-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af6c3-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="af6c3-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af6c3-168">Request</span></span>
<span data-ttu-id="af6c3-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af6c3-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1626

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="af6c3-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="af6c3-170">Response</span></span>
<span data-ttu-id="af6c3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af6c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




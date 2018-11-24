# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="96824-101">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="96824-101">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="96824-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96824-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96824-103">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="96824-103">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96824-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96824-104">Prerequisites</span></span>
<span data-ttu-id="96824-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96824-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96824-107">Permission type</span></span>|<span data-ttu-id="96824-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96824-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96824-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96824-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96824-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96824-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96824-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96824-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96824-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96824-112">Not supported.</span></span>|
|<span data-ttu-id="96824-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96824-113">Application</span></span>|<span data-ttu-id="96824-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96824-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96824-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96824-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96824-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96824-116">Request headers</span></span>
|<span data-ttu-id="96824-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="96824-117">Header</span></span>|<span data-ttu-id="96824-118">Wert</span><span class="sxs-lookup"><span data-stu-id="96824-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96824-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="96824-119">Authorization</span></span>|<span data-ttu-id="96824-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96824-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96824-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="96824-121">Accept</span></span>|<span data-ttu-id="96824-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96824-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96824-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96824-123">Request body</span></span>
<span data-ttu-id="96824-124">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="96824-124">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="96824-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="96824-125">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="96824-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96824-126">Property</span></span>|<span data-ttu-id="96824-127">Typ</span><span class="sxs-lookup"><span data-stu-id="96824-127">Type</span></span>|<span data-ttu-id="96824-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96824-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96824-129">id</span><span class="sxs-lookup"><span data-stu-id="96824-129">id</span></span>|<span data-ttu-id="96824-130">String</span><span class="sxs-lookup"><span data-stu-id="96824-130">String</span></span>|<span data-ttu-id="96824-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-132">displayName</span><span class="sxs-lookup"><span data-stu-id="96824-132">displayName</span></span>|<span data-ttu-id="96824-133">String</span><span class="sxs-lookup"><span data-stu-id="96824-133">String</span></span>|<span data-ttu-id="96824-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-135">description</span><span class="sxs-lookup"><span data-stu-id="96824-135">description</span></span>|<span data-ttu-id="96824-136">String</span><span class="sxs-lookup"><span data-stu-id="96824-136">String</span></span>|<span data-ttu-id="96824-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="96824-138">priority</span></span>|<span data-ttu-id="96824-139">Int32</span><span class="sxs-lookup"><span data-stu-id="96824-139">Int32</span></span>|<span data-ttu-id="96824-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96824-141">createdDateTime</span></span>|<span data-ttu-id="96824-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96824-142">DateTimeOffset</span></span>|<span data-ttu-id="96824-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96824-144">lastModifiedDateTime</span></span>|<span data-ttu-id="96824-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96824-145">DateTimeOffset</span></span>|<span data-ttu-id="96824-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-147">Version</span><span class="sxs-lookup"><span data-stu-id="96824-147">version</span></span>|<span data-ttu-id="96824-148">Int32</span><span class="sxs-lookup"><span data-stu-id="96824-148">Int32</span></span>|<span data-ttu-id="96824-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96824-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="96824-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-150">iosRestriction</span></span>|[<span data-ttu-id="96824-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="96824-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96824-152">Not yet documented</span></span>|
|<span data-ttu-id="96824-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-153">windowsRestriction</span></span>|[<span data-ttu-id="96824-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="96824-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96824-155">Not yet documented</span></span>|
|<span data-ttu-id="96824-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="96824-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="96824-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96824-158">Not yet documented</span></span>|
|<span data-ttu-id="96824-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-159">androidRestriction</span></span>|[<span data-ttu-id="96824-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="96824-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96824-161">Not yet documented</span></span>|
|<span data-ttu-id="96824-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-162">macOSRestriction</span></span>|[<span data-ttu-id="96824-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="96824-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="96824-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="96824-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="96824-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="96824-165">Response</span></span>
<span data-ttu-id="96824-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="96824-166">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96824-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96824-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="96824-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96824-168">Request</span></span>
<span data-ttu-id="96824-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96824-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="96824-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="96824-170">Response</span></span>
<span data-ttu-id="96824-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96824-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="d0e15-101">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d0e15-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="d0e15-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d0e15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0e15-103">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d0e15-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0e15-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d0e15-104">Prerequisites</span></span>
<span data-ttu-id="d0e15-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0e15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0e15-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0e15-107">Permission type</span></span>|<span data-ttu-id="d0e15-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0e15-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0e15-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0e15-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0e15-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0e15-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0e15-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0e15-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0e15-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0e15-112">Not supported.</span></span>|
|<span data-ttu-id="d0e15-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0e15-113">Application</span></span>|<span data-ttu-id="d0e15-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0e15-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0e15-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0e15-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d0e15-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0e15-116">Request headers</span></span>
|<span data-ttu-id="d0e15-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d0e15-117">Header</span></span>|<span data-ttu-id="d0e15-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d0e15-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0e15-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0e15-119">Authorization</span></span>|<span data-ttu-id="d0e15-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d0e15-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0e15-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d0e15-121">Accept</span></span>|<span data-ttu-id="d0e15-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d0e15-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0e15-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0e15-123">Request body</span></span>
<span data-ttu-id="d0e15-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d0e15-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="d0e15-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d0e15-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d0e15-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0e15-126">Property</span></span>|<span data-ttu-id="d0e15-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d0e15-127">Type</span></span>|<span data-ttu-id="d0e15-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0e15-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0e15-129">id</span><span class="sxs-lookup"><span data-stu-id="d0e15-129">id</span></span>|<span data-ttu-id="d0e15-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-130">String</span></span>|<span data-ttu-id="d0e15-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d0e15-132">displayName</span></span>|<span data-ttu-id="d0e15-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-133">String</span></span>|<span data-ttu-id="d0e15-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-135">description</span><span class="sxs-lookup"><span data-stu-id="d0e15-135">description</span></span>|<span data-ttu-id="d0e15-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-136">String</span></span>|<span data-ttu-id="d0e15-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="d0e15-138">priority</span></span>|<span data-ttu-id="d0e15-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-139">Int32</span></span>|<span data-ttu-id="d0e15-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e15-141">createdDateTime</span></span>|<span data-ttu-id="d0e15-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e15-142">DateTimeOffset</span></span>|<span data-ttu-id="d0e15-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0e15-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d0e15-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0e15-145">DateTimeOffset</span></span>|<span data-ttu-id="d0e15-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-147">Version</span><span class="sxs-lookup"><span data-stu-id="d0e15-147">version</span></span>|<span data-ttu-id="d0e15-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-148">Int32</span></span>|<span data-ttu-id="d0e15-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0e15-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0e15-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d0e15-150">pinMinimumLength</span></span>|<span data-ttu-id="d0e15-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-151">Int32</span></span>|<span data-ttu-id="d0e15-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-152">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="d0e15-153">pinMaximumLength</span></span>|<span data-ttu-id="d0e15-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-154">Int32</span></span>|<span data-ttu-id="d0e15-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-155">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d0e15-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="d0e15-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-157">String</span></span>|<span data-ttu-id="d0e15-158">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d0e15-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d0e15-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d0e15-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="d0e15-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-160">String</span></span>|<span data-ttu-id="d0e15-161">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d0e15-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d0e15-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d0e15-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="d0e15-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-163">String</span></span>|<span data-ttu-id="d0e15-164">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="d0e15-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="d0e15-165">state</span><span class="sxs-lookup"><span data-stu-id="d0e15-165">state</span></span>|<span data-ttu-id="d0e15-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-166">String</span></span>|<span data-ttu-id="d0e15-167">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0e15-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d0e15-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="d0e15-168">securityDeviceRequired</span></span>|<span data-ttu-id="d0e15-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d0e15-169">Boolean</span></span>|<span data-ttu-id="d0e15-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-170">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="d0e15-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="d0e15-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d0e15-172">Boolean</span></span>|<span data-ttu-id="d0e15-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-173">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="d0e15-174">remotePassportEnabled</span></span>|<span data-ttu-id="d0e15-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d0e15-175">Boolean</span></span>|<span data-ttu-id="d0e15-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-176">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="d0e15-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="d0e15-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-178">Int32</span></span>|<span data-ttu-id="d0e15-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-179">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="d0e15-180">pinExpirationInDays</span></span>|<span data-ttu-id="d0e15-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d0e15-181">Int32</span></span>|<span data-ttu-id="d0e15-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d0e15-182">Not yet documented</span></span>|
|<span data-ttu-id="d0e15-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="d0e15-183">enhancedBiometricsState</span></span>|<span data-ttu-id="d0e15-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0e15-184">String</span></span>|<span data-ttu-id="d0e15-185">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0e15-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0e15-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0e15-186">Response</span></span>
<span data-ttu-id="d0e15-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d0e15-187">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0e15-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0e15-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0e15-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0e15-189">Request</span></span>
<span data-ttu-id="d0e15-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0e15-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="d0e15-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0e15-191">Response</span></span>
<span data-ttu-id="d0e15-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0e15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```




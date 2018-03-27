# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="00068-101">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="00068-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="00068-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="00068-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00068-103">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="00068-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00068-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00068-104">Prerequisites</span></span>
<span data-ttu-id="00068-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00068-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00068-107">Permission type</span></span>|<span data-ttu-id="00068-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00068-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00068-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00068-109">Delegated (work or school account)</span></span>|<span data-ttu-id="00068-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00068-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="00068-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00068-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00068-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00068-112">Not supported.</span></span>|
|<span data-ttu-id="00068-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00068-113">Application</span></span>|<span data-ttu-id="00068-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00068-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00068-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00068-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00068-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00068-116">Request headers</span></span>
|<span data-ttu-id="00068-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00068-117">Header</span></span>|<span data-ttu-id="00068-118">Wert</span><span class="sxs-lookup"><span data-stu-id="00068-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00068-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="00068-119">Authorization</span></span>|<span data-ttu-id="00068-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00068-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="00068-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00068-121">Accept</span></span>|<span data-ttu-id="00068-122">application/json</span><span class="sxs-lookup"><span data-stu-id="00068-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00068-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00068-123">Request body</span></span>
<span data-ttu-id="00068-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="00068-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="00068-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00068-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="00068-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00068-126">Property</span></span>|<span data-ttu-id="00068-127">Typ</span><span class="sxs-lookup"><span data-stu-id="00068-127">Type</span></span>|<span data-ttu-id="00068-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00068-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00068-129">id</span><span class="sxs-lookup"><span data-stu-id="00068-129">id</span></span>|<span data-ttu-id="00068-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-130">String</span></span>|<span data-ttu-id="00068-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-132">displayName</span><span class="sxs-lookup"><span data-stu-id="00068-132">displayName</span></span>|<span data-ttu-id="00068-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-133">String</span></span>|<span data-ttu-id="00068-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-135">description</span><span class="sxs-lookup"><span data-stu-id="00068-135">description</span></span>|<span data-ttu-id="00068-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-136">String</span></span>|<span data-ttu-id="00068-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="00068-138">priority</span></span>|<span data-ttu-id="00068-139">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-139">Int32</span></span>|<span data-ttu-id="00068-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00068-141">createdDateTime</span></span>|<span data-ttu-id="00068-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00068-142">DateTimeOffset</span></span>|<span data-ttu-id="00068-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00068-144">lastModifiedDateTime</span></span>|<span data-ttu-id="00068-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00068-145">DateTimeOffset</span></span>|<span data-ttu-id="00068-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-147">Version</span><span class="sxs-lookup"><span data-stu-id="00068-147">version</span></span>|<span data-ttu-id="00068-148">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-148">Int32</span></span>|<span data-ttu-id="00068-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00068-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="00068-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="00068-150">pinMinimumLength</span></span>|<span data-ttu-id="00068-151">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-151">Int32</span></span>|<span data-ttu-id="00068-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-152">Not yet documented</span></span>|
|<span data-ttu-id="00068-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="00068-153">pinMaximumLength</span></span>|<span data-ttu-id="00068-154">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-154">Int32</span></span>|<span data-ttu-id="00068-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-155">Not yet documented</span></span>|
|<span data-ttu-id="00068-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="00068-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="00068-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-157">String</span></span>|<span data-ttu-id="00068-158">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="00068-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="00068-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="00068-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="00068-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-160">String</span></span>|<span data-ttu-id="00068-161">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="00068-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="00068-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="00068-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="00068-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-163">String</span></span>|<span data-ttu-id="00068-164">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="00068-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="00068-165">state</span><span class="sxs-lookup"><span data-stu-id="00068-165">state</span></span>|<span data-ttu-id="00068-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-166">String</span></span>|<span data-ttu-id="00068-167">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00068-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="00068-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="00068-168">securityDeviceRequired</span></span>|<span data-ttu-id="00068-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00068-169">Boolean</span></span>|<span data-ttu-id="00068-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-170">Not yet documented</span></span>|
|<span data-ttu-id="00068-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="00068-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="00068-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00068-172">Boolean</span></span>|<span data-ttu-id="00068-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-173">Not yet documented</span></span>|
|<span data-ttu-id="00068-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="00068-174">remotePassportEnabled</span></span>|<span data-ttu-id="00068-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00068-175">Boolean</span></span>|<span data-ttu-id="00068-176">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-176">Not yet documented</span></span>|
|<span data-ttu-id="00068-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="00068-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="00068-178">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-178">Int32</span></span>|<span data-ttu-id="00068-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-179">Not yet documented</span></span>|
|<span data-ttu-id="00068-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="00068-180">pinExpirationInDays</span></span>|<span data-ttu-id="00068-181">Int32</span><span class="sxs-lookup"><span data-stu-id="00068-181">Int32</span></span>|<span data-ttu-id="00068-182">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="00068-182">Not yet documented</span></span>|
|<span data-ttu-id="00068-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="00068-183">enhancedBiometricsState</span></span>|<span data-ttu-id="00068-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00068-184">String</span></span>|<span data-ttu-id="00068-185">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="00068-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="00068-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="00068-186">Response</span></span>
<span data-ttu-id="00068-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00068-187">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00068-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00068-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="00068-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00068-189">Request</span></span>
<span data-ttu-id="00068-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00068-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 693

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
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

### <a name="response"></a><span data-ttu-id="00068-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="00068-191">Response</span></span>
<span data-ttu-id="00068-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00068-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




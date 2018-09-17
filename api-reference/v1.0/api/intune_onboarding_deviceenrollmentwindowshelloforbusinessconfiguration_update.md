# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="0bebd-101">deviceEnrollmentWindowsHelloForBusinessConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bebd-101">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="0bebd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0bebd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bebd-103">Aktualisieren der Eigenschaften eines [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0bebd-103">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bebd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0bebd-104">Prerequisites</span></span>
<span data-ttu-id="0bebd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0bebd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bebd-107">Permission type</span></span>|<span data-ttu-id="0bebd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bebd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bebd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bebd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0bebd-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bebd-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0bebd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bebd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bebd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bebd-112">Not supported.</span></span>|
|<span data-ttu-id="0bebd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bebd-113">Application</span></span>|<span data-ttu-id="0bebd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bebd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bebd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bebd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0bebd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bebd-116">Request headers</span></span>
|<span data-ttu-id="0bebd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0bebd-117">Header</span></span>|<span data-ttu-id="0bebd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0bebd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bebd-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0bebd-119">Authorization</span></span>|<span data-ttu-id="0bebd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bebd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bebd-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0bebd-121">Accept</span></span>|<span data-ttu-id="0bebd-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="0bebd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bebd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bebd-123">Request body</span></span>
<span data-ttu-id="0bebd-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0bebd-124">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="0bebd-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0bebd-125">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="0bebd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bebd-126">Property</span></span>|<span data-ttu-id="0bebd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0bebd-127">Type</span></span>|<span data-ttu-id="0bebd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bebd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bebd-129">ID</span><span class="sxs-lookup"><span data-stu-id="0bebd-129">id</span></span>|<span data-ttu-id="0bebd-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bebd-130">String</span></span>|<span data-ttu-id="0bebd-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0bebd-132">displayName</span></span>|<span data-ttu-id="0bebd-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bebd-133">String</span></span>|<span data-ttu-id="0bebd-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bebd-135">description</span></span>|<span data-ttu-id="0bebd-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bebd-136">String</span></span>|<span data-ttu-id="0bebd-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="0bebd-138">priority</span></span>|<span data-ttu-id="0bebd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-139">Int32</span></span>|<span data-ttu-id="0bebd-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bebd-141">createdDateTime</span></span>|<span data-ttu-id="0bebd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bebd-142">DateTimeOffset</span></span>|<span data-ttu-id="0bebd-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bebd-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0bebd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bebd-145">DateTimeOffset</span></span>|<span data-ttu-id="0bebd-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-147">Version</span><span class="sxs-lookup"><span data-stu-id="0bebd-147">version</span></span>|<span data-ttu-id="0bebd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-148">Int32</span></span>|<span data-ttu-id="0bebd-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bebd-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0bebd-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0bebd-150">pinMinimumLength</span></span>|<span data-ttu-id="0bebd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-151">Int32</span></span>|<span data-ttu-id="0bebd-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-152">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="0bebd-153">pinMaximumLength</span></span>|<span data-ttu-id="0bebd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-154">Int32</span></span>|<span data-ttu-id="0bebd-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-155">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="0bebd-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="0bebd-p102">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p102">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0bebd-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="0bebd-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="0bebd-p103">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p103">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0bebd-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="0bebd-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="0bebd-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="0bebd-p104">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p104">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0bebd-168">Zustand</span><span class="sxs-lookup"><span data-stu-id="0bebd-168">state</span></span>|[<span data-ttu-id="0bebd-169">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="0bebd-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="0bebd-p105">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p105">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0bebd-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="0bebd-172">securityDeviceRequired</span></span>|<span data-ttu-id="0bebd-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0bebd-173">Boolean</span></span>|<span data-ttu-id="0bebd-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-174">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="0bebd-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="0bebd-176">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0bebd-176">Boolean</span></span>|<span data-ttu-id="0bebd-177">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-177">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="0bebd-178">remotePassportEnabled</span></span>|<span data-ttu-id="0bebd-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0bebd-179">Boolean</span></span>|<span data-ttu-id="0bebd-180">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-180">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="0bebd-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="0bebd-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-182">Int32</span></span>|<span data-ttu-id="0bebd-183">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-183">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="0bebd-184">pinExpirationInDays</span></span>|<span data-ttu-id="0bebd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0bebd-185">Int32</span></span>|<span data-ttu-id="0bebd-186">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0bebd-186">Not yet documented</span></span>|
|<span data-ttu-id="0bebd-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="0bebd-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="0bebd-188">Aktivierung</span><span class="sxs-lookup"><span data-stu-id="0bebd-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="0bebd-p106">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p106">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="0bebd-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bebd-191">Response</span></span>
<span data-ttu-id="0bebd-192">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0bebd-192">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bebd-193">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bebd-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bebd-194">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bebd-194">Request</span></span>
<span data-ttu-id="0bebd-195">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bebd-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0bebd-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bebd-196">Response</span></span>
<span data-ttu-id="0bebd-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bebd-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









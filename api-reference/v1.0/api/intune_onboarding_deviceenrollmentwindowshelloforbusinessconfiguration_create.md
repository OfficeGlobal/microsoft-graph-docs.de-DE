# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1c824-101">deviceEnrollmentWindowsHelloForBusinessConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="1c824-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1c824-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c824-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c824-103">Erstellen eines neuen [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1c824-103">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c824-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c824-104">Prerequisites</span></span>
<span data-ttu-id="1c824-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c824-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c824-107">Permission type</span></span>|<span data-ttu-id="1c824-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c824-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c824-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c824-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c824-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c824-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1c824-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c824-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c824-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c824-112">Not supported.</span></span>|
|<span data-ttu-id="1c824-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c824-113">Application</span></span>|<span data-ttu-id="1c824-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c824-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c824-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c824-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c824-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c824-116">Request headers</span></span>
|<span data-ttu-id="1c824-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c824-117">Header</span></span>|<span data-ttu-id="1c824-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1c824-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c824-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1c824-119">Authorization</span></span>|<span data-ttu-id="1c824-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c824-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c824-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1c824-121">Accept</span></span>|<span data-ttu-id="1c824-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1c824-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c824-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c824-123">Request body</span></span>
<span data-ttu-id="1c824-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentWindowsHelloForBusinessConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1c824-124">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="1c824-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentWindowsHelloForBusinessConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1c824-125">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="1c824-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c824-126">Property</span></span>|<span data-ttu-id="1c824-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1c824-127">Type</span></span>|<span data-ttu-id="1c824-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c824-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c824-129">id</span><span class="sxs-lookup"><span data-stu-id="1c824-129">id</span></span>|<span data-ttu-id="1c824-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c824-130">String</span></span>|<span data-ttu-id="1c824-131">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1c824-132">displayName</span></span>|<span data-ttu-id="1c824-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c824-133">String</span></span>|<span data-ttu-id="1c824-134">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c824-135">description</span></span>|<span data-ttu-id="1c824-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c824-136">String</span></span>|<span data-ttu-id="1c824-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-138">Priorität</span><span class="sxs-lookup"><span data-stu-id="1c824-138">priority</span></span>|<span data-ttu-id="1c824-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-139">Int32</span></span>|<span data-ttu-id="1c824-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c824-141">createdDateTime</span></span>|<span data-ttu-id="1c824-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c824-142">DateTimeOffset</span></span>|<span data-ttu-id="1c824-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c824-144">lastModifiedDateTime</span></span>|<span data-ttu-id="1c824-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c824-145">DateTimeOffset</span></span>|<span data-ttu-id="1c824-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-147">Version</span><span class="sxs-lookup"><span data-stu-id="1c824-147">version</span></span>|<span data-ttu-id="1c824-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-148">Int32</span></span>|<span data-ttu-id="1c824-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c824-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1c824-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1c824-150">pinMinimumLength</span></span>|<span data-ttu-id="1c824-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-151">Int32</span></span>|<span data-ttu-id="1c824-152">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-152">Not yet documented</span></span>|
|<span data-ttu-id="1c824-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1c824-153">pinMaximumLength</span></span>|<span data-ttu-id="1c824-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-154">Int32</span></span>|<span data-ttu-id="1c824-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-155">Not yet documented</span></span>|
|<span data-ttu-id="1c824-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1c824-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="1c824-p102">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1c824-p102">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1c824-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1c824-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="1c824-p103">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1c824-p103">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1c824-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1c824-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="1c824-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="1c824-p104">Noch nicht dokumentiert. Mögliche Werte: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1c824-p104">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1c824-168">Zustand</span><span class="sxs-lookup"><span data-stu-id="1c824-168">state</span></span>|[<span data-ttu-id="1c824-169">enablement</span><span class="sxs-lookup"><span data-stu-id="1c824-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="1c824-p105">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1c824-p105">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1c824-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1c824-172">securityDeviceRequired</span></span>|<span data-ttu-id="1c824-173">boolesch</span><span class="sxs-lookup"><span data-stu-id="1c824-173">Boolean</span></span>|<span data-ttu-id="1c824-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-174">Not yet documented</span></span>|
|<span data-ttu-id="1c824-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1c824-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1c824-176">boolesch</span><span class="sxs-lookup"><span data-stu-id="1c824-176">Boolean</span></span>|<span data-ttu-id="1c824-177">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-177">Not yet documented</span></span>|
|<span data-ttu-id="1c824-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1c824-178">remotePassportEnabled</span></span>|<span data-ttu-id="1c824-179">boolesch</span><span class="sxs-lookup"><span data-stu-id="1c824-179">Boolean</span></span>|<span data-ttu-id="1c824-180">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-180">Not yet documented</span></span>|
|<span data-ttu-id="1c824-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1c824-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="1c824-182">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-182">Int32</span></span>|<span data-ttu-id="1c824-183">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-183">Not yet documented</span></span>|
|<span data-ttu-id="1c824-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1c824-184">pinExpirationInDays</span></span>|<span data-ttu-id="1c824-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1c824-185">Int32</span></span>|<span data-ttu-id="1c824-186">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1c824-186">Not yet documented</span></span>|
|<span data-ttu-id="1c824-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1c824-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="1c824-188">enablement</span><span class="sxs-lookup"><span data-stu-id="1c824-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="1c824-p106">Noch nicht dokumentiert. Mögliche Werte: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1c824-p106">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1c824-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c824-191">Response</span></span>
<span data-ttu-id="1c824-192">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c824-192">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c824-193">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c824-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c824-194">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c824-194">Request</span></span>
<span data-ttu-id="1c824-195">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c824-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c824-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c824-196">Response</span></span>
<span data-ttu-id="1c824-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c824-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









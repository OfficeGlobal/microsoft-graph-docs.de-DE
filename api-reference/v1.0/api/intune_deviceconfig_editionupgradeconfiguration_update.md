# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="58fcd-101">Aktualisieren von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="58fcd-101">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="58fcd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58fcd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58fcd-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-103">Update the properties of a [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58fcd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58fcd-104">Prerequisites</span></span>
<span data-ttu-id="58fcd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58fcd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58fcd-107">Permission type</span></span>|<span data-ttu-id="58fcd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58fcd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58fcd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58fcd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58fcd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58fcd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58fcd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58fcd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58fcd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58fcd-112">Not supported.</span></span>|
|<span data-ttu-id="58fcd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58fcd-113">Application</span></span>|<span data-ttu-id="58fcd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58fcd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58fcd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58fcd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58fcd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58fcd-116">Request headers</span></span>
|<span data-ttu-id="58fcd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58fcd-117">Header</span></span>|<span data-ttu-id="58fcd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="58fcd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58fcd-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="58fcd-119">Authorization</span></span>|<span data-ttu-id="58fcd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58fcd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58fcd-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="58fcd-121">Accept</span></span>|<span data-ttu-id="58fcd-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="58fcd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58fcd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58fcd-123">Request body</span></span>
<span data-ttu-id="58fcd-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="58fcd-124">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="58fcd-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="58fcd-125">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="58fcd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58fcd-126">Property</span></span>|<span data-ttu-id="58fcd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="58fcd-127">Type</span></span>|<span data-ttu-id="58fcd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58fcd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fcd-129">id</span><span class="sxs-lookup"><span data-stu-id="58fcd-129">id</span></span>|<span data-ttu-id="58fcd-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fcd-130">String</span></span>|<span data-ttu-id="58fcd-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="58fcd-131">Key of the entity.</span></span> <span data-ttu-id="58fcd-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58fcd-133">lastModifiedDateTime</span></span>|<span data-ttu-id="58fcd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58fcd-134">DateTimeOffset</span></span>|<span data-ttu-id="58fcd-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58fcd-135">DateTime the object was last modified.</span></span> <span data-ttu-id="58fcd-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58fcd-137">createdDateTime</span></span>|<span data-ttu-id="58fcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58fcd-138">DateTimeOffset</span></span>|<span data-ttu-id="58fcd-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="58fcd-139">DateTime the object was created.</span></span> <span data-ttu-id="58fcd-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-141">description</span><span class="sxs-lookup"><span data-stu-id="58fcd-141">description</span></span>|<span data-ttu-id="58fcd-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fcd-142">String</span></span>|<span data-ttu-id="58fcd-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58fcd-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58fcd-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="58fcd-145">displayName</span></span>|<span data-ttu-id="58fcd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fcd-146">String</span></span>|<span data-ttu-id="58fcd-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="58fcd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58fcd-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-149">Version</span><span class="sxs-lookup"><span data-stu-id="58fcd-149">version</span></span>|<span data-ttu-id="58fcd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="58fcd-150">Int32</span></span>|<span data-ttu-id="58fcd-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="58fcd-151">Version of the device configuration.</span></span> <span data-ttu-id="58fcd-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58fcd-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58fcd-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="58fcd-153">licenseType</span></span>|[<span data-ttu-id="58fcd-154">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="58fcd-154">editionUpgradeLicenseType</span></span>](../resources/intune_deviceconfig_editionupgradelicensetype.md)|<span data-ttu-id="58fcd-155">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="58fcd-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="58fcd-156">Die möglichen Werte sind: `productKey`, `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="58fcd-156">The possible values are:</span></span>|
|<span data-ttu-id="58fcd-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="58fcd-157">targetEdition</span></span>|[<span data-ttu-id="58fcd-158">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="58fcd-158">windows10EditionType</span></span>](../resources/intune_deviceconfig_windows10editiontype.md)|<span data-ttu-id="58fcd-159">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="58fcd-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="58fcd-160">Die möglichen Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="58fcd-160">The possible values are `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, or `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="58fcd-161">license</span><span class="sxs-lookup"><span data-stu-id="58fcd-161">license</span></span>|<span data-ttu-id="58fcd-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fcd-162">String</span></span>|<span data-ttu-id="58fcd-163">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="58fcd-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="58fcd-164">productKey</span><span class="sxs-lookup"><span data-stu-id="58fcd-164">productKey</span></span>|<span data-ttu-id="58fcd-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58fcd-165">String</span></span>|<span data-ttu-id="58fcd-166">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="58fcd-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="58fcd-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="58fcd-167">Response</span></span>
<span data-ttu-id="58fcd-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="58fcd-168">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58fcd-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58fcd-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="58fcd-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58fcd-170">Request</span></span>
<span data-ttu-id="58fcd-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58fcd-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 309

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="58fcd-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="58fcd-172">Response</span></span>
<span data-ttu-id="58fcd-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58fcd-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```




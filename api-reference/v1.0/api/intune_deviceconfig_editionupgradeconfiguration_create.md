# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="3d272-101">Erstellen von „editionUpgradeConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3d272-101">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="3d272-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d272-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d272-103">Diese Methode erstellt ein neues Objekt des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-103">Create a new [plannerBucket](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d272-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d272-104">Prerequisites</span></span>
<span data-ttu-id="3d272-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d272-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d272-107">Permission type</span></span>|<span data-ttu-id="3d272-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d272-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d272-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d272-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3d272-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d272-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d272-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d272-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d272-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d272-112">Not supported.</span></span>|
|<span data-ttu-id="3d272-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d272-113">Application</span></span>|<span data-ttu-id="3d272-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d272-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d272-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d272-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d272-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d272-116">Request headers</span></span>
|<span data-ttu-id="3d272-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d272-117">Header</span></span>|<span data-ttu-id="3d272-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3d272-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d272-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d272-119">Authorization</span></span>|<span data-ttu-id="3d272-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d272-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3d272-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3d272-121">Accept</span></span>|<span data-ttu-id="3d272-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3d272-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d272-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d272-123">Request body</span></span>
<span data-ttu-id="3d272-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „editionUpgradeConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="3d272-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3d272-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „editionUpgradeConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3d272-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3d272-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d272-126">Property</span></span>|<span data-ttu-id="3d272-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3d272-127">Type</span></span>|<span data-ttu-id="3d272-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d272-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d272-129">id</span><span class="sxs-lookup"><span data-stu-id="3d272-129">id</span></span>|<span data-ttu-id="3d272-130">String</span><span class="sxs-lookup"><span data-stu-id="3d272-130">String</span></span>|<span data-ttu-id="3d272-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3d272-131">Key of the setting.</span></span> <span data-ttu-id="3d272-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d272-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3d272-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d272-134">DateTimeOffset</span></span>|<span data-ttu-id="3d272-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d272-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="3d272-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d272-137">createdDateTime</span></span>|<span data-ttu-id="3d272-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d272-138">DateTimeOffset</span></span>|<span data-ttu-id="3d272-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d272-139">DateTime the object was created.</span></span> <span data-ttu-id="3d272-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-141">description</span><span class="sxs-lookup"><span data-stu-id="3d272-141">description</span></span>|<span data-ttu-id="3d272-142">String</span><span class="sxs-lookup"><span data-stu-id="3d272-142">String</span></span>|<span data-ttu-id="3d272-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3d272-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d272-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3d272-145">displayName</span></span>|<span data-ttu-id="3d272-146">String</span><span class="sxs-lookup"><span data-stu-id="3d272-146">String</span></span>|<span data-ttu-id="3d272-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3d272-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d272-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-149">version</span><span class="sxs-lookup"><span data-stu-id="3d272-149">version</span></span>|<span data-ttu-id="3d272-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3d272-150">Int32</span></span>|<span data-ttu-id="3d272-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d272-151">Version of the device configuration.</span></span> <span data-ttu-id="3d272-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d272-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d272-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="3d272-153">licenseType</span></span>|<span data-ttu-id="3d272-154">String</span><span class="sxs-lookup"><span data-stu-id="3d272-154">String</span></span>|<span data-ttu-id="3d272-155">Typ der Edition Upgrade-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="3d272-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="3d272-156">Mögliche Werte sind: `productKey` und `licenseFile`.</span><span class="sxs-lookup"><span data-stu-id="3d272-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="3d272-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="3d272-157">targetEdition</span></span>|<span data-ttu-id="3d272-158">String</span><span class="sxs-lookup"><span data-stu-id="3d272-158">String</span></span>|<span data-ttu-id="3d272-159">Zieledition von Edition Upgrade.</span><span class="sxs-lookup"><span data-stu-id="3d272-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="3d272-160">Mögliche Werte sind: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation` und `windows10ProfessionalWorkstationN`.</span><span class="sxs-lookup"><span data-stu-id="3d272-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="3d272-161">license</span><span class="sxs-lookup"><span data-stu-id="3d272-161">License</span></span>|<span data-ttu-id="3d272-162">String</span><span class="sxs-lookup"><span data-stu-id="3d272-162">String</span></span>|<span data-ttu-id="3d272-163">Inhalt der Edition Upgrade-Lizenzdatei</span><span class="sxs-lookup"><span data-stu-id="3d272-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="3d272-164">productKey</span><span class="sxs-lookup"><span data-stu-id="3d272-164">productKey</span></span>|<span data-ttu-id="3d272-165">String</span><span class="sxs-lookup"><span data-stu-id="3d272-165">String</span></span>|<span data-ttu-id="3d272-166">Product Key von Edition Upgrade</span><span class="sxs-lookup"><span data-stu-id="3d272-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="3d272-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d272-167">Response</span></span>
<span data-ttu-id="3d272-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3d272-168">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d272-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d272-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d272-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d272-170">Request</span></span>
<span data-ttu-id="3d272-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d272-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
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

### <a name="response"></a><span data-ttu-id="3d272-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d272-172">Response</span></span>
<span data-ttu-id="3d272-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d272-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




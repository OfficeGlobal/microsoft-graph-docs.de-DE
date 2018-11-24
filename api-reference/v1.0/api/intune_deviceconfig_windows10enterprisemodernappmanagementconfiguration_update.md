# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="32762-101">Aktualisieren von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="32762-101">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="32762-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="32762-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32762-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-103">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32762-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32762-104">Prerequisites</span></span>
<span data-ttu-id="32762-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32762-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32762-107">Permission type</span></span>|<span data-ttu-id="32762-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32762-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32762-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32762-109">Delegated (work or school account)</span></span>|<span data-ttu-id="32762-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32762-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32762-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32762-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32762-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32762-112">Not supported.</span></span>|
|<span data-ttu-id="32762-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32762-113">Application</span></span>|<span data-ttu-id="32762-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32762-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32762-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32762-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="32762-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32762-116">Request headers</span></span>
|<span data-ttu-id="32762-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32762-117">Header</span></span>|<span data-ttu-id="32762-118">Wert</span><span class="sxs-lookup"><span data-stu-id="32762-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32762-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="32762-119">Authorization</span></span>|<span data-ttu-id="32762-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32762-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32762-121">Accept</span><span class="sxs-lookup"><span data-stu-id="32762-121">Accept</span></span>|<span data-ttu-id="32762-122">application/json</span><span class="sxs-lookup"><span data-stu-id="32762-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32762-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32762-123">Request body</span></span>
<span data-ttu-id="32762-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="32762-124">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="32762-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="32762-125">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="32762-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32762-126">Property</span></span>|<span data-ttu-id="32762-127">Typ</span><span class="sxs-lookup"><span data-stu-id="32762-127">Type</span></span>|<span data-ttu-id="32762-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32762-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32762-129">id</span><span class="sxs-lookup"><span data-stu-id="32762-129">id</span></span>|<span data-ttu-id="32762-130">String</span><span class="sxs-lookup"><span data-stu-id="32762-130">String</span></span>|<span data-ttu-id="32762-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="32762-131">Key of the entity.</span></span> <span data-ttu-id="32762-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32762-133">lastModifiedDateTime</span></span>|<span data-ttu-id="32762-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32762-134">DateTimeOffset</span></span>|<span data-ttu-id="32762-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32762-135">DateTime the object was last modified.</span></span> <span data-ttu-id="32762-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32762-137">createdDateTime</span></span>|<span data-ttu-id="32762-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32762-138">DateTimeOffset</span></span>|<span data-ttu-id="32762-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32762-139">DateTime the object was created.</span></span> <span data-ttu-id="32762-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-141">description</span><span class="sxs-lookup"><span data-stu-id="32762-141">description</span></span>|<span data-ttu-id="32762-142">String</span><span class="sxs-lookup"><span data-stu-id="32762-142">String</span></span>|<span data-ttu-id="32762-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32762-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32762-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-145">displayName</span><span class="sxs-lookup"><span data-stu-id="32762-145">displayName</span></span>|<span data-ttu-id="32762-146">String</span><span class="sxs-lookup"><span data-stu-id="32762-146">String</span></span>|<span data-ttu-id="32762-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32762-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32762-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-149">version</span><span class="sxs-lookup"><span data-stu-id="32762-149">version</span></span>|<span data-ttu-id="32762-150">Int32</span><span class="sxs-lookup"><span data-stu-id="32762-150">Int32</span></span>|<span data-ttu-id="32762-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="32762-151">Version of the device configuration.</span></span> <span data-ttu-id="32762-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32762-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32762-153">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="32762-153">uninstallBuiltInApps</span></span>|<span data-ttu-id="32762-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="32762-154">Boolean</span></span>|<span data-ttu-id="32762-155">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="32762-155">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="32762-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="32762-156">Response</span></span>
<span data-ttu-id="32762-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="32762-157">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32762-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32762-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="32762-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32762-159">Request</span></span>
<span data-ttu-id="32762-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32762-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="32762-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="32762-161">Response</span></span>
<span data-ttu-id="32762-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32762-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```




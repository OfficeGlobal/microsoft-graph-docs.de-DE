# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="a532e-101">Erstellen von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a532e-101">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="a532e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a532e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a532e-103">Diese Methode erstellt ein neues Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-103">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a532e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a532e-104">Prerequisites</span></span>
<span data-ttu-id="a532e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a532e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a532e-107">Permission type</span></span>|<span data-ttu-id="a532e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a532e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a532e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a532e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a532e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a532e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a532e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a532e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a532e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a532e-112">Not supported.</span></span>|
|<span data-ttu-id="a532e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a532e-113">Application</span></span>|<span data-ttu-id="a532e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a532e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a532e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a532e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a532e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a532e-116">Request headers</span></span>
|<span data-ttu-id="a532e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a532e-117">Header</span></span>|<span data-ttu-id="a532e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a532e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a532e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a532e-119">Authorization</span></span>|<span data-ttu-id="a532e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a532e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a532e-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="a532e-121">Accept</span></span>|<span data-ttu-id="a532e-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="a532e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a532e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a532e-123">Request body</span></span>
<span data-ttu-id="a532e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10EnterpriseModernAppManagementConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="a532e-124">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="a532e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10EnterpriseModernAppManagementConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a532e-125">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="a532e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a532e-126">Property</span></span>|<span data-ttu-id="a532e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a532e-127">Type</span></span>|<span data-ttu-id="a532e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a532e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a532e-129">ID</span><span class="sxs-lookup"><span data-stu-id="a532e-129">id</span></span>|<span data-ttu-id="a532e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a532e-130">String</span></span>|<span data-ttu-id="a532e-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a532e-131">Key of the entity.</span></span> <span data-ttu-id="a532e-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a532e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a532e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a532e-134">DateTimeOffset</span></span>|<span data-ttu-id="a532e-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a532e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a532e-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a532e-137">createdDateTime</span></span>|<span data-ttu-id="a532e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a532e-138">DateTimeOffset</span></span>|<span data-ttu-id="a532e-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a532e-139">DateTime the object was created.</span></span> <span data-ttu-id="a532e-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a532e-141">description</span></span>|<span data-ttu-id="a532e-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a532e-142">String</span></span>|<span data-ttu-id="a532e-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a532e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a532e-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a532e-145">displayName</span></span>|<span data-ttu-id="a532e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a532e-146">String</span></span>|<span data-ttu-id="a532e-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a532e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a532e-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-149">Version</span><span class="sxs-lookup"><span data-stu-id="a532e-149">version</span></span>|<span data-ttu-id="a532e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a532e-150">Int32</span></span>|<span data-ttu-id="a532e-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a532e-151">Version of the device configuration.</span></span> <span data-ttu-id="a532e-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a532e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a532e-153">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="a532e-153">uninstallBuiltInApps</span></span>|<span data-ttu-id="a532e-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="a532e-154">Boolean</span></span>|<span data-ttu-id="a532e-155">Gibt an, ob eine festgelegte Liste integrierter Windows-Apps deinstalliert werden soll.</span><span class="sxs-lookup"><span data-stu-id="a532e-155">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="a532e-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="a532e-156">Response</span></span>
<span data-ttu-id="a532e-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a532e-157">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a532e-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a532e-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="a532e-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a532e-159">Request</span></span>
<span data-ttu-id="a532e-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a532e-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 286

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="a532e-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="a532e-161">Response</span></span>
<span data-ttu-id="a532e-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a532e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









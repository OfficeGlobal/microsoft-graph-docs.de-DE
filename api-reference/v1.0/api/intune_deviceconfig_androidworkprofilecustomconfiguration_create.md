# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="fc9b4-101">Erstellen von androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc9b4-101">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="fc9b4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc9b4-103">Erstellen eines neuen [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-103">Create a new [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc9b4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc9b4-104">Prerequisites</span></span>
<span data-ttu-id="fc9b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc9b4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc9b4-107">Permission type</span></span>|<span data-ttu-id="fc9b4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc9b4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc9b4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc9b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fc9b4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc9b4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc9b4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc9b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc9b4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc9b4-112">Not supported.</span></span>|
|<span data-ttu-id="fc9b4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-113">Application</span></span>|<span data-ttu-id="fc9b4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc9b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc9b4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fc9b4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc9b4-116">Request headers</span></span>
|<span data-ttu-id="fc9b4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fc9b4-117">Header</span></span>|<span data-ttu-id="fc9b4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fc9b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc9b4-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-119">Authorization</span></span>|<span data-ttu-id="fc9b4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc9b4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc9b4-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fc9b4-121">Accept</span></span>|<span data-ttu-id="fc9b4-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="fc9b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc9b4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc9b4-123">Request body</span></span>
<span data-ttu-id="fc9b4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des androidWorkProfileCustomConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="fc9b4-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen von androidWorkProfileCustomConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="fc9b4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc9b4-126">Property</span></span>|<span data-ttu-id="fc9b4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fc9b4-127">Type</span></span>|<span data-ttu-id="fc9b4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc9b4-129">ID</span><span class="sxs-lookup"><span data-stu-id="fc9b4-129">id</span></span>|<span data-ttu-id="fc9b4-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc9b4-130">String</span></span>|<span data-ttu-id="fc9b4-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fc9b4-131">Key of the entity.</span></span> <span data-ttu-id="fc9b4-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc9b4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fc9b4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc9b4-134">DateTimeOffset</span></span>|<span data-ttu-id="fc9b4-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-135">DateTime the object was last modified.</span></span> <span data-ttu-id="fc9b4-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc9b4-137">createdDateTime</span></span>|<span data-ttu-id="fc9b4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc9b4-138">DateTimeOffset</span></span>|<span data-ttu-id="fc9b4-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-139">DateTime the object was created.</span></span> <span data-ttu-id="fc9b4-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-141">description</span></span>|<span data-ttu-id="fc9b4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc9b4-142">String</span></span>|<span data-ttu-id="fc9b4-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc9b4-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fc9b4-145">displayName</span></span>|<span data-ttu-id="fc9b4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc9b4-146">String</span></span>|<span data-ttu-id="fc9b4-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc9b4-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-149">Version</span><span class="sxs-lookup"><span data-stu-id="fc9b4-149">version</span></span>|<span data-ttu-id="fc9b4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="fc9b4-150">Int32</span></span>|<span data-ttu-id="fc9b4-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-151">Version of the device configuration.</span></span> <span data-ttu-id="fc9b4-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc9b4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc9b4-153">omaSettings</span><span class="sxs-lookup"><span data-stu-id="fc9b4-153">omaSettings</span></span>|<span data-ttu-id="fc9b4-154">Collection von Objekten des Typs [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc9b4-154">[omaSetting](../resources/intune_deviceconfig_omasetting.md) collection</span></span>|<span data-ttu-id="fc9b4-155">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-155">OMA settings.</span></span> <span data-ttu-id="fc9b4-156">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-156">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fc9b4-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc9b4-157">Response</span></span>
<span data-ttu-id="fc9b4-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und ein [AndroidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-158">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc9b4-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc9b4-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc9b4-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc9b4-160">Request</span></span>
<span data-ttu-id="fc9b4-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 477

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc9b4-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc9b4-162">Response</span></span>
<span data-ttu-id="fc9b4-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc9b4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```









# <a name="update-deviceconfigurationstate"></a><span data-ttu-id="98f7b-101">Aktualisieren von „deviceConfigurationState“</span><span class="sxs-lookup"><span data-stu-id="98f7b-101">Update deviceConfigurationState</span></span>

> <span data-ttu-id="98f7b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="98f7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98f7b-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md).</span><span class="sxs-lookup"><span data-stu-id="98f7b-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98f7b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="98f7b-104">Prerequisites</span></span>
<span data-ttu-id="98f7b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="98f7b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98f7b-107">Permission type</span></span>|<span data-ttu-id="98f7b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98f7b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98f7b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98f7b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="98f7b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f7b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98f7b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98f7b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98f7b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98f7b-112">Not supported.</span></span>|
|<span data-ttu-id="98f7b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98f7b-113">Application</span></span>|<span data-ttu-id="98f7b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98f7b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98f7b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98f7b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /managedDevices/{managedDevicesId}/deviceConfigurationStates/{deviceConfigurationStateId}
```

## <a name="request-headers"></a><span data-ttu-id="98f7b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98f7b-116">Request headers</span></span>
|<span data-ttu-id="98f7b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="98f7b-117">Header</span></span>|<span data-ttu-id="98f7b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="98f7b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98f7b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="98f7b-119">Authorization</span></span>|<span data-ttu-id="98f7b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="98f7b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="98f7b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="98f7b-121">Accept</span></span>|<span data-ttu-id="98f7b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="98f7b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98f7b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98f7b-123">Request body</span></span>
<span data-ttu-id="98f7b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="98f7b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationstate.md) object.</span></span>

<span data-ttu-id="98f7b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="98f7b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="98f7b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98f7b-126">Property</span></span>|<span data-ttu-id="98f7b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="98f7b-127">Type</span></span>|<span data-ttu-id="98f7b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98f7b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98f7b-129">id</span><span class="sxs-lookup"><span data-stu-id="98f7b-129">id</span></span>|<span data-ttu-id="98f7b-130">String</span><span class="sxs-lookup"><span data-stu-id="98f7b-130">String</span></span>|<span data-ttu-id="98f7b-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="98f7b-131">Key of the setting.</span></span>|
|<span data-ttu-id="98f7b-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="98f7b-132">settingStates</span></span>|<span data-ttu-id="98f7b-133">Collection von Objekten des Typs [deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="98f7b-133">[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md) collection</span></span>|<span data-ttu-id="98f7b-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="98f7b-134">Not yet documented</span></span>|
|<span data-ttu-id="98f7b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="98f7b-135">displayName</span></span>|<span data-ttu-id="98f7b-136">String</span><span class="sxs-lookup"><span data-stu-id="98f7b-136">String</span></span>|<span data-ttu-id="98f7b-137">Name der Richtlinie für dieses Objekt des Typs „policyBase“</span><span class="sxs-lookup"><span data-stu-id="98f7b-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="98f7b-138">version</span><span class="sxs-lookup"><span data-stu-id="98f7b-138">version</span></span>|<span data-ttu-id="98f7b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="98f7b-139">Int32</span></span>|<span data-ttu-id="98f7b-140">Version der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="98f7b-140">The version of the message.</span></span>|
|<span data-ttu-id="98f7b-141">platformType</span><span class="sxs-lookup"><span data-stu-id="98f7b-141">PlatformType</span></span>|<span data-ttu-id="98f7b-142">String</span><span class="sxs-lookup"><span data-stu-id="98f7b-142">String</span></span>|<span data-ttu-id="98f7b-143">Plattformtyp, für den die Richtlinie gilt. Mögliche Werte sind: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `all`.</span><span class="sxs-lookup"><span data-stu-id="98f7b-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="98f7b-144">state</span><span class="sxs-lookup"><span data-stu-id="98f7b-144">state</span></span>|<span data-ttu-id="98f7b-145">String</span><span class="sxs-lookup"><span data-stu-id="98f7b-145">String</span></span>|<span data-ttu-id="98f7b-146">Konformitätsstatus der Richtlinie. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error` und `conflict`.</span><span class="sxs-lookup"><span data-stu-id="98f7b-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="98f7b-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="98f7b-147">settingCount</span></span>|<span data-ttu-id="98f7b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="98f7b-148">Int32</span></span>|<span data-ttu-id="98f7b-149">Anzahl der Einstellungen, die eine Richtlinie enthält</span><span class="sxs-lookup"><span data-stu-id="98f7b-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="98f7b-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="98f7b-150">Response</span></span>
<span data-ttu-id="98f7b-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="98f7b-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98f7b-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98f7b-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="98f7b-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98f7b-153">Request</span></span>
<span data-ttu-id="98f7b-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98f7b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceConfigurationStates/{deviceConfigurationStateId}
Content-type: application/json
Content-length: 904

{
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```

### <a name="response"></a><span data-ttu-id="98f7b-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="98f7b-155">Response</span></span>
<span data-ttu-id="98f7b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98f7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1016

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "11692784-2784-1169-8427-691184276911",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```




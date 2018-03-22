# <a name="create-devicecompliancepolicystate"></a><span data-ttu-id="cda00-101">deviceCompliancePolicyState erstellen</span><span class="sxs-lookup"><span data-stu-id="cda00-101">Create deviceCompliancePolicyState</span></span>

> <span data-ttu-id="cda00-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cda00-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cda00-103">Erstellen eines neuen [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cda00-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cda00-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cda00-104">Prerequisites</span></span>
<span data-ttu-id="cda00-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cda00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cda00-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cda00-107">Permission type</span></span>|<span data-ttu-id="cda00-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cda00-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda00-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cda00-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cda00-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda00-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cda00-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cda00-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda00-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda00-112">Not supported.</span></span>|
|<span data-ttu-id="cda00-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cda00-113">Application</span></span>|<span data-ttu-id="cda00-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cda00-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda00-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda00-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a><span data-ttu-id="cda00-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cda00-116">Request headers</span></span>
|<span data-ttu-id="cda00-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cda00-117">Header</span></span>|<span data-ttu-id="cda00-118">Wert</span><span class="sxs-lookup"><span data-stu-id="cda00-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cda00-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cda00-119">Authorization</span></span>|<span data-ttu-id="cda00-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cda00-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cda00-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cda00-121">Accept</span></span>|<span data-ttu-id="cda00-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cda00-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda00-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cda00-123">Request body</span></span>
<span data-ttu-id="cda00-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicyState an.</span><span class="sxs-lookup"><span data-stu-id="cda00-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="cda00-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicyState erstellen.</span><span class="sxs-lookup"><span data-stu-id="cda00-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="cda00-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cda00-126">Property</span></span>|<span data-ttu-id="cda00-127">Typ</span><span class="sxs-lookup"><span data-stu-id="cda00-127">Type</span></span>|<span data-ttu-id="cda00-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cda00-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda00-129">id</span><span class="sxs-lookup"><span data-stu-id="cda00-129">id</span></span>|<span data-ttu-id="cda00-130">String</span><span class="sxs-lookup"><span data-stu-id="cda00-130">String</span></span>|<span data-ttu-id="cda00-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cda00-131">Key of the setting.</span></span>|
|<span data-ttu-id="cda00-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="cda00-132">settingStates</span></span>|<span data-ttu-id="cda00-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="cda00-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) collection</span></span>|<span data-ttu-id="cda00-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="cda00-134">Not yet documented</span></span>|
|<span data-ttu-id="cda00-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cda00-135">displayName</span></span>|<span data-ttu-id="cda00-136">String</span><span class="sxs-lookup"><span data-stu-id="cda00-136">String</span></span>|<span data-ttu-id="cda00-137">Name der Richtlinie für diese policyBase</span><span class="sxs-lookup"><span data-stu-id="cda00-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="cda00-138">Version</span><span class="sxs-lookup"><span data-stu-id="cda00-138">version</span></span>|<span data-ttu-id="cda00-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cda00-139">Int32</span></span>|<span data-ttu-id="cda00-140">Version der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="cda00-140">The version of the message.</span></span>|
|<span data-ttu-id="cda00-141">platformType</span><span class="sxs-lookup"><span data-stu-id="cda00-141">PlatformType</span></span>|<span data-ttu-id="cda00-142">String</span><span class="sxs-lookup"><span data-stu-id="cda00-142">String</span></span>|<span data-ttu-id="cda00-143">Der Plattformtyp, für den die Richtlinie gilt. Mögliche Werte: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="cda00-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="cda00-144">state</span><span class="sxs-lookup"><span data-stu-id="cda00-144">state</span></span>|<span data-ttu-id="cda00-145">String</span><span class="sxs-lookup"><span data-stu-id="cda00-145">String</span></span>|<span data-ttu-id="cda00-146">Der Compliance-Status der Richtlinie. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="cda00-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="cda00-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="cda00-147">settingCount</span></span>|<span data-ttu-id="cda00-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cda00-148">Int32</span></span>|<span data-ttu-id="cda00-149">Anzahl der Einstellungen, die eine Richtlinie enthält</span><span class="sxs-lookup"><span data-stu-id="cda00-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="cda00-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda00-150">Response</span></span>
<span data-ttu-id="cda00-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cda00-151">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda00-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cda00-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="cda00-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cda00-153">Request</span></span>
<span data-ttu-id="cda00-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cda00-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
Content-type: application/json
Content-length: 973

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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

### <a name="response"></a><span data-ttu-id="cda00-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="cda00-155">Response</span></span>
<span data-ttu-id="cda00-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cda00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1022

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "2999e387-e387-2999-87e3-992987e39929",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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




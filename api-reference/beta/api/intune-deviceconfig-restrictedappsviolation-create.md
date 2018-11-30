---
title: Erstellen von restrictedAppsViolation
description: Erstellen eines neuen RestrictedAppsViolation-Objekts.
ms.openlocfilehash: 2d43ddf5ae6c5965f67fdb32c4b242fd0a3f82e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061384"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="e113f-103">Erstellen von restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="e113f-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="e113f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e113f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e113f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e113f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e113f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e113f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e113f-107">Erstellen eines neuen [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e113f-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e113f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e113f-108">Prerequisites</span></span>
<span data-ttu-id="e113f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e113f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e113f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e113f-111">Permission type</span></span>|<span data-ttu-id="e113f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e113f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e113f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e113f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e113f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e113f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e113f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e113f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e113f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e113f-116">Not supported.</span></span>|
|<span data-ttu-id="e113f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e113f-117">Application</span></span>|<span data-ttu-id="e113f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e113f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e113f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e113f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="e113f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e113f-120">Request headers</span></span>
|<span data-ttu-id="e113f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e113f-121">Header</span></span>|<span data-ttu-id="e113f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e113f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e113f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e113f-123">Authorization</span></span>|<span data-ttu-id="e113f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e113f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e113f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e113f-125">Accept</span></span>|<span data-ttu-id="e113f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e113f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e113f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e113f-127">Request body</span></span>
<span data-ttu-id="e113f-128">Geben Sie im Textkörper Anforderung für das Objekt RestrictedAppsViolation eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e113f-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="e113f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die RestrictedAppsViolation erstellen.</span><span class="sxs-lookup"><span data-stu-id="e113f-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="e113f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e113f-130">Property</span></span>|<span data-ttu-id="e113f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e113f-131">Type</span></span>|<span data-ttu-id="e113f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e113f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e113f-133">id</span><span class="sxs-lookup"><span data-stu-id="e113f-133">id</span></span>|<span data-ttu-id="e113f-134">String</span><span class="sxs-lookup"><span data-stu-id="e113f-134">String</span></span>|<span data-ttu-id="e113f-135">Eindeutiger Bezeichner für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="e113f-135">Unique identifier for the object.</span></span> <span data-ttu-id="e113f-136">Besteht aus den AccountId, Geräte-ID, PolicyId und Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="e113f-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="e113f-137">userId</span><span class="sxs-lookup"><span data-stu-id="e113f-137">userId</span></span>|<span data-ttu-id="e113f-138">String</span><span class="sxs-lookup"><span data-stu-id="e113f-138">String</span></span>|<span data-ttu-id="e113f-139">Eindeutige Benutzer-ID muss Guid</span><span class="sxs-lookup"><span data-stu-id="e113f-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e113f-140">userName</span><span class="sxs-lookup"><span data-stu-id="e113f-140">userName</span></span>|<span data-ttu-id="e113f-141">String</span><span class="sxs-lookup"><span data-stu-id="e113f-141">String</span></span>|<span data-ttu-id="e113f-142">Benutzername</span><span class="sxs-lookup"><span data-stu-id="e113f-142">User name</span></span>|
|<span data-ttu-id="e113f-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e113f-143">managedDeviceId</span></span>|<span data-ttu-id="e113f-144">String</span><span class="sxs-lookup"><span data-stu-id="e113f-144">String</span></span>|<span data-ttu-id="e113f-145">Eindeutiger Bezeichner der verwalteten Gerät, muss die Guid</span><span class="sxs-lookup"><span data-stu-id="e113f-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e113f-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="e113f-146">deviceName</span></span>|<span data-ttu-id="e113f-147">String</span><span class="sxs-lookup"><span data-stu-id="e113f-147">String</span></span>|<span data-ttu-id="e113f-148">Gerätename</span><span class="sxs-lookup"><span data-stu-id="e113f-148">Device name</span></span>|
|<span data-ttu-id="e113f-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e113f-149">deviceConfigurationId</span></span>|<span data-ttu-id="e113f-150">String</span><span class="sxs-lookup"><span data-stu-id="e113f-150">String</span></span>|<span data-ttu-id="e113f-151">Gerät Konfiguration Profil Eindeutiger Bezeichner muss Guid</span><span class="sxs-lookup"><span data-stu-id="e113f-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e113f-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="e113f-152">deviceConfigurationName</span></span>|<span data-ttu-id="e113f-153">String</span><span class="sxs-lookup"><span data-stu-id="e113f-153">String</span></span>|<span data-ttu-id="e113f-154">Gerätename Konfiguration-Profil</span><span class="sxs-lookup"><span data-stu-id="e113f-154">Device configuration profile name</span></span>|
|<span data-ttu-id="e113f-155">platformType</span><span class="sxs-lookup"><span data-stu-id="e113f-155">platformType</span></span>|[<span data-ttu-id="e113f-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e113f-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="e113f-157">Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="e113f-157">Platform type.</span></span> <span data-ttu-id="e113f-158">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e113f-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e113f-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e113f-159">restrictedAppsState</span></span>|[<span data-ttu-id="e113f-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e113f-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="e113f-161">Eingeschränkte apps Zustand.</span><span class="sxs-lookup"><span data-stu-id="e113f-161">Restricted apps state.</span></span> <span data-ttu-id="e113f-162">Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="e113f-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="e113f-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e113f-163">restrictedApps</span></span>|<span data-ttu-id="e113f-164">[ManagedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e113f-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="e113f-165">Liste der verletzte eingeschränkte apps</span><span class="sxs-lookup"><span data-stu-id="e113f-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="e113f-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="e113f-166">Response</span></span>
<span data-ttu-id="e113f-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e113f-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e113f-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e113f-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="e113f-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e113f-169">Request</span></span>
<span data-ttu-id="e113f-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e113f-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e113f-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="e113f-171">Response</span></span>
<span data-ttu-id="e113f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e113f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```






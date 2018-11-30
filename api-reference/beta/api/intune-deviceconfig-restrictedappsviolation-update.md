---
title: RestrictedAppsViolation aktualisieren
description: Aktualisieren Sie die Eigenschaften eines RestrictedAppsViolation-Objekts.
ms.openlocfilehash: ad6fcfd8571890a06877f503520533f2907fd3cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058195"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="a6681-103">RestrictedAppsViolation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6681-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="a6681-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6681-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6681-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6681-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6681-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6681-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6681-107">Aktualisieren Sie die Eigenschaften eines [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6681-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6681-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6681-108">Prerequisites</span></span>
<span data-ttu-id="a6681-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6681-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6681-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6681-111">Permission type</span></span>|<span data-ttu-id="a6681-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6681-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6681-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6681-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6681-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6681-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6681-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6681-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6681-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6681-116">Not supported.</span></span>|
|<span data-ttu-id="a6681-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6681-117">Application</span></span>|<span data-ttu-id="a6681-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6681-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6681-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6681-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6681-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6681-120">Request headers</span></span>
|<span data-ttu-id="a6681-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a6681-121">Header</span></span>|<span data-ttu-id="a6681-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a6681-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6681-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6681-123">Authorization</span></span>|<span data-ttu-id="a6681-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6681-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6681-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6681-125">Accept</span></span>|<span data-ttu-id="a6681-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6681-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6681-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6681-127">Request body</span></span>
<span data-ttu-id="a6681-128">Geben Sie im Textkörper Anforderung für das Objekt [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a6681-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="a6681-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="a6681-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="a6681-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6681-130">Property</span></span>|<span data-ttu-id="a6681-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a6681-131">Type</span></span>|<span data-ttu-id="a6681-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6681-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6681-133">id</span><span class="sxs-lookup"><span data-stu-id="a6681-133">id</span></span>|<span data-ttu-id="a6681-134">String</span><span class="sxs-lookup"><span data-stu-id="a6681-134">String</span></span>|<span data-ttu-id="a6681-135">Eindeutiger Bezeichner für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="a6681-135">Unique identifier for the object.</span></span> <span data-ttu-id="a6681-136">Besteht aus den AccountId, Geräte-ID, PolicyId und Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="a6681-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="a6681-137">userId</span><span class="sxs-lookup"><span data-stu-id="a6681-137">userId</span></span>|<span data-ttu-id="a6681-138">String</span><span class="sxs-lookup"><span data-stu-id="a6681-138">String</span></span>|<span data-ttu-id="a6681-139">Eindeutige Benutzer-ID muss Guid</span><span class="sxs-lookup"><span data-stu-id="a6681-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a6681-140">userName</span><span class="sxs-lookup"><span data-stu-id="a6681-140">userName</span></span>|<span data-ttu-id="a6681-141">String</span><span class="sxs-lookup"><span data-stu-id="a6681-141">String</span></span>|<span data-ttu-id="a6681-142">Benutzername</span><span class="sxs-lookup"><span data-stu-id="a6681-142">User name</span></span>|
|<span data-ttu-id="a6681-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a6681-143">managedDeviceId</span></span>|<span data-ttu-id="a6681-144">String</span><span class="sxs-lookup"><span data-stu-id="a6681-144">String</span></span>|<span data-ttu-id="a6681-145">Eindeutiger Bezeichner der verwalteten Gerät, muss die Guid</span><span class="sxs-lookup"><span data-stu-id="a6681-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a6681-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="a6681-146">deviceName</span></span>|<span data-ttu-id="a6681-147">String</span><span class="sxs-lookup"><span data-stu-id="a6681-147">String</span></span>|<span data-ttu-id="a6681-148">Gerätename</span><span class="sxs-lookup"><span data-stu-id="a6681-148">Device name</span></span>|
|<span data-ttu-id="a6681-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a6681-149">deviceConfigurationId</span></span>|<span data-ttu-id="a6681-150">String</span><span class="sxs-lookup"><span data-stu-id="a6681-150">String</span></span>|<span data-ttu-id="a6681-151">Gerät Konfiguration Profil Eindeutiger Bezeichner muss Guid</span><span class="sxs-lookup"><span data-stu-id="a6681-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a6681-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="a6681-152">deviceConfigurationName</span></span>|<span data-ttu-id="a6681-153">String</span><span class="sxs-lookup"><span data-stu-id="a6681-153">String</span></span>|<span data-ttu-id="a6681-154">Gerätename Konfiguration-Profil</span><span class="sxs-lookup"><span data-stu-id="a6681-154">Device configuration profile name</span></span>|
|<span data-ttu-id="a6681-155">platformType</span><span class="sxs-lookup"><span data-stu-id="a6681-155">platformType</span></span>|[<span data-ttu-id="a6681-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a6681-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a6681-157">Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="a6681-157">Platform type.</span></span> <span data-ttu-id="a6681-158">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a6681-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a6681-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="a6681-159">restrictedAppsState</span></span>|[<span data-ttu-id="a6681-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="a6681-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="a6681-161">Eingeschränkte apps Zustand.</span><span class="sxs-lookup"><span data-stu-id="a6681-161">Restricted apps state.</span></span> <span data-ttu-id="a6681-162">Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="a6681-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="a6681-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="a6681-163">restrictedApps</span></span>|<span data-ttu-id="a6681-164">[ManagedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a6681-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="a6681-165">Liste der verletzte eingeschränkte apps</span><span class="sxs-lookup"><span data-stu-id="a6681-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="a6681-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6681-166">Response</span></span>
<span data-ttu-id="a6681-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a6681-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6681-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6681-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6681-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6681-169">Request</span></span>
<span data-ttu-id="a6681-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6681-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 502

{
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

### <a name="response"></a><span data-ttu-id="a6681-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6681-171">Response</span></span>
<span data-ttu-id="a6681-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6681-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






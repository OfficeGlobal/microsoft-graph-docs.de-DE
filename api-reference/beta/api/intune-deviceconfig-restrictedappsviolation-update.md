---
title: RestrictedAppsViolation aktualisieren
description: Aktualisieren der Eigenschaften eines restrictedAppsViolation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc2a440872d399cc684c2ce52ce2d825ba52f9ce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163350"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="87f8c-103">RestrictedAppsViolation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="87f8c-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="87f8c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87f8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87f8c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="87f8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87f8c-106">Aktualisieren der Eigenschaften eines [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="87f8c-106">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87f8c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87f8c-107">Prerequisites</span></span>
<span data-ttu-id="87f8c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87f8c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87f8c-110">Permission type</span></span>|<span data-ttu-id="87f8c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87f8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f8c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87f8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87f8c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f8c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87f8c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87f8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f8c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87f8c-115">Not supported.</span></span>|
|<span data-ttu-id="87f8c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87f8c-116">Application</span></span>|<span data-ttu-id="87f8c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87f8c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f8c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87f8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="87f8c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87f8c-119">Request headers</span></span>
|<span data-ttu-id="87f8c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87f8c-120">Header</span></span>|<span data-ttu-id="87f8c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="87f8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87f8c-122">Authorization</span></span>|<span data-ttu-id="87f8c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87f8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f8c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="87f8c-124">Accept</span></span>|<span data-ttu-id="87f8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87f8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f8c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87f8c-126">Request body</span></span>
<span data-ttu-id="87f8c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="87f8c-127">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="87f8c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="87f8c-128">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="87f8c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87f8c-129">Property</span></span>|<span data-ttu-id="87f8c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="87f8c-130">Type</span></span>|<span data-ttu-id="87f8c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87f8c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87f8c-132">id</span><span class="sxs-lookup"><span data-stu-id="87f8c-132">id</span></span>|<span data-ttu-id="87f8c-133">string</span><span class="sxs-lookup"><span data-stu-id="87f8c-133">String</span></span>|<span data-ttu-id="87f8c-134">Eindeutiger Bezeichner für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="87f8c-134">Unique identifier for the object.</span></span> <span data-ttu-id="87f8c-135">Zusammengesetzt aus "Account-ID", "Device", "Policies" und "userId"</span><span class="sxs-lookup"><span data-stu-id="87f8c-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="87f8c-136">userId</span><span class="sxs-lookup"><span data-stu-id="87f8c-136">userId</span></span>|<span data-ttu-id="87f8c-137">String</span><span class="sxs-lookup"><span data-stu-id="87f8c-137">String</span></span>|<span data-ttu-id="87f8c-138">Benutzer eindeutiger Bezeichner, muss GUID sein</span><span class="sxs-lookup"><span data-stu-id="87f8c-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="87f8c-139">userName</span><span class="sxs-lookup"><span data-stu-id="87f8c-139">userName</span></span>|<span data-ttu-id="87f8c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87f8c-140">String</span></span>|<span data-ttu-id="87f8c-141">Benutzername</span><span class="sxs-lookup"><span data-stu-id="87f8c-141">User name</span></span>|
|<span data-ttu-id="87f8c-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="87f8c-142">managedDeviceId</span></span>|<span data-ttu-id="87f8c-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87f8c-143">String</span></span>|<span data-ttu-id="87f8c-144">Eindeutiger Bezeichner für verwaltetes Gerät, muss GUID sein</span><span class="sxs-lookup"><span data-stu-id="87f8c-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="87f8c-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="87f8c-145">deviceName</span></span>|<span data-ttu-id="87f8c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87f8c-146">String</span></span>|<span data-ttu-id="87f8c-147">Gerätename</span><span class="sxs-lookup"><span data-stu-id="87f8c-147">Device name</span></span>|
|<span data-ttu-id="87f8c-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="87f8c-148">deviceConfigurationId</span></span>|<span data-ttu-id="87f8c-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87f8c-149">String</span></span>|<span data-ttu-id="87f8c-150">Device Configuration Profile Unique Identifier, must be GUID</span><span class="sxs-lookup"><span data-stu-id="87f8c-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="87f8c-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="87f8c-151">deviceConfigurationName</span></span>|<span data-ttu-id="87f8c-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87f8c-152">String</span></span>|<span data-ttu-id="87f8c-153">Name des Geräte Konfigurationsprofils</span><span class="sxs-lookup"><span data-stu-id="87f8c-153">Device configuration profile name</span></span>|
|<span data-ttu-id="87f8c-154">platformType</span><span class="sxs-lookup"><span data-stu-id="87f8c-154">platformType</span></span>|[<span data-ttu-id="87f8c-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="87f8c-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="87f8c-156">Plattformtyp.</span><span class="sxs-lookup"><span data-stu-id="87f8c-156">Platform type.</span></span> <span data-ttu-id="87f8c-157">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="87f8c-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="87f8c-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="87f8c-158">restrictedAppsState</span></span>|[<span data-ttu-id="87f8c-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="87f8c-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="87f8c-160">Eingeschränkter apps-Status.</span><span class="sxs-lookup"><span data-stu-id="87f8c-160">Restricted apps state.</span></span> <span data-ttu-id="87f8c-161">Mögliche Werte sind: `prohibitedApps` und `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="87f8c-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="87f8c-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="87f8c-162">restrictedApps</span></span>|<span data-ttu-id="87f8c-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="87f8c-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="87f8c-164">Liste der verletzten eingeschränkten apps</span><span class="sxs-lookup"><span data-stu-id="87f8c-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="87f8c-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="87f8c-165">Response</span></span>
<span data-ttu-id="87f8c-166">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="87f8c-166">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f8c-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87f8c-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="87f8c-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87f8c-168">Request</span></span>
<span data-ttu-id="87f8c-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87f8c-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
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

### <a name="response"></a><span data-ttu-id="87f8c-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="87f8c-170">Response</span></span>
<span data-ttu-id="87f8c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87f8c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





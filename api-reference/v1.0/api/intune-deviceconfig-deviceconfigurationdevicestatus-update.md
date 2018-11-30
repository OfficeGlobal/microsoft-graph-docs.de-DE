---
title: Aktualisieren von „deviceConfigurationDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStatus.
ms.openlocfilehash: 1ea327f61ef1afcebebbe92d80e61f5fc2d0f00e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016684"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="47408-103">Aktualisieren von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="47408-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="47408-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47408-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47408-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="47408-105">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47408-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47408-106">Prerequisites</span></span>
<span data-ttu-id="47408-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47408-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47408-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47408-109">Permission type</span></span>|<span data-ttu-id="47408-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47408-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47408-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47408-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47408-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47408-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47408-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47408-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47408-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47408-114">Not supported.</span></span>|
|<span data-ttu-id="47408-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47408-115">Application</span></span>|<span data-ttu-id="47408-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47408-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47408-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47408-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="47408-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47408-118">Request headers</span></span>
|<span data-ttu-id="47408-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47408-119">Header</span></span>|<span data-ttu-id="47408-120">Wert</span><span class="sxs-lookup"><span data-stu-id="47408-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47408-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47408-121">Authorization</span></span>|<span data-ttu-id="47408-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47408-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47408-123">Accept</span><span class="sxs-lookup"><span data-stu-id="47408-123">Accept</span></span>|<span data-ttu-id="47408-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47408-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47408-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47408-125">Request body</span></span>
<span data-ttu-id="47408-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="47408-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="47408-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="47408-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="47408-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47408-128">Property</span></span>|<span data-ttu-id="47408-129">Typ</span><span class="sxs-lookup"><span data-stu-id="47408-129">Type</span></span>|<span data-ttu-id="47408-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47408-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47408-131">id</span><span class="sxs-lookup"><span data-stu-id="47408-131">id</span></span>|<span data-ttu-id="47408-132">String</span><span class="sxs-lookup"><span data-stu-id="47408-132">String</span></span>|<span data-ttu-id="47408-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="47408-133">Key of the entity.</span></span>|
|<span data-ttu-id="47408-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="47408-134">deviceDisplayName</span></span>|<span data-ttu-id="47408-135">String</span><span class="sxs-lookup"><span data-stu-id="47408-135">String</span></span>|<span data-ttu-id="47408-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="47408-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="47408-137">userName</span><span class="sxs-lookup"><span data-stu-id="47408-137">userName</span></span>|<span data-ttu-id="47408-138">String</span><span class="sxs-lookup"><span data-stu-id="47408-138">String</span></span>|<span data-ttu-id="47408-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="47408-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="47408-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="47408-140">deviceModel</span></span>|<span data-ttu-id="47408-141">String</span><span class="sxs-lookup"><span data-stu-id="47408-141">String</span></span>|<span data-ttu-id="47408-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="47408-142">The device model that is being reported</span></span>|
|<span data-ttu-id="47408-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="47408-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="47408-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47408-144">DateTimeOffset</span></span>|<span data-ttu-id="47408-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="47408-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="47408-146">status</span><span class="sxs-lookup"><span data-stu-id="47408-146">status</span></span>|[<span data-ttu-id="47408-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="47408-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="47408-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="47408-148">Compliance status of the policy report.</span></span> <span data-ttu-id="47408-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="47408-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="47408-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="47408-150">lastReportedDateTime</span></span>|<span data-ttu-id="47408-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47408-151">DateTimeOffset</span></span>|<span data-ttu-id="47408-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="47408-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="47408-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="47408-153">userPrincipalName</span></span>|<span data-ttu-id="47408-154">String</span><span class="sxs-lookup"><span data-stu-id="47408-154">String</span></span>|<span data-ttu-id="47408-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="47408-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="47408-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="47408-156">Response</span></span>
<span data-ttu-id="47408-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47408-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47408-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47408-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="47408-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47408-159">Request</span></span>
<span data-ttu-id="47408-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47408-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="47408-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="47408-161">Response</span></span>
<span data-ttu-id="47408-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47408-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




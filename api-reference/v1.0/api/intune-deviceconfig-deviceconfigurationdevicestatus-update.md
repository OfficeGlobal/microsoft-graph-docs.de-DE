---
title: Aktualisieren von „deviceConfigurationDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fe30e76b9b9c392bdad9532559b1489d470bc98
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258128"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="093e0-103">Aktualisieren von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="093e0-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="093e0-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="093e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="093e0-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="093e0-105">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="093e0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="093e0-106">Prerequisites</span></span>
<span data-ttu-id="093e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="093e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="093e0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="093e0-109">Permission type</span></span>|<span data-ttu-id="093e0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="093e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="093e0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="093e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="093e0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093e0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="093e0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="093e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="093e0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="093e0-114">Not supported.</span></span>|
|<span data-ttu-id="093e0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="093e0-115">Application</span></span>|<span data-ttu-id="093e0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="093e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="093e0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="093e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="093e0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="093e0-118">Request headers</span></span>
|<span data-ttu-id="093e0-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="093e0-119">Header</span></span>|<span data-ttu-id="093e0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="093e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="093e0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="093e0-121">Authorization</span></span>|<span data-ttu-id="093e0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="093e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="093e0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="093e0-123">Accept</span></span>|<span data-ttu-id="093e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="093e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="093e0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="093e0-125">Request body</span></span>
<span data-ttu-id="093e0-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="093e0-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="093e0-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="093e0-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="093e0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="093e0-128">Property</span></span>|<span data-ttu-id="093e0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="093e0-129">Type</span></span>|<span data-ttu-id="093e0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="093e0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="093e0-131">id</span><span class="sxs-lookup"><span data-stu-id="093e0-131">id</span></span>|<span data-ttu-id="093e0-132">String</span><span class="sxs-lookup"><span data-stu-id="093e0-132">String</span></span>|<span data-ttu-id="093e0-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="093e0-133">Key of the entity.</span></span>|
|<span data-ttu-id="093e0-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="093e0-134">deviceDisplayName</span></span>|<span data-ttu-id="093e0-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="093e0-135">String</span></span>|<span data-ttu-id="093e0-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="093e0-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="093e0-137">userName</span><span class="sxs-lookup"><span data-stu-id="093e0-137">userName</span></span>|<span data-ttu-id="093e0-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="093e0-138">String</span></span>|<span data-ttu-id="093e0-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="093e0-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="093e0-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="093e0-140">deviceModel</span></span>|<span data-ttu-id="093e0-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="093e0-141">String</span></span>|<span data-ttu-id="093e0-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="093e0-142">The device model that is being reported</span></span>|
|<span data-ttu-id="093e0-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="093e0-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="093e0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="093e0-144">DateTimeOffset</span></span>|<span data-ttu-id="093e0-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="093e0-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="093e0-146">status</span><span class="sxs-lookup"><span data-stu-id="093e0-146">status</span></span>|[<span data-ttu-id="093e0-147">Wurde</span><span class="sxs-lookup"><span data-stu-id="093e0-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="093e0-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="093e0-148">Compliance status of the policy report.</span></span> <span data-ttu-id="093e0-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="093e0-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="093e0-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="093e0-150">lastReportedDateTime</span></span>|<span data-ttu-id="093e0-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="093e0-151">DateTimeOffset</span></span>|<span data-ttu-id="093e0-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="093e0-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="093e0-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="093e0-153">userPrincipalName</span></span>|<span data-ttu-id="093e0-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="093e0-154">String</span></span>|<span data-ttu-id="093e0-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="093e0-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="093e0-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="093e0-156">Response</span></span>
<span data-ttu-id="093e0-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="093e0-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="093e0-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="093e0-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="093e0-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="093e0-159">Request</span></span>
<span data-ttu-id="093e0-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="093e0-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="093e0-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="093e0-161">Response</span></span>
<span data-ttu-id="093e0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="093e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Aktualisieren von „deviceComplianceDeviceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 5f894c325e6f7732cb41b7472e85e3dbb8361e3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343680"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="d877b-103">Aktualisieren von „deviceComplianceDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="d877b-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="d877b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d877b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d877b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d877b-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d877b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d877b-106">Prerequisites</span></span>
<span data-ttu-id="d877b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d877b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d877b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d877b-109">Permission type</span></span>|<span data-ttu-id="d877b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d877b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d877b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d877b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d877b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d877b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d877b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d877b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d877b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d877b-114">Not supported.</span></span>|
|<span data-ttu-id="d877b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d877b-115">Application</span></span>|<span data-ttu-id="d877b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d877b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d877b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d877b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d877b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d877b-118">Request headers</span></span>
|<span data-ttu-id="d877b-119">Header</span><span class="sxs-lookup"><span data-stu-id="d877b-119">Header</span></span>|<span data-ttu-id="d877b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d877b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d877b-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d877b-121">Authorization</span></span>|<span data-ttu-id="d877b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d877b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d877b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d877b-123">Accept</span></span>|<span data-ttu-id="d877b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d877b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d877b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d877b-125">Request body</span></span>
<span data-ttu-id="d877b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="d877b-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="d877b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d877b-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="d877b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d877b-128">Property</span></span>|<span data-ttu-id="d877b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d877b-129">Type</span></span>|<span data-ttu-id="d877b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d877b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d877b-131">id</span><span class="sxs-lookup"><span data-stu-id="d877b-131">id</span></span>|<span data-ttu-id="d877b-132">String</span><span class="sxs-lookup"><span data-stu-id="d877b-132">String</span></span>|<span data-ttu-id="d877b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d877b-133">Key of the entity.</span></span>|
|<span data-ttu-id="d877b-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d877b-134">deviceDisplayName</span></span>|<span data-ttu-id="d877b-135">String</span><span class="sxs-lookup"><span data-stu-id="d877b-135">String</span></span>|<span data-ttu-id="d877b-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="d877b-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d877b-137">userName</span><span class="sxs-lookup"><span data-stu-id="d877b-137">userName</span></span>|<span data-ttu-id="d877b-138">String</span><span class="sxs-lookup"><span data-stu-id="d877b-138">String</span></span>|<span data-ttu-id="d877b-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="d877b-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="d877b-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d877b-140">deviceModel</span></span>|<span data-ttu-id="d877b-141">String</span><span class="sxs-lookup"><span data-stu-id="d877b-141">String</span></span>|<span data-ttu-id="d877b-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="d877b-142">The device model that is being reported</span></span>|
|<span data-ttu-id="d877b-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d877b-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d877b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d877b-144">DateTimeOffset</span></span>|<span data-ttu-id="d877b-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="d877b-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d877b-146">status</span><span class="sxs-lookup"><span data-stu-id="d877b-146">status</span></span>|[<span data-ttu-id="d877b-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d877b-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d877b-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="d877b-148">Compliance status of the policy report.</span></span> <span data-ttu-id="d877b-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d877b-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d877b-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d877b-150">lastReportedDateTime</span></span>|<span data-ttu-id="d877b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d877b-151">DateTimeOffset</span></span>|<span data-ttu-id="d877b-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="d877b-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d877b-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d877b-153">userPrincipalName</span></span>|<span data-ttu-id="d877b-154">String</span><span class="sxs-lookup"><span data-stu-id="d877b-154">String</span></span>|<span data-ttu-id="d877b-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="d877b-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d877b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="d877b-156">Response</span></span>
<span data-ttu-id="d877b-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d877b-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d877b-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d877b-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="d877b-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d877b-159">Request</span></span>
<span data-ttu-id="d877b-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d877b-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="d877b-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="d877b-161">Response</span></span>
<span data-ttu-id="d877b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d877b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




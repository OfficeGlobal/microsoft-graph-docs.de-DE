---
title: ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren
description: Aktualisieren der Eigenschaften eines managedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48afdece32d82d0112ebc77cf13fa71ff1b175d1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961945"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="1b457-103">ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1b457-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="1b457-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b457-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1b457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b457-106">Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b457-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b457-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b457-107">Prerequisites</span></span>
<span data-ttu-id="1b457-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b457-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b457-110">Permission type</span></span>|<span data-ttu-id="1b457-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b457-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b457-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b457-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b457-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b457-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b457-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b457-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b457-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b457-115">Not supported.</span></span>|
|<span data-ttu-id="1b457-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b457-116">Application</span></span>|<span data-ttu-id="1b457-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b457-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b457-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b457-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1b457-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b457-119">Request headers</span></span>
|<span data-ttu-id="1b457-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b457-120">Header</span></span>|<span data-ttu-id="1b457-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1b457-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b457-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b457-122">Authorization</span></span>|<span data-ttu-id="1b457-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b457-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b457-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1b457-124">Accept</span></span>|<span data-ttu-id="1b457-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b457-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b457-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b457-126">Request body</span></span>
<span data-ttu-id="1b457-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1b457-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="1b457-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1b457-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="1b457-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b457-129">Property</span></span>|<span data-ttu-id="1b457-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1b457-130">Type</span></span>|<span data-ttu-id="1b457-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b457-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b457-132">id</span><span class="sxs-lookup"><span data-stu-id="1b457-132">id</span></span>|<span data-ttu-id="1b457-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b457-133">String</span></span>|<span data-ttu-id="1b457-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1b457-134">Key of the entity.</span></span>|
|<span data-ttu-id="1b457-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1b457-135">deviceDisplayName</span></span>|<span data-ttu-id="1b457-136">String</span><span class="sxs-lookup"><span data-stu-id="1b457-136">String</span></span>|<span data-ttu-id="1b457-137">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="1b457-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1b457-138">userName</span><span class="sxs-lookup"><span data-stu-id="1b457-138">userName</span></span>|<span data-ttu-id="1b457-139">String</span><span class="sxs-lookup"><span data-stu-id="1b457-139">String</span></span>|<span data-ttu-id="1b457-140">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="1b457-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="1b457-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1b457-141">deviceModel</span></span>|<span data-ttu-id="1b457-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b457-142">String</span></span>|<span data-ttu-id="1b457-143">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="1b457-143">The device model that is being reported</span></span>|
|<span data-ttu-id="1b457-144">Plattform</span><span class="sxs-lookup"><span data-stu-id="1b457-144">platform</span></span>|<span data-ttu-id="1b457-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1b457-145">Int32</span></span>|<span data-ttu-id="1b457-146">Plattform des gemeldeten Geräts</span><span class="sxs-lookup"><span data-stu-id="1b457-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="1b457-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1b457-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1b457-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b457-148">DateTimeOffset</span></span>|<span data-ttu-id="1b457-149">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="1b457-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1b457-150">status</span><span class="sxs-lookup"><span data-stu-id="1b457-150">status</span></span>|[<span data-ttu-id="1b457-151">Wurde</span><span class="sxs-lookup"><span data-stu-id="1b457-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1b457-152">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="1b457-152">Compliance status of the policy report.</span></span> <span data-ttu-id="1b457-153">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1b457-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1b457-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b457-154">lastReportedDateTime</span></span>|<span data-ttu-id="1b457-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b457-155">DateTimeOffset</span></span>|<span data-ttu-id="1b457-156">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="1b457-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1b457-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b457-157">userPrincipalName</span></span>|<span data-ttu-id="1b457-158">String</span><span class="sxs-lookup"><span data-stu-id="1b457-158">String</span></span>|<span data-ttu-id="1b457-159">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="1b457-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1b457-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b457-160">Response</span></span>
<span data-ttu-id="1b457-161">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1b457-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b457-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b457-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b457-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b457-163">Request</span></span>
<span data-ttu-id="1b457-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b457-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="1b457-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b457-165">Response</span></span>
<span data-ttu-id="1b457-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b457-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





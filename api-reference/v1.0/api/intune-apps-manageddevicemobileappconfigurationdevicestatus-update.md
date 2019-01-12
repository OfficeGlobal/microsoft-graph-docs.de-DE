---
title: ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a5cc2b46bc02644dc6467e3e629c3d631a13a59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913823"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="46486-103">ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="46486-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="46486-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46486-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46486-105">Aktualisieren Sie die Eigenschaften eines [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="46486-105">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46486-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46486-106">Prerequisites</span></span>
<span data-ttu-id="46486-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46486-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46486-109">Permission type</span></span>|<span data-ttu-id="46486-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46486-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46486-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46486-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46486-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46486-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46486-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46486-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46486-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46486-114">Not supported.</span></span>|
|<span data-ttu-id="46486-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46486-115">Application</span></span>|<span data-ttu-id="46486-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46486-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46486-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46486-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="46486-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46486-118">Request headers</span></span>
|<span data-ttu-id="46486-119">Header</span><span class="sxs-lookup"><span data-stu-id="46486-119">Header</span></span>|<span data-ttu-id="46486-120">Wert</span><span class="sxs-lookup"><span data-stu-id="46486-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46486-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46486-121">Authorization</span></span>|<span data-ttu-id="46486-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46486-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46486-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46486-123">Accept</span></span>|<span data-ttu-id="46486-124">application/json</span><span class="sxs-lookup"><span data-stu-id="46486-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46486-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46486-125">Request body</span></span>
<span data-ttu-id="46486-126">Geben Sie im Textkörper Anforderung für das Objekt [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="46486-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="46486-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="46486-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="46486-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46486-128">Property</span></span>|<span data-ttu-id="46486-129">Typ</span><span class="sxs-lookup"><span data-stu-id="46486-129">Type</span></span>|<span data-ttu-id="46486-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46486-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46486-131">id</span><span class="sxs-lookup"><span data-stu-id="46486-131">id</span></span>|<span data-ttu-id="46486-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46486-132">String</span></span>|<span data-ttu-id="46486-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="46486-133">Key of the entity.</span></span>|
|<span data-ttu-id="46486-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="46486-134">deviceDisplayName</span></span>|<span data-ttu-id="46486-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46486-135">String</span></span>|<span data-ttu-id="46486-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="46486-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46486-137">userName</span><span class="sxs-lookup"><span data-stu-id="46486-137">userName</span></span>|<span data-ttu-id="46486-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46486-138">String</span></span>|<span data-ttu-id="46486-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="46486-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="46486-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="46486-140">deviceModel</span></span>|<span data-ttu-id="46486-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46486-141">String</span></span>|<span data-ttu-id="46486-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="46486-142">The device model that is being reported</span></span>|
|<span data-ttu-id="46486-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="46486-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="46486-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46486-144">DateTimeOffset</span></span>|<span data-ttu-id="46486-145">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="46486-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="46486-146">status</span><span class="sxs-lookup"><span data-stu-id="46486-146">status</span></span>|[<span data-ttu-id="46486-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="46486-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46486-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="46486-148">Compliance status of the policy report.</span></span> <span data-ttu-id="46486-149">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="46486-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46486-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46486-150">lastReportedDateTime</span></span>|<span data-ttu-id="46486-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46486-151">DateTimeOffset</span></span>|<span data-ttu-id="46486-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="46486-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46486-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46486-153">userPrincipalName</span></span>|<span data-ttu-id="46486-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="46486-154">String</span></span>|<span data-ttu-id="46486-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="46486-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46486-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="46486-156">Response</span></span>
<span data-ttu-id="46486-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="46486-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46486-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46486-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="46486-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46486-159">Request</span></span>
<span data-ttu-id="46486-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46486-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="46486-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="46486-161">Response</span></span>
<span data-ttu-id="46486-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46486-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




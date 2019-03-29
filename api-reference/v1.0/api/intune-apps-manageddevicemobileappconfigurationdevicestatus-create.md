---
title: ManagedDeviceMobileAppConfigurationDeviceStatus erstellen
description: Erstellen eines neuen managedDeviceMobileAppConfigurationDeviceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c70d74e1ac98710b8b56c3ca3a262e34c2e39fd2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962246"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="7d7fd-103">ManagedDeviceMobileAppConfigurationDeviceStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="7d7fd-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="7d7fd-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d7fd-105">Erstellen eines neuen [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-105">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d7fd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d7fd-106">Prerequisites</span></span>
<span data-ttu-id="7d7fd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7fd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d7fd-109">Permission type</span></span>|<span data-ttu-id="7d7fd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d7fd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7fd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d7fd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7fd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7fd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7fd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d7fd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7fd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d7fd-114">Not supported.</span></span>|
|<span data-ttu-id="7d7fd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d7fd-115">Application</span></span>|<span data-ttu-id="7d7fd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d7fd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7fd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d7fd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7d7fd-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d7fd-118">Request headers</span></span>
|<span data-ttu-id="7d7fd-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7d7fd-119">Header</span></span>|<span data-ttu-id="7d7fd-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7d7fd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d7fd-121">Authorization</span></span>|<span data-ttu-id="7d7fd-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d7fd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7fd-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7d7fd-123">Accept</span></span>|<span data-ttu-id="7d7fd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7fd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7fd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d7fd-125">Request body</span></span>
<span data-ttu-id="7d7fd-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das managedDeviceMobileAppConfigurationDeviceStatus-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="7d7fd-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedDeviceMobileAppConfigurationDeviceStatus erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="7d7fd-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d7fd-128">Property</span></span>|<span data-ttu-id="7d7fd-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7d7fd-129">Type</span></span>|<span data-ttu-id="7d7fd-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d7fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7fd-131">id</span><span class="sxs-lookup"><span data-stu-id="7d7fd-131">id</span></span>|<span data-ttu-id="7d7fd-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d7fd-132">String</span></span>|<span data-ttu-id="7d7fd-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7d7fd-133">Key of the entity.</span></span>|
|<span data-ttu-id="7d7fd-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7d7fd-134">deviceDisplayName</span></span>|<span data-ttu-id="7d7fd-135">String</span><span class="sxs-lookup"><span data-stu-id="7d7fd-135">String</span></span>|<span data-ttu-id="7d7fd-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="7d7fd-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="7d7fd-137">userName</span><span class="sxs-lookup"><span data-stu-id="7d7fd-137">userName</span></span>|<span data-ttu-id="7d7fd-138">String</span><span class="sxs-lookup"><span data-stu-id="7d7fd-138">String</span></span>|<span data-ttu-id="7d7fd-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="7d7fd-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="7d7fd-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7d7fd-140">deviceModel</span></span>|<span data-ttu-id="7d7fd-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d7fd-141">String</span></span>|<span data-ttu-id="7d7fd-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="7d7fd-142">The device model that is being reported</span></span>|
|<span data-ttu-id="7d7fd-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7fd-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7d7fd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7fd-144">DateTimeOffset</span></span>|<span data-ttu-id="7d7fd-145">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="7d7fd-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="7d7fd-146">status</span><span class="sxs-lookup"><span data-stu-id="7d7fd-146">status</span></span>|[<span data-ttu-id="7d7fd-147">Wurde</span><span class="sxs-lookup"><span data-stu-id="7d7fd-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7d7fd-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-148">Compliance status of the policy report.</span></span> <span data-ttu-id="7d7fd-149">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7d7fd-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7fd-150">lastReportedDateTime</span></span>|<span data-ttu-id="7d7fd-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7fd-151">DateTimeOffset</span></span>|<span data-ttu-id="7d7fd-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="7d7fd-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="7d7fd-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7d7fd-153">userPrincipalName</span></span>|<span data-ttu-id="7d7fd-154">String</span><span class="sxs-lookup"><span data-stu-id="7d7fd-154">String</span></span>|<span data-ttu-id="7d7fd-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7d7fd-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="7d7fd-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d7fd-156">Response</span></span>
<span data-ttu-id="7d7fd-157">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-157">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7fd-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d7fd-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d7fd-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d7fd-159">Request</span></span>
<span data-ttu-id="7d7fd-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="7d7fd-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d7fd-161">Response</span></span>
<span data-ttu-id="7d7fd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d7fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




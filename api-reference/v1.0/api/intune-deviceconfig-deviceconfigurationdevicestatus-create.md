---
title: Erstellen von „deviceConfigurationDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 847363fa484de3ea1c210d5e6bd0918721db45b1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984268"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="e7c1b-103">Erstellen von „deviceConfigurationDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="e7c1b-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="e7c1b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c1b-105">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e7c1b-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c1b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7c1b-106">Prerequisites</span></span>
<span data-ttu-id="e7c1b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c1b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7c1b-109">Permission type</span></span>|<span data-ttu-id="e7c1b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7c1b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c1b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7c1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c1b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c1b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c1b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7c1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c1b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c1b-114">Not supported.</span></span>|
|<span data-ttu-id="e7c1b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7c1b-115">Application</span></span>|<span data-ttu-id="e7c1b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7c1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c1b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c1b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e7c1b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7c1b-118">Request headers</span></span>
|<span data-ttu-id="e7c1b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e7c1b-119">Header</span></span>|<span data-ttu-id="e7c1b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e7c1b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c1b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c1b-121">Authorization</span></span>|<span data-ttu-id="e7c1b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7c1b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c1b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7c1b-123">Accept</span></span>|<span data-ttu-id="e7c1b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c1b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c1b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7c1b-125">Request body</span></span>
<span data-ttu-id="e7c1b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationDeviceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="e7c1b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationDeviceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="e7c1b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7c1b-128">Property</span></span>|<span data-ttu-id="e7c1b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e7c1b-129">Type</span></span>|<span data-ttu-id="e7c1b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7c1b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c1b-131">id</span><span class="sxs-lookup"><span data-stu-id="e7c1b-131">id</span></span>|<span data-ttu-id="e7c1b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7c1b-132">String</span></span>|<span data-ttu-id="e7c1b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e7c1b-133">Key of the entity.</span></span>|
|<span data-ttu-id="e7c1b-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7c1b-134">deviceDisplayName</span></span>|<span data-ttu-id="e7c1b-135">String</span><span class="sxs-lookup"><span data-stu-id="e7c1b-135">String</span></span>|<span data-ttu-id="e7c1b-136">Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="e7c1b-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e7c1b-137">userName</span><span class="sxs-lookup"><span data-stu-id="e7c1b-137">userName</span></span>|<span data-ttu-id="e7c1b-138">String</span><span class="sxs-lookup"><span data-stu-id="e7c1b-138">String</span></span>|<span data-ttu-id="e7c1b-139">Gemeldeter Benutzername</span><span class="sxs-lookup"><span data-stu-id="e7c1b-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="e7c1b-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e7c1b-140">deviceModel</span></span>|<span data-ttu-id="e7c1b-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7c1b-141">String</span></span>|<span data-ttu-id="e7c1b-142">Gemeldetes Gerätemodell</span><span class="sxs-lookup"><span data-stu-id="e7c1b-142">The device model that is being reported</span></span>|
|<span data-ttu-id="e7c1b-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e7c1b-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e7c1b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7c1b-144">DateTimeOffset</span></span>|<span data-ttu-id="e7c1b-145">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="e7c1b-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="e7c1b-146">status</span><span class="sxs-lookup"><span data-stu-id="e7c1b-146">status</span></span>|[<span data-ttu-id="e7c1b-147">Wurde</span><span class="sxs-lookup"><span data-stu-id="e7c1b-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e7c1b-148">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-148">Compliance status of the policy report.</span></span> <span data-ttu-id="e7c1b-149">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e7c1b-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7c1b-150">lastReportedDateTime</span></span>|<span data-ttu-id="e7c1b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7c1b-151">DateTimeOffset</span></span>|<span data-ttu-id="e7c1b-152">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="e7c1b-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e7c1b-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7c1b-153">userPrincipalName</span></span>|<span data-ttu-id="e7c1b-154">String</span><span class="sxs-lookup"><span data-stu-id="e7c1b-154">String</span></span>|<span data-ttu-id="e7c1b-155">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="e7c1b-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="e7c1b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c1b-156">Response</span></span>
<span data-ttu-id="e7c1b-157">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c1b-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7c1b-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c1b-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7c1b-159">Request</span></span>
<span data-ttu-id="e7c1b-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="e7c1b-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7c1b-161">Response</span></span>
<span data-ttu-id="e7c1b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7c1b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




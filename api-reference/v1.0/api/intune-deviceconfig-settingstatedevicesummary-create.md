---
title: settingStateDeviceSummary erstellen
description: Erstellen eines neuen SettingStateDeviceSummary-Objekts.
author: tfitzmac
ms.openlocfilehash: 53cccf3ee6cf11daa6cec1697de89eaf7f0a7140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309576"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="93b08-103">settingStateDeviceSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="93b08-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="93b08-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93b08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93b08-105">Erstellen eines neuen [SettingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="93b08-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93b08-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93b08-106">Prerequisites</span></span>
<span data-ttu-id="93b08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93b08-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93b08-109">Permission type</span></span>|<span data-ttu-id="93b08-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93b08-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93b08-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93b08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93b08-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93b08-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93b08-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93b08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93b08-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93b08-114">Not supported.</span></span>|
|<span data-ttu-id="93b08-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93b08-115">Application</span></span>|<span data-ttu-id="93b08-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93b08-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93b08-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93b08-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="93b08-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93b08-118">Request headers</span></span>
|<span data-ttu-id="93b08-119">Header</span><span class="sxs-lookup"><span data-stu-id="93b08-119">Header</span></span>|<span data-ttu-id="93b08-120">Wert</span><span class="sxs-lookup"><span data-stu-id="93b08-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93b08-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="93b08-121">Authorization</span></span>|<span data-ttu-id="93b08-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93b08-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93b08-123">Accept</span><span class="sxs-lookup"><span data-stu-id="93b08-123">Accept</span></span>|<span data-ttu-id="93b08-124">application/json</span><span class="sxs-lookup"><span data-stu-id="93b08-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93b08-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93b08-125">Request body</span></span>
<span data-ttu-id="93b08-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs settingStateDeviceSummary an.</span><span class="sxs-lookup"><span data-stu-id="93b08-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="93b08-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs settingStateDeviceSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="93b08-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="93b08-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93b08-128">Property</span></span>|<span data-ttu-id="93b08-129">Typ</span><span class="sxs-lookup"><span data-stu-id="93b08-129">Type</span></span>|<span data-ttu-id="93b08-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93b08-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93b08-131">id</span><span class="sxs-lookup"><span data-stu-id="93b08-131">id</span></span>|<span data-ttu-id="93b08-132">String</span><span class="sxs-lookup"><span data-stu-id="93b08-132">String</span></span>|<span data-ttu-id="93b08-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="93b08-133">Key of the entity.</span></span>|
|<span data-ttu-id="93b08-134">settingName</span><span class="sxs-lookup"><span data-stu-id="93b08-134">settingName</span></span>|<span data-ttu-id="93b08-135">String</span><span class="sxs-lookup"><span data-stu-id="93b08-135">String</span></span>|<span data-ttu-id="93b08-136">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-136">Name of the setting</span></span>|
|<span data-ttu-id="93b08-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="93b08-137">instancePath</span></span>|<span data-ttu-id="93b08-138">String</span><span class="sxs-lookup"><span data-stu-id="93b08-138">String</span></span>|<span data-ttu-id="93b08-139">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="93b08-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="93b08-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-140">unknownDeviceCount</span></span>|<span data-ttu-id="93b08-141">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-141">Int32</span></span>|<span data-ttu-id="93b08-142">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="93b08-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="93b08-144">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-144">Int32</span></span>|<span data-ttu-id="93b08-145">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="93b08-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-146">compliantDeviceCount</span></span>|<span data-ttu-id="93b08-147">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-147">Int32</span></span>|<span data-ttu-id="93b08-148">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="93b08-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-149">remediatedDeviceCount</span></span>|<span data-ttu-id="93b08-150">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-150">Int32</span></span>|<span data-ttu-id="93b08-151">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="93b08-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="93b08-153">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-153">Int32</span></span>|<span data-ttu-id="93b08-154">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="93b08-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-155">errorDeviceCount</span></span>|<span data-ttu-id="93b08-156">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-156">Int32</span></span>|<span data-ttu-id="93b08-157">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-157">Device error count for the setting</span></span>|
|<span data-ttu-id="93b08-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="93b08-158">conflictDeviceCount</span></span>|<span data-ttu-id="93b08-159">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-159">Int32</span></span>|<span data-ttu-id="93b08-160">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="93b08-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="93b08-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="93b08-161">Response</span></span>
<span data-ttu-id="93b08-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="93b08-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93b08-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93b08-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="93b08-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93b08-164">Request</span></span>
<span data-ttu-id="93b08-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93b08-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="93b08-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="93b08-166">Response</span></span>
<span data-ttu-id="93b08-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93b08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




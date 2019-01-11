---
title: Aktualisieren von „settingStateDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3927f039164c8b8e5be4092615cd213f505d7e76
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845836"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="92904-103">Aktualisieren von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="92904-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="92904-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="92904-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92904-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="92904-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92904-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92904-106">Prerequisites</span></span>
<span data-ttu-id="92904-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92904-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92904-109">Permission type</span></span>|<span data-ttu-id="92904-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92904-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92904-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92904-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92904-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92904-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92904-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92904-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92904-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92904-114">Not supported.</span></span>|
|<span data-ttu-id="92904-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92904-115">Application</span></span>|<span data-ttu-id="92904-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92904-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92904-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92904-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="92904-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92904-118">Request headers</span></span>
|<span data-ttu-id="92904-119">Header</span><span class="sxs-lookup"><span data-stu-id="92904-119">Header</span></span>|<span data-ttu-id="92904-120">Wert</span><span class="sxs-lookup"><span data-stu-id="92904-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92904-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92904-121">Authorization</span></span>|<span data-ttu-id="92904-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92904-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92904-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="92904-123">Accept</span></span>|<span data-ttu-id="92904-124">application/json</span><span class="sxs-lookup"><span data-stu-id="92904-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92904-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92904-125">Request body</span></span>
<span data-ttu-id="92904-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="92904-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="92904-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="92904-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="92904-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92904-128">Property</span></span>|<span data-ttu-id="92904-129">Typ</span><span class="sxs-lookup"><span data-stu-id="92904-129">Type</span></span>|<span data-ttu-id="92904-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92904-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92904-131">id</span><span class="sxs-lookup"><span data-stu-id="92904-131">id</span></span>|<span data-ttu-id="92904-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92904-132">String</span></span>|<span data-ttu-id="92904-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="92904-133">Key of the entity.</span></span>|
|<span data-ttu-id="92904-134">settingName</span><span class="sxs-lookup"><span data-stu-id="92904-134">settingName</span></span>|<span data-ttu-id="92904-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92904-135">String</span></span>|<span data-ttu-id="92904-136">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-136">Name of the setting</span></span>|
|<span data-ttu-id="92904-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="92904-137">instancePath</span></span>|<span data-ttu-id="92904-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="92904-138">String</span></span>|<span data-ttu-id="92904-139">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="92904-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="92904-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-140">unknownDeviceCount</span></span>|<span data-ttu-id="92904-141">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-141">Int32</span></span>|<span data-ttu-id="92904-142">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="92904-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="92904-144">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-144">Int32</span></span>|<span data-ttu-id="92904-145">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="92904-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-146">compliantDeviceCount</span></span>|<span data-ttu-id="92904-147">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-147">Int32</span></span>|<span data-ttu-id="92904-148">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="92904-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-149">remediatedDeviceCount</span></span>|<span data-ttu-id="92904-150">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-150">Int32</span></span>|<span data-ttu-id="92904-151">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="92904-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="92904-153">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-153">Int32</span></span>|<span data-ttu-id="92904-154">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="92904-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-155">errorDeviceCount</span></span>|<span data-ttu-id="92904-156">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-156">Int32</span></span>|<span data-ttu-id="92904-157">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-157">Device error count for the setting</span></span>|
|<span data-ttu-id="92904-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92904-158">conflictDeviceCount</span></span>|<span data-ttu-id="92904-159">Int32</span><span class="sxs-lookup"><span data-stu-id="92904-159">Int32</span></span>|<span data-ttu-id="92904-160">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="92904-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="92904-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="92904-161">Response</span></span>
<span data-ttu-id="92904-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="92904-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92904-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92904-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="92904-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92904-164">Request</span></span>
<span data-ttu-id="92904-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92904-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
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

### <a name="response"></a><span data-ttu-id="92904-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="92904-166">Response</span></span>
<span data-ttu-id="92904-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92904-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




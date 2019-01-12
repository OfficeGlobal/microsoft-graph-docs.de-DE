---
title: Aktualisieren von „settingStateDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 889466321037d72ab3f31d95deb3bd877ede7dbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961442"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="c1619-103">Aktualisieren von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="c1619-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="c1619-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1619-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1619-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c1619-105">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1619-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1619-106">Prerequisites</span></span>
<span data-ttu-id="c1619-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1619-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1619-109">Permission type</span></span>|<span data-ttu-id="c1619-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1619-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1619-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1619-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1619-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1619-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1619-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1619-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1619-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1619-114">Not supported.</span></span>|
|<span data-ttu-id="c1619-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1619-115">Application</span></span>|<span data-ttu-id="c1619-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1619-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1619-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1619-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="c1619-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1619-118">Request headers</span></span>
|<span data-ttu-id="c1619-119">Header</span><span class="sxs-lookup"><span data-stu-id="c1619-119">Header</span></span>|<span data-ttu-id="c1619-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c1619-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1619-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1619-121">Authorization</span></span>|<span data-ttu-id="c1619-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1619-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1619-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1619-123">Accept</span></span>|<span data-ttu-id="c1619-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1619-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1619-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1619-125">Request body</span></span>
<span data-ttu-id="c1619-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="c1619-126">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="c1619-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1619-127">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="c1619-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1619-128">Property</span></span>|<span data-ttu-id="c1619-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c1619-129">Type</span></span>|<span data-ttu-id="c1619-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1619-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1619-131">id</span><span class="sxs-lookup"><span data-stu-id="c1619-131">id</span></span>|<span data-ttu-id="c1619-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1619-132">String</span></span>|<span data-ttu-id="c1619-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1619-133">Key of the entity.</span></span>|
|<span data-ttu-id="c1619-134">settingName</span><span class="sxs-lookup"><span data-stu-id="c1619-134">settingName</span></span>|<span data-ttu-id="c1619-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1619-135">String</span></span>|<span data-ttu-id="c1619-136">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-136">Name of the setting</span></span>|
|<span data-ttu-id="c1619-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="c1619-137">instancePath</span></span>|<span data-ttu-id="c1619-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1619-138">String</span></span>|<span data-ttu-id="c1619-139">Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“</span><span class="sxs-lookup"><span data-stu-id="c1619-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="c1619-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-140">unknownDeviceCount</span></span>|<span data-ttu-id="c1619-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-141">Int32</span></span>|<span data-ttu-id="c1619-142">Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="c1619-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="c1619-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-144">Int32</span></span>|<span data-ttu-id="c1619-145">Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="c1619-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-146">compliantDeviceCount</span></span>|<span data-ttu-id="c1619-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-147">Int32</span></span>|<span data-ttu-id="c1619-148">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="c1619-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-149">remediatedDeviceCount</span></span>|<span data-ttu-id="c1619-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-150">Int32</span></span>|<span data-ttu-id="c1619-151">Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="c1619-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c1619-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-153">Int32</span></span>|<span data-ttu-id="c1619-154">Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="c1619-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-155">errorDeviceCount</span></span>|<span data-ttu-id="c1619-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-156">Int32</span></span>|<span data-ttu-id="c1619-157">Anzahl der Geräte mit Meldung „Error“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-157">Device error count for the setting</span></span>|
|<span data-ttu-id="c1619-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1619-158">conflictDeviceCount</span></span>|<span data-ttu-id="c1619-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c1619-159">Int32</span></span>|<span data-ttu-id="c1619-160">Anzahl der Geräte mit Meldung „Conflict“ für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="c1619-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="c1619-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1619-161">Response</span></span>
<span data-ttu-id="c1619-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1619-162">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1619-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1619-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1619-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1619-164">Request</span></span>
<span data-ttu-id="c1619-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1619-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1619-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1619-166">Response</span></span>
<span data-ttu-id="c1619-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1619-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




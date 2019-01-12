---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4224a90ec0e71508b01c21f22fa6317219090fa4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949787"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="7706b-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="7706b-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="7706b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7706b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7706b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7706b-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7706b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7706b-106">Prerequisites</span></span>
<span data-ttu-id="7706b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7706b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7706b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7706b-109">Permission type</span></span>|<span data-ttu-id="7706b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7706b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7706b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7706b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7706b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7706b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7706b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7706b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7706b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7706b-114">Not supported.</span></span>|
|<span data-ttu-id="7706b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7706b-115">Application</span></span>|<span data-ttu-id="7706b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7706b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7706b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7706b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7706b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7706b-118">Request headers</span></span>
|<span data-ttu-id="7706b-119">Header</span><span class="sxs-lookup"><span data-stu-id="7706b-119">Header</span></span>|<span data-ttu-id="7706b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7706b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7706b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7706b-121">Authorization</span></span>|<span data-ttu-id="7706b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7706b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7706b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7706b-123">Accept</span></span>|<span data-ttu-id="7706b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7706b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7706b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7706b-125">Request body</span></span>
<span data-ttu-id="7706b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="7706b-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="7706b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7706b-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="7706b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7706b-128">Property</span></span>|<span data-ttu-id="7706b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7706b-129">Type</span></span>|<span data-ttu-id="7706b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7706b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7706b-131">id</span><span class="sxs-lookup"><span data-stu-id="7706b-131">id</span></span>|<span data-ttu-id="7706b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7706b-132">String</span></span>|<span data-ttu-id="7706b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7706b-133">Key of the entity.</span></span>|
|<span data-ttu-id="7706b-134">setting</span><span class="sxs-lookup"><span data-stu-id="7706b-134">setting</span></span>|<span data-ttu-id="7706b-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7706b-135">String</span></span>|<span data-ttu-id="7706b-136">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="7706b-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="7706b-137">settingName</span><span class="sxs-lookup"><span data-stu-id="7706b-137">settingName</span></span>|<span data-ttu-id="7706b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7706b-138">String</span></span>|<span data-ttu-id="7706b-139">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="7706b-139">Name of the setting.</span></span>|
|<span data-ttu-id="7706b-140">platformType</span><span class="sxs-lookup"><span data-stu-id="7706b-140">platformType</span></span>|[<span data-ttu-id="7706b-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="7706b-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="7706b-142">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="7706b-142">Setting platform.</span></span> <span data-ttu-id="7706b-143">Mögliche Werte sind: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile` und `all`.</span><span class="sxs-lookup"><span data-stu-id="7706b-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="7706b-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-144">unknownDeviceCount</span></span>|<span data-ttu-id="7706b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-145">Int32</span></span>|<span data-ttu-id="7706b-146">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="7706b-146">Number of unknown devices</span></span>|
|<span data-ttu-id="7706b-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="7706b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-148">Int32</span></span>|<span data-ttu-id="7706b-149">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="7706b-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="7706b-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-150">compliantDeviceCount</span></span>|<span data-ttu-id="7706b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-151">Int32</span></span>|<span data-ttu-id="7706b-152">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="7706b-152">Number of compliant devices</span></span>|
|<span data-ttu-id="7706b-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-153">remediatedDeviceCount</span></span>|<span data-ttu-id="7706b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-154">Int32</span></span>|<span data-ttu-id="7706b-155">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="7706b-155">Number of remediated devices</span></span>|
|<span data-ttu-id="7706b-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7706b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-157">Int32</span></span>|<span data-ttu-id="7706b-158">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="7706b-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7706b-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-159">errorDeviceCount</span></span>|<span data-ttu-id="7706b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-160">Int32</span></span>|<span data-ttu-id="7706b-161">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="7706b-161">Number of error devices</span></span>|
|<span data-ttu-id="7706b-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7706b-162">conflictDeviceCount</span></span>|<span data-ttu-id="7706b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-163">Int32</span></span>|<span data-ttu-id="7706b-164">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="7706b-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="7706b-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="7706b-165">Response</span></span>
<span data-ttu-id="7706b-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7706b-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7706b-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7706b-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="7706b-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7706b-168">Request</span></span>
<span data-ttu-id="7706b-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7706b-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="7706b-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="7706b-170">Response</span></span>
<span data-ttu-id="7706b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7706b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
author: tfitzmac
ms.openlocfilehash: d85aa50045c3378a2a4da7826dcaa3fb968664ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345073"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="30f64-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="30f64-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="30f64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="30f64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30f64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="30f64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30f64-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30f64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30f64-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="30f64-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30f64-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="30f64-108">Prerequisites</span></span>
<span data-ttu-id="30f64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30f64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30f64-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30f64-111">Permission type</span></span>|<span data-ttu-id="30f64-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30f64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30f64-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30f64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30f64-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f64-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30f64-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30f64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30f64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30f64-116">Not supported.</span></span>|
|<span data-ttu-id="30f64-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30f64-117">Application</span></span>|<span data-ttu-id="30f64-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30f64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30f64-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30f64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="30f64-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30f64-120">Request headers</span></span>
|<span data-ttu-id="30f64-121">Header</span><span class="sxs-lookup"><span data-stu-id="30f64-121">Header</span></span>|<span data-ttu-id="30f64-122">Wert</span><span class="sxs-lookup"><span data-stu-id="30f64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30f64-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="30f64-123">Authorization</span></span>|<span data-ttu-id="30f64-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="30f64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30f64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30f64-125">Accept</span></span>|<span data-ttu-id="30f64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30f64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30f64-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30f64-127">Request body</span></span>
<span data-ttu-id="30f64-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="30f64-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="30f64-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="30f64-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="30f64-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30f64-130">Property</span></span>|<span data-ttu-id="30f64-131">Typ</span><span class="sxs-lookup"><span data-stu-id="30f64-131">Type</span></span>|<span data-ttu-id="30f64-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30f64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f64-133">id</span><span class="sxs-lookup"><span data-stu-id="30f64-133">id</span></span>|<span data-ttu-id="30f64-134">String</span><span class="sxs-lookup"><span data-stu-id="30f64-134">String</span></span>|<span data-ttu-id="30f64-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="30f64-135">Key of the entity.</span></span>|
|<span data-ttu-id="30f64-136">setting</span><span class="sxs-lookup"><span data-stu-id="30f64-136">setting</span></span>|<span data-ttu-id="30f64-137">String</span><span class="sxs-lookup"><span data-stu-id="30f64-137">String</span></span>|<span data-ttu-id="30f64-138">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="30f64-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="30f64-139">settingName</span><span class="sxs-lookup"><span data-stu-id="30f64-139">settingName</span></span>|<span data-ttu-id="30f64-140">String</span><span class="sxs-lookup"><span data-stu-id="30f64-140">String</span></span>|<span data-ttu-id="30f64-141">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="30f64-141">Name of the setting.</span></span>|
|<span data-ttu-id="30f64-142">platformType</span><span class="sxs-lookup"><span data-stu-id="30f64-142">platformType</span></span>|[<span data-ttu-id="30f64-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="30f64-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="30f64-144">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="30f64-144">Setting platform.</span></span> <span data-ttu-id="30f64-145">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="30f64-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="30f64-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-146">unknownDeviceCount</span></span>|<span data-ttu-id="30f64-147">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-147">Int32</span></span>|<span data-ttu-id="30f64-148">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="30f64-148">Number of unknown devices</span></span>|
|<span data-ttu-id="30f64-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="30f64-150">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-150">Int32</span></span>|<span data-ttu-id="30f64-151">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="30f64-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="30f64-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-152">compliantDeviceCount</span></span>|<span data-ttu-id="30f64-153">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-153">Int32</span></span>|<span data-ttu-id="30f64-154">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="30f64-154">Number of compliant devices</span></span>|
|<span data-ttu-id="30f64-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-155">remediatedDeviceCount</span></span>|<span data-ttu-id="30f64-156">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-156">Int32</span></span>|<span data-ttu-id="30f64-157">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="30f64-157">Number of remediated devices</span></span>|
|<span data-ttu-id="30f64-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="30f64-159">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-159">Int32</span></span>|<span data-ttu-id="30f64-160">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="30f64-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="30f64-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-161">errorDeviceCount</span></span>|<span data-ttu-id="30f64-162">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-162">Int32</span></span>|<span data-ttu-id="30f64-163">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="30f64-163">Number of error devices</span></span>|
|<span data-ttu-id="30f64-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30f64-164">conflictDeviceCount</span></span>|<span data-ttu-id="30f64-165">Int32</span><span class="sxs-lookup"><span data-stu-id="30f64-165">Int32</span></span>|<span data-ttu-id="30f64-166">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="30f64-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="30f64-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="30f64-167">Response</span></span>
<span data-ttu-id="30f64-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="30f64-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30f64-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30f64-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="30f64-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30f64-170">Request</span></span>
<span data-ttu-id="30f64-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30f64-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 322

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="30f64-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="30f64-172">Response</span></span>
<span data-ttu-id="30f64-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30f64-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






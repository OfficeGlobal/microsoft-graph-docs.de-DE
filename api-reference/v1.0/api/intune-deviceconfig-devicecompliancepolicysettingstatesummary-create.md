---
title: deviceCompliancePolicySettingStateSummary erstellen
description: Erstellen eines neuen deviceCompliancePolicySettingStateSummary-Objekts.
ms.openlocfilehash: f7924b8ec3e8c32ccd62899a8576d56c85f0b233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019385"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="60d58-103">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="60d58-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="60d58-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60d58-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60d58-105">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="60d58-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60d58-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="60d58-106">Prerequisites</span></span>
<span data-ttu-id="60d58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d58-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60d58-109">Permission type</span></span>|<span data-ttu-id="60d58-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60d58-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60d58-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60d58-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60d58-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d58-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60d58-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60d58-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60d58-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60d58-114">Not supported.</span></span>|
|<span data-ttu-id="60d58-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60d58-115">Application</span></span>|<span data-ttu-id="60d58-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60d58-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60d58-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60d58-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="60d58-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60d58-118">Request headers</span></span>
|<span data-ttu-id="60d58-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="60d58-119">Header</span></span>|<span data-ttu-id="60d58-120">Wert</span><span class="sxs-lookup"><span data-stu-id="60d58-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60d58-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="60d58-121">Authorization</span></span>|<span data-ttu-id="60d58-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="60d58-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60d58-123">Accept</span><span class="sxs-lookup"><span data-stu-id="60d58-123">Accept</span></span>|<span data-ttu-id="60d58-124">application/json</span><span class="sxs-lookup"><span data-stu-id="60d58-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d58-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60d58-125">Request body</span></span>
<span data-ttu-id="60d58-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="60d58-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="60d58-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="60d58-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="60d58-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60d58-128">Property</span></span>|<span data-ttu-id="60d58-129">Typ</span><span class="sxs-lookup"><span data-stu-id="60d58-129">Type</span></span>|<span data-ttu-id="60d58-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60d58-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60d58-131">id</span><span class="sxs-lookup"><span data-stu-id="60d58-131">id</span></span>|<span data-ttu-id="60d58-132">String</span><span class="sxs-lookup"><span data-stu-id="60d58-132">String</span></span>|<span data-ttu-id="60d58-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="60d58-133">Key of the entity.</span></span>|
|<span data-ttu-id="60d58-134">setting</span><span class="sxs-lookup"><span data-stu-id="60d58-134">setting</span></span>|<span data-ttu-id="60d58-135">String</span><span class="sxs-lookup"><span data-stu-id="60d58-135">String</span></span>|<span data-ttu-id="60d58-136">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="60d58-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="60d58-137">settingName</span><span class="sxs-lookup"><span data-stu-id="60d58-137">settingName</span></span>|<span data-ttu-id="60d58-138">String</span><span class="sxs-lookup"><span data-stu-id="60d58-138">String</span></span>|<span data-ttu-id="60d58-139">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="60d58-139">Name of the setting.</span></span>|
|<span data-ttu-id="60d58-140">platformType</span><span class="sxs-lookup"><span data-stu-id="60d58-140">platformType</span></span>|[<span data-ttu-id="60d58-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="60d58-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="60d58-142">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="60d58-142">Setting platform.</span></span> <span data-ttu-id="60d58-143">Mögliche Werte sind: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile` und `all`.</span><span class="sxs-lookup"><span data-stu-id="60d58-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="60d58-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-144">unknownDeviceCount</span></span>|<span data-ttu-id="60d58-145">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-145">Int32</span></span>|<span data-ttu-id="60d58-146">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="60d58-146">Number of unknown devices</span></span>|
|<span data-ttu-id="60d58-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="60d58-148">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-148">Int32</span></span>|<span data-ttu-id="60d58-149">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="60d58-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="60d58-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-150">compliantDeviceCount</span></span>|<span data-ttu-id="60d58-151">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-151">Int32</span></span>|<span data-ttu-id="60d58-152">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="60d58-152">Number of compliant devices</span></span>|
|<span data-ttu-id="60d58-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-153">remediatedDeviceCount</span></span>|<span data-ttu-id="60d58-154">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-154">Int32</span></span>|<span data-ttu-id="60d58-155">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="60d58-155">Number of remediated devices</span></span>|
|<span data-ttu-id="60d58-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="60d58-157">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-157">Int32</span></span>|<span data-ttu-id="60d58-158">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="60d58-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="60d58-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-159">errorDeviceCount</span></span>|<span data-ttu-id="60d58-160">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-160">Int32</span></span>|<span data-ttu-id="60d58-161">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="60d58-161">Number of error devices</span></span>|
|<span data-ttu-id="60d58-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="60d58-162">conflictDeviceCount</span></span>|<span data-ttu-id="60d58-163">Int32</span><span class="sxs-lookup"><span data-stu-id="60d58-163">Int32</span></span>|<span data-ttu-id="60d58-164">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="60d58-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="60d58-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="60d58-165">Response</span></span>
<span data-ttu-id="60d58-166">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60d58-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60d58-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60d58-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="60d58-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60d58-168">Request</span></span>
<span data-ttu-id="60d58-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60d58-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="60d58-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="60d58-170">Response</span></span>
<span data-ttu-id="60d58-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60d58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




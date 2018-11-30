---
title: deviceCompliancePolicySettingStateSummary erstellen
description: Erstellen eines neuen deviceCompliancePolicySettingStateSummary-Objekts.
ms.openlocfilehash: f7fd5a8d65655b4015d0fcf6dee6377e008b9c99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058922"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="975f4-103">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="975f4-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="975f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="975f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="975f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="975f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="975f4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="975f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="975f4-107">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="975f4-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="975f4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="975f4-108">Prerequisites</span></span>
<span data-ttu-id="975f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="975f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="975f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="975f4-111">Permission type</span></span>|<span data-ttu-id="975f4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="975f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="975f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="975f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="975f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="975f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="975f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="975f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="975f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975f4-116">Not supported.</span></span>|
|<span data-ttu-id="975f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="975f4-117">Application</span></span>|<span data-ttu-id="975f4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="975f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="975f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="975f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="975f4-120">Request headers</span></span>
|<span data-ttu-id="975f4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="975f4-121">Header</span></span>|<span data-ttu-id="975f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="975f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="975f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="975f4-123">Authorization</span></span>|<span data-ttu-id="975f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="975f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="975f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="975f4-125">Accept</span></span>|<span data-ttu-id="975f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="975f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="975f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="975f4-127">Request body</span></span>
<span data-ttu-id="975f4-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="975f4-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="975f4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="975f4-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="975f4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="975f4-130">Property</span></span>|<span data-ttu-id="975f4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="975f4-131">Type</span></span>|<span data-ttu-id="975f4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="975f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="975f4-133">id</span><span class="sxs-lookup"><span data-stu-id="975f4-133">id</span></span>|<span data-ttu-id="975f4-134">String</span><span class="sxs-lookup"><span data-stu-id="975f4-134">String</span></span>|<span data-ttu-id="975f4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="975f4-135">Key of the entity.</span></span>|
|<span data-ttu-id="975f4-136">setting</span><span class="sxs-lookup"><span data-stu-id="975f4-136">setting</span></span>|<span data-ttu-id="975f4-137">String</span><span class="sxs-lookup"><span data-stu-id="975f4-137">String</span></span>|<span data-ttu-id="975f4-138">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="975f4-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="975f4-139">settingName</span><span class="sxs-lookup"><span data-stu-id="975f4-139">settingName</span></span>|<span data-ttu-id="975f4-140">String</span><span class="sxs-lookup"><span data-stu-id="975f4-140">String</span></span>|<span data-ttu-id="975f4-141">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="975f4-141">Name of the setting.</span></span>|
|<span data-ttu-id="975f4-142">platformType</span><span class="sxs-lookup"><span data-stu-id="975f4-142">platformType</span></span>|[<span data-ttu-id="975f4-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="975f4-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="975f4-144">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="975f4-144">Setting platform.</span></span> <span data-ttu-id="975f4-145">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="975f4-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="975f4-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-146">unknownDeviceCount</span></span>|<span data-ttu-id="975f4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-147">Int32</span></span>|<span data-ttu-id="975f4-148">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="975f4-148">Number of unknown devices</span></span>|
|<span data-ttu-id="975f4-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="975f4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-150">Int32</span></span>|<span data-ttu-id="975f4-151">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="975f4-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="975f4-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-152">compliantDeviceCount</span></span>|<span data-ttu-id="975f4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-153">Int32</span></span>|<span data-ttu-id="975f4-154">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="975f4-154">Number of compliant devices</span></span>|
|<span data-ttu-id="975f4-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-155">remediatedDeviceCount</span></span>|<span data-ttu-id="975f4-156">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-156">Int32</span></span>|<span data-ttu-id="975f4-157">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="975f4-157">Number of remediated devices</span></span>|
|<span data-ttu-id="975f4-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="975f4-159">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-159">Int32</span></span>|<span data-ttu-id="975f4-160">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="975f4-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="975f4-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-161">errorDeviceCount</span></span>|<span data-ttu-id="975f4-162">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-162">Int32</span></span>|<span data-ttu-id="975f4-163">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="975f4-163">Number of error devices</span></span>|
|<span data-ttu-id="975f4-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="975f4-164">conflictDeviceCount</span></span>|<span data-ttu-id="975f4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="975f4-165">Int32</span></span>|<span data-ttu-id="975f4-166">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="975f4-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="975f4-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="975f4-167">Response</span></span>
<span data-ttu-id="975f4-168">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="975f4-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="975f4-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="975f4-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="975f4-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="975f4-170">Request</span></span>
<span data-ttu-id="975f4-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="975f4-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
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

### <a name="response"></a><span data-ttu-id="975f4-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="975f4-172">Response</span></span>
<span data-ttu-id="975f4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="975f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






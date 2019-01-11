---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b739f136252658385a3ef94edd959c855d2f0032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873788"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="b4923-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="b4923-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="b4923-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4923-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4923-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4923-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4923-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4923-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4923-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="b4923-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4923-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4923-108">Prerequisites</span></span>
<span data-ttu-id="b4923-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4923-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4923-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4923-111">Permission type</span></span>|<span data-ttu-id="b4923-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4923-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4923-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4923-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4923-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4923-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4923-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4923-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4923-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4923-116">Not supported.</span></span>|
|<span data-ttu-id="b4923-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4923-117">Application</span></span>|<span data-ttu-id="b4923-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4923-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4923-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4923-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b4923-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4923-120">Request headers</span></span>
|<span data-ttu-id="b4923-121">Header</span><span class="sxs-lookup"><span data-stu-id="b4923-121">Header</span></span>|<span data-ttu-id="b4923-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b4923-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4923-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4923-123">Authorization</span></span>|<span data-ttu-id="b4923-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4923-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4923-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4923-125">Accept</span></span>|<span data-ttu-id="b4923-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4923-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4923-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4923-127">Request body</span></span>
<span data-ttu-id="b4923-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="b4923-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="b4923-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4923-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="b4923-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4923-130">Property</span></span>|<span data-ttu-id="b4923-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b4923-131">Type</span></span>|<span data-ttu-id="b4923-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4923-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4923-133">id</span><span class="sxs-lookup"><span data-stu-id="b4923-133">id</span></span>|<span data-ttu-id="b4923-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4923-134">String</span></span>|<span data-ttu-id="b4923-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4923-135">Key of the entity.</span></span>|
|<span data-ttu-id="b4923-136">setting</span><span class="sxs-lookup"><span data-stu-id="b4923-136">setting</span></span>|<span data-ttu-id="b4923-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4923-137">String</span></span>|<span data-ttu-id="b4923-138">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="b4923-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="b4923-139">settingName</span><span class="sxs-lookup"><span data-stu-id="b4923-139">settingName</span></span>|<span data-ttu-id="b4923-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4923-140">String</span></span>|<span data-ttu-id="b4923-141">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="b4923-141">Name of the setting.</span></span>|
|<span data-ttu-id="b4923-142">platformType</span><span class="sxs-lookup"><span data-stu-id="b4923-142">platformType</span></span>|[<span data-ttu-id="b4923-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="b4923-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="b4923-144">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="b4923-144">Setting platform.</span></span> <span data-ttu-id="b4923-145">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b4923-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="b4923-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-146">unknownDeviceCount</span></span>|<span data-ttu-id="b4923-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-147">Int32</span></span>|<span data-ttu-id="b4923-148">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="b4923-148">Number of unknown devices</span></span>|
|<span data-ttu-id="b4923-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="b4923-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-150">Int32</span></span>|<span data-ttu-id="b4923-151">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="b4923-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="b4923-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-152">compliantDeviceCount</span></span>|<span data-ttu-id="b4923-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-153">Int32</span></span>|<span data-ttu-id="b4923-154">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="b4923-154">Number of compliant devices</span></span>|
|<span data-ttu-id="b4923-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-155">remediatedDeviceCount</span></span>|<span data-ttu-id="b4923-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-156">Int32</span></span>|<span data-ttu-id="b4923-157">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="b4923-157">Number of remediated devices</span></span>|
|<span data-ttu-id="b4923-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b4923-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-159">Int32</span></span>|<span data-ttu-id="b4923-160">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="b4923-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b4923-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-161">errorDeviceCount</span></span>|<span data-ttu-id="b4923-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-162">Int32</span></span>|<span data-ttu-id="b4923-163">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="b4923-163">Number of error devices</span></span>|
|<span data-ttu-id="b4923-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4923-164">conflictDeviceCount</span></span>|<span data-ttu-id="b4923-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b4923-165">Int32</span></span>|<span data-ttu-id="b4923-166">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="b4923-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="b4923-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4923-167">Response</span></span>
<span data-ttu-id="b4923-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4923-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4923-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4923-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4923-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4923-170">Request</span></span>
<span data-ttu-id="b4923-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4923-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4923-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4923-172">Response</span></span>
<span data-ttu-id="b4923-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4923-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






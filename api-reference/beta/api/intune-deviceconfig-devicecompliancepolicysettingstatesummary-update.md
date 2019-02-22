---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 216c5005b9d6a33e10accccd728f9f0d40e9d2ec
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171911"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="75f10-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="75f10-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="75f10-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75f10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75f10-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="75f10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75f10-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="75f10-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75f10-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75f10-107">Prerequisites</span></span>
<span data-ttu-id="75f10-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="75f10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="75f10-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75f10-110">Permission type</span></span>|<span data-ttu-id="75f10-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75f10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f10-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75f10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75f10-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f10-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75f10-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75f10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f10-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75f10-115">Not supported.</span></span>|
|<span data-ttu-id="75f10-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75f10-116">Application</span></span>|<span data-ttu-id="75f10-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75f10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f10-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75f10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="75f10-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75f10-119">Request headers</span></span>
|<span data-ttu-id="75f10-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="75f10-120">Header</span></span>|<span data-ttu-id="75f10-121">Wert</span><span class="sxs-lookup"><span data-stu-id="75f10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75f10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75f10-122">Authorization</span></span>|<span data-ttu-id="75f10-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="75f10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75f10-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="75f10-124">Accept</span></span>|<span data-ttu-id="75f10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75f10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f10-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75f10-126">Request body</span></span>
<span data-ttu-id="75f10-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="75f10-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="75f10-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="75f10-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="75f10-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75f10-129">Property</span></span>|<span data-ttu-id="75f10-130">Typ</span><span class="sxs-lookup"><span data-stu-id="75f10-130">Type</span></span>|<span data-ttu-id="75f10-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75f10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f10-132">id</span><span class="sxs-lookup"><span data-stu-id="75f10-132">id</span></span>|<span data-ttu-id="75f10-133">String</span><span class="sxs-lookup"><span data-stu-id="75f10-133">String</span></span>|<span data-ttu-id="75f10-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="75f10-134">Key of the entity.</span></span>|
|<span data-ttu-id="75f10-135">setting</span><span class="sxs-lookup"><span data-stu-id="75f10-135">setting</span></span>|<span data-ttu-id="75f10-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75f10-136">String</span></span>|<span data-ttu-id="75f10-137">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="75f10-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="75f10-138">settingName</span><span class="sxs-lookup"><span data-stu-id="75f10-138">settingName</span></span>|<span data-ttu-id="75f10-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75f10-139">String</span></span>|<span data-ttu-id="75f10-140">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="75f10-140">Name of the setting.</span></span>|
|<span data-ttu-id="75f10-141">platformType</span><span class="sxs-lookup"><span data-stu-id="75f10-141">platformType</span></span>|[<span data-ttu-id="75f10-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="75f10-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="75f10-143">Einstellungs Plattform.</span><span class="sxs-lookup"><span data-stu-id="75f10-143">Setting platform.</span></span> <span data-ttu-id="75f10-144">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="75f10-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="75f10-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-145">unknownDeviceCount</span></span>|<span data-ttu-id="75f10-146">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-146">Int32</span></span>|<span data-ttu-id="75f10-147">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="75f10-147">Number of unknown devices</span></span>|
|<span data-ttu-id="75f10-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="75f10-149">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-149">Int32</span></span>|<span data-ttu-id="75f10-150">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="75f10-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="75f10-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-151">compliantDeviceCount</span></span>|<span data-ttu-id="75f10-152">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-152">Int32</span></span>|<span data-ttu-id="75f10-153">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="75f10-153">Number of compliant devices</span></span>|
|<span data-ttu-id="75f10-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-154">remediatedDeviceCount</span></span>|<span data-ttu-id="75f10-155">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-155">Int32</span></span>|<span data-ttu-id="75f10-156">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="75f10-156">Number of remediated devices</span></span>|
|<span data-ttu-id="75f10-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="75f10-158">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-158">Int32</span></span>|<span data-ttu-id="75f10-159">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="75f10-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="75f10-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-160">errorDeviceCount</span></span>|<span data-ttu-id="75f10-161">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-161">Int32</span></span>|<span data-ttu-id="75f10-162">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="75f10-162">Number of error devices</span></span>|
|<span data-ttu-id="75f10-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75f10-163">conflictDeviceCount</span></span>|<span data-ttu-id="75f10-164">Int32</span><span class="sxs-lookup"><span data-stu-id="75f10-164">Int32</span></span>|<span data-ttu-id="75f10-165">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="75f10-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="75f10-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="75f10-166">Response</span></span>
<span data-ttu-id="75f10-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="75f10-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75f10-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75f10-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="75f10-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75f10-169">Request</span></span>
<span data-ttu-id="75f10-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75f10-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="75f10-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="75f10-171">Response</span></span>
<span data-ttu-id="75f10-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75f10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





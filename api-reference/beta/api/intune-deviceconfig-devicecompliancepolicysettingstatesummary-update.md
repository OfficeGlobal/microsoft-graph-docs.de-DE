---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc3e5652522f5b3968b6a8c9994ffe1a47629940
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966383"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a413c-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="a413c-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="a413c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a413c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a413c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a413c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a413c-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a413c-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a413c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a413c-107">Prerequisites</span></span>
<span data-ttu-id="a413c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a413c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a413c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a413c-110">Permission type</span></span>|<span data-ttu-id="a413c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a413c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a413c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a413c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a413c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a413c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a413c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a413c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a413c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a413c-115">Not supported.</span></span>|
|<span data-ttu-id="a413c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a413c-116">Application</span></span>|<span data-ttu-id="a413c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a413c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a413c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a413c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a413c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a413c-119">Request headers</span></span>
|<span data-ttu-id="a413c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a413c-120">Header</span></span>|<span data-ttu-id="a413c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a413c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a413c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a413c-122">Authorization</span></span>|<span data-ttu-id="a413c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a413c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a413c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a413c-124">Accept</span></span>|<span data-ttu-id="a413c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a413c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a413c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a413c-126">Request body</span></span>
<span data-ttu-id="a413c-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="a413c-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="a413c-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a413c-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="a413c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a413c-129">Property</span></span>|<span data-ttu-id="a413c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a413c-130">Type</span></span>|<span data-ttu-id="a413c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a413c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a413c-132">id</span><span class="sxs-lookup"><span data-stu-id="a413c-132">id</span></span>|<span data-ttu-id="a413c-133">String</span><span class="sxs-lookup"><span data-stu-id="a413c-133">String</span></span>|<span data-ttu-id="a413c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a413c-134">Key of the entity.</span></span>|
|<span data-ttu-id="a413c-135">Einstellung</span><span class="sxs-lookup"><span data-stu-id="a413c-135">setting</span></span>|<span data-ttu-id="a413c-136">String</span><span class="sxs-lookup"><span data-stu-id="a413c-136">String</span></span>|<span data-ttu-id="a413c-137">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="a413c-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="a413c-138">settingName</span><span class="sxs-lookup"><span data-stu-id="a413c-138">settingName</span></span>|<span data-ttu-id="a413c-139">String</span><span class="sxs-lookup"><span data-stu-id="a413c-139">String</span></span>|<span data-ttu-id="a413c-140">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="a413c-140">Name of the setting.</span></span>|
|<span data-ttu-id="a413c-141">platformType</span><span class="sxs-lookup"><span data-stu-id="a413c-141">platformType</span></span>|[<span data-ttu-id="a413c-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a413c-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a413c-143">Einstellungs Plattform.</span><span class="sxs-lookup"><span data-stu-id="a413c-143">Setting platform.</span></span> <span data-ttu-id="a413c-144">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a413c-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a413c-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-145">unknownDeviceCount</span></span>|<span data-ttu-id="a413c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-146">Int32</span></span>|<span data-ttu-id="a413c-147">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-147">Number of unknown devices</span></span>|
|<span data-ttu-id="a413c-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="a413c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-149">Int32</span></span>|<span data-ttu-id="a413c-150">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="a413c-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-151">compliantDeviceCount</span></span>|<span data-ttu-id="a413c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-152">Int32</span></span>|<span data-ttu-id="a413c-153">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-153">Number of compliant devices</span></span>|
|<span data-ttu-id="a413c-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-154">remediatedDeviceCount</span></span>|<span data-ttu-id="a413c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-155">Int32</span></span>|<span data-ttu-id="a413c-156">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-156">Number of remediated devices</span></span>|
|<span data-ttu-id="a413c-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a413c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-158">Int32</span></span>|<span data-ttu-id="a413c-159">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a413c-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-160">errorDeviceCount</span></span>|<span data-ttu-id="a413c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-161">Int32</span></span>|<span data-ttu-id="a413c-162">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="a413c-162">Number of error devices</span></span>|
|<span data-ttu-id="a413c-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a413c-163">conflictDeviceCount</span></span>|<span data-ttu-id="a413c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a413c-164">Int32</span></span>|<span data-ttu-id="a413c-165">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="a413c-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a413c-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a413c-166">Response</span></span>
<span data-ttu-id="a413c-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a413c-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a413c-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a413c-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a413c-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a413c-169">Request</span></span>
<span data-ttu-id="a413c-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a413c-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a413c-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a413c-171">Response</span></span>
<span data-ttu-id="a413c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a413c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





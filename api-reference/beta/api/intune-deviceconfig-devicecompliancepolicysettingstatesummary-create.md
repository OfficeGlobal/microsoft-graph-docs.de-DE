---
title: deviceCompliancePolicySettingStateSummary erstellen
description: Erstellen eines neuen deviceCompliancePolicySettingStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6aac612b6a94a59ff17d12d5a328b5eac793e3e9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986551"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a5df8-103">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="a5df8-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="a5df8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5df8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5df8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5df8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5df8-106">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a5df8-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5df8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a5df8-107">Prerequisites</span></span>
<span data-ttu-id="a5df8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5df8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5df8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5df8-110">Permission type</span></span>|<span data-ttu-id="a5df8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5df8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5df8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5df8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5df8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5df8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5df8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5df8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5df8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5df8-115">Not supported.</span></span>|
|<span data-ttu-id="a5df8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5df8-116">Application</span></span>|<span data-ttu-id="a5df8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5df8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5df8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5df8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a5df8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5df8-119">Request headers</span></span>
|<span data-ttu-id="a5df8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a5df8-120">Header</span></span>|<span data-ttu-id="a5df8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a5df8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5df8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5df8-122">Authorization</span></span>|<span data-ttu-id="a5df8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a5df8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5df8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a5df8-124">Accept</span></span>|<span data-ttu-id="a5df8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5df8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5df8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5df8-126">Request body</span></span>
<span data-ttu-id="a5df8-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="a5df8-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="a5df8-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5df8-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="a5df8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5df8-129">Property</span></span>|<span data-ttu-id="a5df8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a5df8-130">Type</span></span>|<span data-ttu-id="a5df8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5df8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5df8-132">id</span><span class="sxs-lookup"><span data-stu-id="a5df8-132">id</span></span>|<span data-ttu-id="a5df8-133">String</span><span class="sxs-lookup"><span data-stu-id="a5df8-133">String</span></span>|<span data-ttu-id="a5df8-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a5df8-134">Key of the entity.</span></span>|
|<span data-ttu-id="a5df8-135">Einstellung</span><span class="sxs-lookup"><span data-stu-id="a5df8-135">setting</span></span>|<span data-ttu-id="a5df8-136">String</span><span class="sxs-lookup"><span data-stu-id="a5df8-136">String</span></span>|<span data-ttu-id="a5df8-137">Der Klassenname und der Eigenschaftenname der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="a5df8-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="a5df8-138">settingName</span><span class="sxs-lookup"><span data-stu-id="a5df8-138">settingName</span></span>|<span data-ttu-id="a5df8-139">String</span><span class="sxs-lookup"><span data-stu-id="a5df8-139">String</span></span>|<span data-ttu-id="a5df8-140">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="a5df8-140">Name of the setting.</span></span>|
|<span data-ttu-id="a5df8-141">platformType</span><span class="sxs-lookup"><span data-stu-id="a5df8-141">platformType</span></span>|[<span data-ttu-id="a5df8-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a5df8-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a5df8-143">Einstellungs Plattform.</span><span class="sxs-lookup"><span data-stu-id="a5df8-143">Setting platform.</span></span> <span data-ttu-id="a5df8-144">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a5df8-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a5df8-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-145">unknownDeviceCount</span></span>|<span data-ttu-id="a5df8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-146">Int32</span></span>|<span data-ttu-id="a5df8-147">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-147">Number of unknown devices</span></span>|
|<span data-ttu-id="a5df8-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="a5df8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-149">Int32</span></span>|<span data-ttu-id="a5df8-150">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="a5df8-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-151">compliantDeviceCount</span></span>|<span data-ttu-id="a5df8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-152">Int32</span></span>|<span data-ttu-id="a5df8-153">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-153">Number of compliant devices</span></span>|
|<span data-ttu-id="a5df8-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-154">remediatedDeviceCount</span></span>|<span data-ttu-id="a5df8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-155">Int32</span></span>|<span data-ttu-id="a5df8-156">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-156">Number of remediated devices</span></span>|
|<span data-ttu-id="a5df8-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a5df8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-158">Int32</span></span>|<span data-ttu-id="a5df8-159">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a5df8-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-160">errorDeviceCount</span></span>|<span data-ttu-id="a5df8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-161">Int32</span></span>|<span data-ttu-id="a5df8-162">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="a5df8-162">Number of error devices</span></span>|
|<span data-ttu-id="a5df8-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5df8-163">conflictDeviceCount</span></span>|<span data-ttu-id="a5df8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a5df8-164">Int32</span></span>|<span data-ttu-id="a5df8-165">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="a5df8-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a5df8-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5df8-166">Response</span></span>
<span data-ttu-id="a5df8-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5df8-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5df8-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5df8-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5df8-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5df8-169">Request</span></span>
<span data-ttu-id="a5df8-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a5df8-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a5df8-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5df8-171">Response</span></span>
<span data-ttu-id="a5df8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5df8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





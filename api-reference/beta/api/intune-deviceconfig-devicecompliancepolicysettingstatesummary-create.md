---
title: deviceCompliancePolicySettingStateSummary erstellen
description: Erstellen eines neuen deviceCompliancePolicySettingStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 110b3853c7e36280cf530f6d5d18a197cfd33230
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170924"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a3e6d-103">deviceCompliancePolicySettingStateSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="a3e6d-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="a3e6d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e6d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e6d-106">Erstellen eines neuen [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3e6d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3e6d-107">Prerequisites</span></span>
<span data-ttu-id="a3e6d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3e6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3e6d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3e6d-110">Permission type</span></span>|<span data-ttu-id="a3e6d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3e6d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e6d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3e6d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e6d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3e6d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3e6d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3e6d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e6d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3e6d-115">Not supported.</span></span>|
|<span data-ttu-id="a3e6d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-116">Application</span></span>|<span data-ttu-id="a3e6d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3e6d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e6d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a3e6d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3e6d-119">Request headers</span></span>
|<span data-ttu-id="a3e6d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3e6d-120">Header</span></span>|<span data-ttu-id="a3e6d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a3e6d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3e6d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e6d-122">Authorization</span></span>|<span data-ttu-id="a3e6d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3e6d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3e6d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3e6d-124">Accept</span></span>|<span data-ttu-id="a3e6d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3e6d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e6d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3e6d-126">Request body</span></span>
<span data-ttu-id="a3e6d-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceCompliancePolicySettingStateSummary an.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="a3e6d-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceCompliancePolicySettingStateSummary erstellen.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="a3e6d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3e6d-129">Property</span></span>|<span data-ttu-id="a3e6d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a3e6d-130">Type</span></span>|<span data-ttu-id="a3e6d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e6d-132">id</span><span class="sxs-lookup"><span data-stu-id="a3e6d-132">id</span></span>|<span data-ttu-id="a3e6d-133">String</span><span class="sxs-lookup"><span data-stu-id="a3e6d-133">String</span></span>|<span data-ttu-id="a3e6d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a3e6d-134">Key of the entity.</span></span>|
|<span data-ttu-id="a3e6d-135">setting</span><span class="sxs-lookup"><span data-stu-id="a3e6d-135">setting</span></span>|<span data-ttu-id="a3e6d-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3e6d-136">String</span></span>|<span data-ttu-id="a3e6d-137">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="a3e6d-138">settingName</span><span class="sxs-lookup"><span data-stu-id="a3e6d-138">settingName</span></span>|<span data-ttu-id="a3e6d-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3e6d-139">String</span></span>|<span data-ttu-id="a3e6d-140">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-140">Name of the setting.</span></span>|
|<span data-ttu-id="a3e6d-141">platformType</span><span class="sxs-lookup"><span data-stu-id="a3e6d-141">platformType</span></span>|[<span data-ttu-id="a3e6d-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a3e6d-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a3e6d-143">Einstellungs Plattform.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-143">Setting platform.</span></span> <span data-ttu-id="a3e6d-144">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a3e6d-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-145">unknownDeviceCount</span></span>|<span data-ttu-id="a3e6d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-146">Int32</span></span>|<span data-ttu-id="a3e6d-147">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="a3e6d-147">Number of unknown devices</span></span>|
|<span data-ttu-id="a3e6d-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="a3e6d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-149">Int32</span></span>|<span data-ttu-id="a3e6d-150">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="a3e6d-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="a3e6d-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-151">compliantDeviceCount</span></span>|<span data-ttu-id="a3e6d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-152">Int32</span></span>|<span data-ttu-id="a3e6d-153">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="a3e6d-153">Number of compliant devices</span></span>|
|<span data-ttu-id="a3e6d-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-154">remediatedDeviceCount</span></span>|<span data-ttu-id="a3e6d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-155">Int32</span></span>|<span data-ttu-id="a3e6d-156">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="a3e6d-156">Number of remediated devices</span></span>|
|<span data-ttu-id="a3e6d-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a3e6d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-158">Int32</span></span>|<span data-ttu-id="a3e6d-159">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="a3e6d-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a3e6d-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-160">errorDeviceCount</span></span>|<span data-ttu-id="a3e6d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-161">Int32</span></span>|<span data-ttu-id="a3e6d-162">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="a3e6d-162">Number of error devices</span></span>|
|<span data-ttu-id="a3e6d-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a3e6d-163">conflictDeviceCount</span></span>|<span data-ttu-id="a3e6d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e6d-164">Int32</span></span>|<span data-ttu-id="a3e6d-165">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="a3e6d-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a3e6d-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3e6d-166">Response</span></span>
<span data-ttu-id="a3e6d-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e6d-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3e6d-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3e6d-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3e6d-169">Request</span></span>
<span data-ttu-id="a3e6d-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3e6d-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3e6d-171">Response</span></span>
<span data-ttu-id="a3e6d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3e6d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Aktualisieren von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicySettingStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43aaa3b1269a6de2862ad15b8fda03eb92ec0631
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409776"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="9cd22-103">Aktualisieren von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="9cd22-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="9cd22-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9cd22-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cd22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cd22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cd22-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9cd22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cd22-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9cd22-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cd22-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9cd22-108">Prerequisites</span></span>
<span data-ttu-id="9cd22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cd22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9cd22-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9cd22-111">Permission type</span></span>|<span data-ttu-id="9cd22-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9cd22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cd22-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9cd22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cd22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cd22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cd22-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9cd22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cd22-116">Not supported.</span></span>|
|<span data-ttu-id="9cd22-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9cd22-117">Application</span></span>|<span data-ttu-id="9cd22-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cd22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cd22-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cd22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="9cd22-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9cd22-120">Request headers</span></span>
|<span data-ttu-id="9cd22-121">Header</span><span class="sxs-lookup"><span data-stu-id="9cd22-121">Header</span></span>|<span data-ttu-id="9cd22-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9cd22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cd22-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9cd22-123">Authorization</span></span>|<span data-ttu-id="9cd22-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9cd22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cd22-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9cd22-125">Accept</span></span>|<span data-ttu-id="9cd22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cd22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cd22-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9cd22-127">Request body</span></span>
<span data-ttu-id="9cd22-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="9cd22-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="9cd22-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9cd22-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="9cd22-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cd22-130">Property</span></span>|<span data-ttu-id="9cd22-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9cd22-131">Type</span></span>|<span data-ttu-id="9cd22-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cd22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cd22-133">id</span><span class="sxs-lookup"><span data-stu-id="9cd22-133">id</span></span>|<span data-ttu-id="9cd22-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cd22-134">String</span></span>|<span data-ttu-id="9cd22-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9cd22-135">Key of the entity.</span></span>|
|<span data-ttu-id="9cd22-136">setting</span><span class="sxs-lookup"><span data-stu-id="9cd22-136">setting</span></span>|<span data-ttu-id="9cd22-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cd22-137">String</span></span>|<span data-ttu-id="9cd22-138">Klassenname und Eigenschaftenname der Einstellung</span><span class="sxs-lookup"><span data-stu-id="9cd22-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="9cd22-139">settingName</span><span class="sxs-lookup"><span data-stu-id="9cd22-139">settingName</span></span>|<span data-ttu-id="9cd22-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cd22-140">String</span></span>|<span data-ttu-id="9cd22-141">Name der Einstellung</span><span class="sxs-lookup"><span data-stu-id="9cd22-141">Name of the setting.</span></span>|
|<span data-ttu-id="9cd22-142">platformType</span><span class="sxs-lookup"><span data-stu-id="9cd22-142">platformType</span></span>|[<span data-ttu-id="9cd22-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9cd22-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="9cd22-144">Einstellung-Plattform.</span><span class="sxs-lookup"><span data-stu-id="9cd22-144">Setting platform.</span></span> <span data-ttu-id="9cd22-145">Mögliche Werte: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="9cd22-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="9cd22-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-146">unknownDeviceCount</span></span>|<span data-ttu-id="9cd22-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-147">Int32</span></span>|<span data-ttu-id="9cd22-148">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="9cd22-148">Number of unknown devices</span></span>|
|<span data-ttu-id="9cd22-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="9cd22-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-150">Int32</span></span>|<span data-ttu-id="9cd22-151">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="9cd22-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="9cd22-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-152">compliantDeviceCount</span></span>|<span data-ttu-id="9cd22-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-153">Int32</span></span>|<span data-ttu-id="9cd22-154">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="9cd22-154">Number of compliant devices</span></span>|
|<span data-ttu-id="9cd22-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-155">remediatedDeviceCount</span></span>|<span data-ttu-id="9cd22-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-156">Int32</span></span>|<span data-ttu-id="9cd22-157">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="9cd22-157">Number of remediated devices</span></span>|
|<span data-ttu-id="9cd22-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9cd22-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-159">Int32</span></span>|<span data-ttu-id="9cd22-160">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="9cd22-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="9cd22-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-161">errorDeviceCount</span></span>|<span data-ttu-id="9cd22-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-162">Int32</span></span>|<span data-ttu-id="9cd22-163">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="9cd22-163">Number of error devices</span></span>|
|<span data-ttu-id="9cd22-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9cd22-164">conflictDeviceCount</span></span>|<span data-ttu-id="9cd22-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9cd22-165">Int32</span></span>|<span data-ttu-id="9cd22-166">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="9cd22-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="9cd22-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cd22-167">Response</span></span>
<span data-ttu-id="9cd22-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9cd22-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cd22-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cd22-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cd22-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cd22-170">Request</span></span>
<span data-ttu-id="9cd22-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cd22-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9cd22-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cd22-172">Response</span></span>
<span data-ttu-id="9cd22-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cd22-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





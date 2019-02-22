---
title: AdvancedThreatProtectionOnboardingStateSummary aktualisieren
description: Aktualisieren der Eigenschaften eines advancedThreatProtectionOnboardingStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94d146bc9696e02e824af02732b6e22b70533535
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144856"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="6b5e0-103">AdvancedThreatProtectionOnboardingStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6b5e0-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="6b5e0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b5e0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b5e0-106">Aktualisieren der Eigenschaften eines [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b5e0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b5e0-107">Prerequisites</span></span>
<span data-ttu-id="6b5e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b5e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b5e0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b5e0-110">Permission type</span></span>|<span data-ttu-id="6b5e0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b5e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b5e0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b5e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b5e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b5e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b5e0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b5e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b5e0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b5e0-115">Not supported.</span></span>|
|<span data-ttu-id="6b5e0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b5e0-116">Application</span></span>|<span data-ttu-id="6b5e0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b5e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b5e0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b5e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="6b5e0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b5e0-119">Request headers</span></span>
|<span data-ttu-id="6b5e0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6b5e0-120">Header</span></span>|<span data-ttu-id="6b5e0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6b5e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b5e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b5e0-122">Authorization</span></span>|<span data-ttu-id="6b5e0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b5e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b5e0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6b5e0-124">Accept</span></span>|<span data-ttu-id="6b5e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b5e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b5e0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b5e0-126">Request body</span></span>
<span data-ttu-id="6b5e0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="6b5e0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="6b5e0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6b5e0-129">Property</span></span>|<span data-ttu-id="6b5e0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6b5e0-130">Type</span></span>|<span data-ttu-id="6b5e0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b5e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b5e0-132">id</span><span class="sxs-lookup"><span data-stu-id="6b5e0-132">id</span></span>|<span data-ttu-id="6b5e0-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b5e0-133">String</span></span>|<span data-ttu-id="6b5e0-134">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="6b5e0-134">Unique Identifier</span></span>|
|<span data-ttu-id="6b5e0-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-135">unknownDeviceCount</span></span>|<span data-ttu-id="6b5e0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-136">Int32</span></span>|<span data-ttu-id="6b5e0-137">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="6b5e0-137">Number of unknown devices</span></span>|
|<span data-ttu-id="6b5e0-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="6b5e0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-139">Int32</span></span>|<span data-ttu-id="6b5e0-140">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="6b5e0-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="6b5e0-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-141">compliantDeviceCount</span></span>|<span data-ttu-id="6b5e0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-142">Int32</span></span>|<span data-ttu-id="6b5e0-143">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="6b5e0-143">Number of compliant devices</span></span>|
|<span data-ttu-id="6b5e0-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-144">remediatedDeviceCount</span></span>|<span data-ttu-id="6b5e0-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-145">Int32</span></span>|<span data-ttu-id="6b5e0-146">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="6b5e0-146">Number of remediated devices</span></span>|
|<span data-ttu-id="6b5e0-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6b5e0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-148">Int32</span></span>|<span data-ttu-id="6b5e0-149">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="6b5e0-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="6b5e0-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-150">errorDeviceCount</span></span>|<span data-ttu-id="6b5e0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-151">Int32</span></span>|<span data-ttu-id="6b5e0-152">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="6b5e0-152">Number of error devices</span></span>|
|<span data-ttu-id="6b5e0-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-153">conflictDeviceCount</span></span>|<span data-ttu-id="6b5e0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-154">Int32</span></span>|<span data-ttu-id="6b5e0-155">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="6b5e0-155">Number of conflict devices</span></span>|
|<span data-ttu-id="6b5e0-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b5e0-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="6b5e0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6b5e0-157">Int32</span></span>|<span data-ttu-id="6b5e0-158">Anzahl der nicht zugewiesenen Geräte</span><span class="sxs-lookup"><span data-stu-id="6b5e0-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="6b5e0-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b5e0-159">Response</span></span>
<span data-ttu-id="6b5e0-160">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b5e0-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b5e0-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b5e0-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b5e0-162">Request</span></span>
<span data-ttu-id="6b5e0-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="6b5e0-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b5e0-164">Response</span></span>
<span data-ttu-id="6b5e0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b5e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```





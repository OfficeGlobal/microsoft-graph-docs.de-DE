---
title: AdvancedThreatProtectionOnboardingStateSummary aktualisieren
description: Aktualisieren der Eigenschaften eines advancedThreatProtectionOnboardingStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ca5bb4fe9ef9fe0b5ac67e2d4569713fef2ea6d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964213"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="2a9ab-103">AdvancedThreatProtectionOnboardingStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a9ab-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="2a9ab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a9ab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a9ab-106">Aktualisieren der Eigenschaften eines [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a9ab-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a9ab-107">Prerequisites</span></span>
<span data-ttu-id="2a9ab-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a9ab-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a9ab-110">Permission type</span></span>|<span data-ttu-id="2a9ab-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a9ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a9ab-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a9ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a9ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a9ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a9ab-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a9ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a9ab-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a9ab-115">Not supported.</span></span>|
|<span data-ttu-id="2a9ab-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a9ab-116">Application</span></span>|<span data-ttu-id="2a9ab-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a9ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a9ab-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a9ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2a9ab-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a9ab-119">Request headers</span></span>
|<span data-ttu-id="2a9ab-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a9ab-120">Header</span></span>|<span data-ttu-id="2a9ab-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2a9ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a9ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a9ab-122">Authorization</span></span>|<span data-ttu-id="2a9ab-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a9ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a9ab-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a9ab-124">Accept</span></span>|<span data-ttu-id="2a9ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a9ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a9ab-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a9ab-126">Request body</span></span>
<span data-ttu-id="2a9ab-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="2a9ab-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="2a9ab-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a9ab-129">Property</span></span>|<span data-ttu-id="2a9ab-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2a9ab-130">Type</span></span>|<span data-ttu-id="2a9ab-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a9ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a9ab-132">id</span><span class="sxs-lookup"><span data-stu-id="2a9ab-132">id</span></span>|<span data-ttu-id="2a9ab-133">String</span><span class="sxs-lookup"><span data-stu-id="2a9ab-133">String</span></span>|<span data-ttu-id="2a9ab-134">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="2a9ab-134">Unique Identifier</span></span>|
|<span data-ttu-id="2a9ab-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-135">unknownDeviceCount</span></span>|<span data-ttu-id="2a9ab-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-136">Int32</span></span>|<span data-ttu-id="2a9ab-137">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-137">Number of unknown devices</span></span>|
|<span data-ttu-id="2a9ab-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="2a9ab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-139">Int32</span></span>|<span data-ttu-id="2a9ab-140">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="2a9ab-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-141">compliantDeviceCount</span></span>|<span data-ttu-id="2a9ab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-142">Int32</span></span>|<span data-ttu-id="2a9ab-143">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-143">Number of compliant devices</span></span>|
|<span data-ttu-id="2a9ab-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-144">remediatedDeviceCount</span></span>|<span data-ttu-id="2a9ab-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-145">Int32</span></span>|<span data-ttu-id="2a9ab-146">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-146">Number of remediated devices</span></span>|
|<span data-ttu-id="2a9ab-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2a9ab-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-148">Int32</span></span>|<span data-ttu-id="2a9ab-149">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="2a9ab-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-150">errorDeviceCount</span></span>|<span data-ttu-id="2a9ab-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-151">Int32</span></span>|<span data-ttu-id="2a9ab-152">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-152">Number of error devices</span></span>|
|<span data-ttu-id="2a9ab-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-153">conflictDeviceCount</span></span>|<span data-ttu-id="2a9ab-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-154">Int32</span></span>|<span data-ttu-id="2a9ab-155">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="2a9ab-155">Number of conflict devices</span></span>|
|<span data-ttu-id="2a9ab-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a9ab-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="2a9ab-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2a9ab-157">Int32</span></span>|<span data-ttu-id="2a9ab-158">Anzahl der nicht zugewiesenen Geräte</span><span class="sxs-lookup"><span data-stu-id="2a9ab-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="2a9ab-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a9ab-159">Response</span></span>
<span data-ttu-id="2a9ab-160">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a9ab-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a9ab-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a9ab-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a9ab-162">Request</span></span>
<span data-ttu-id="2a9ab-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a9ab-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a9ab-164">Response</span></span>
<span data-ttu-id="2a9ab-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a9ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





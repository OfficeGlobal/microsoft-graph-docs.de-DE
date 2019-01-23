---
title: AdvancedThreatProtectionOnboardingStateSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AdvancedThreatProtectionOnboardingStateSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9a94e5b0abee3d369148c2301942a1196ef9010c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409279"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="28e22-103">AdvancedThreatProtectionOnboardingStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28e22-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="28e22-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="28e22-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28e22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28e22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28e22-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28e22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e22-107">Aktualisieren Sie die Eigenschaften eines [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="28e22-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28e22-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28e22-108">Prerequisites</span></span>
<span data-ttu-id="28e22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="28e22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28e22-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28e22-111">Permission type</span></span>|<span data-ttu-id="28e22-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28e22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28e22-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28e22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28e22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28e22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28e22-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28e22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28e22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28e22-116">Not supported.</span></span>|
|<span data-ttu-id="28e22-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28e22-117">Application</span></span>|<span data-ttu-id="28e22-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28e22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28e22-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28e22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="28e22-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28e22-120">Request headers</span></span>
|<span data-ttu-id="28e22-121">Header</span><span class="sxs-lookup"><span data-stu-id="28e22-121">Header</span></span>|<span data-ttu-id="28e22-122">Wert</span><span class="sxs-lookup"><span data-stu-id="28e22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28e22-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="28e22-123">Authorization</span></span>|<span data-ttu-id="28e22-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28e22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28e22-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28e22-125">Accept</span></span>|<span data-ttu-id="28e22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28e22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e22-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28e22-127">Request body</span></span>
<span data-ttu-id="28e22-128">Geben Sie im Textkörper Anforderung für das Objekt [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="28e22-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="28e22-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="28e22-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="28e22-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28e22-130">Property</span></span>|<span data-ttu-id="28e22-131">Typ</span><span class="sxs-lookup"><span data-stu-id="28e22-131">Type</span></span>|<span data-ttu-id="28e22-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28e22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e22-133">id</span><span class="sxs-lookup"><span data-stu-id="28e22-133">id</span></span>|<span data-ttu-id="28e22-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28e22-134">String</span></span>|<span data-ttu-id="28e22-135">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="28e22-135">Unique Identifier</span></span>|
|<span data-ttu-id="28e22-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-136">unknownDeviceCount</span></span>|<span data-ttu-id="28e22-137">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-137">Int32</span></span>|<span data-ttu-id="28e22-138">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="28e22-138">Number of unknown devices</span></span>|
|<span data-ttu-id="28e22-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="28e22-140">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-140">Int32</span></span>|<span data-ttu-id="28e22-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="28e22-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="28e22-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-142">compliantDeviceCount</span></span>|<span data-ttu-id="28e22-143">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-143">Int32</span></span>|<span data-ttu-id="28e22-144">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="28e22-144">Number of compliant devices</span></span>|
|<span data-ttu-id="28e22-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-145">remediatedDeviceCount</span></span>|<span data-ttu-id="28e22-146">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-146">Int32</span></span>|<span data-ttu-id="28e22-147">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="28e22-147">Number of remediated devices</span></span>|
|<span data-ttu-id="28e22-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="28e22-149">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-149">Int32</span></span>|<span data-ttu-id="28e22-150">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="28e22-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="28e22-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-151">errorDeviceCount</span></span>|<span data-ttu-id="28e22-152">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-152">Int32</span></span>|<span data-ttu-id="28e22-153">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="28e22-153">Number of error devices</span></span>|
|<span data-ttu-id="28e22-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-154">conflictDeviceCount</span></span>|<span data-ttu-id="28e22-155">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-155">Int32</span></span>|<span data-ttu-id="28e22-156">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="28e22-156">Number of conflict devices</span></span>|
|<span data-ttu-id="28e22-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="28e22-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="28e22-158">Int32</span><span class="sxs-lookup"><span data-stu-id="28e22-158">Int32</span></span>|<span data-ttu-id="28e22-159">Anzahl der nicht zugewiesenen Geräte</span><span class="sxs-lookup"><span data-stu-id="28e22-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="28e22-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="28e22-160">Response</span></span>
<span data-ttu-id="28e22-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="28e22-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e22-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28e22-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="28e22-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28e22-163">Request</span></span>
<span data-ttu-id="28e22-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28e22-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28e22-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="28e22-165">Response</span></span>
<span data-ttu-id="28e22-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28e22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





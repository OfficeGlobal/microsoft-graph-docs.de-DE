---
title: AdvancedThreatProtectionOnboardingStateSummary aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AdvancedThreatProtectionOnboardingStateSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 67d127ae3fb4545857dca2719fd2ae8417a400fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837069"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="56e37-103">AdvancedThreatProtectionOnboardingStateSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56e37-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="56e37-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56e37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56e37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56e37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56e37-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56e37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56e37-107">Aktualisieren Sie die Eigenschaften eines [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="56e37-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56e37-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56e37-108">Prerequisites</span></span>
<span data-ttu-id="56e37-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56e37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e37-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56e37-111">Permission type</span></span>|<span data-ttu-id="56e37-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56e37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56e37-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56e37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56e37-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56e37-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56e37-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56e37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56e37-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56e37-116">Not supported.</span></span>|
|<span data-ttu-id="56e37-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56e37-117">Application</span></span>|<span data-ttu-id="56e37-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56e37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56e37-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56e37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="56e37-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56e37-120">Request headers</span></span>
|<span data-ttu-id="56e37-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56e37-121">Header</span></span>|<span data-ttu-id="56e37-122">Wert</span><span class="sxs-lookup"><span data-stu-id="56e37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56e37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56e37-123">Authorization</span></span>|<span data-ttu-id="56e37-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56e37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56e37-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56e37-125">Accept</span></span>|<span data-ttu-id="56e37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56e37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e37-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56e37-127">Request body</span></span>
<span data-ttu-id="56e37-128">Geben Sie im Textkörper Anforderung für das Objekt [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="56e37-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="56e37-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="56e37-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="56e37-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56e37-130">Property</span></span>|<span data-ttu-id="56e37-131">Typ</span><span class="sxs-lookup"><span data-stu-id="56e37-131">Type</span></span>|<span data-ttu-id="56e37-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56e37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e37-133">id</span><span class="sxs-lookup"><span data-stu-id="56e37-133">id</span></span>|<span data-ttu-id="56e37-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56e37-134">String</span></span>|<span data-ttu-id="56e37-135">Eindeutiger Bezeichner</span><span class="sxs-lookup"><span data-stu-id="56e37-135">Unique Identifier</span></span>|
|<span data-ttu-id="56e37-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-136">unknownDeviceCount</span></span>|<span data-ttu-id="56e37-137">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-137">Int32</span></span>|<span data-ttu-id="56e37-138">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="56e37-138">Number of unknown devices</span></span>|
|<span data-ttu-id="56e37-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="56e37-140">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-140">Int32</span></span>|<span data-ttu-id="56e37-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="56e37-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="56e37-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-142">compliantDeviceCount</span></span>|<span data-ttu-id="56e37-143">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-143">Int32</span></span>|<span data-ttu-id="56e37-144">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="56e37-144">Number of compliant devices</span></span>|
|<span data-ttu-id="56e37-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-145">remediatedDeviceCount</span></span>|<span data-ttu-id="56e37-146">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-146">Int32</span></span>|<span data-ttu-id="56e37-147">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="56e37-147">Number of remediated devices</span></span>|
|<span data-ttu-id="56e37-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="56e37-149">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-149">Int32</span></span>|<span data-ttu-id="56e37-150">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="56e37-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="56e37-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-151">errorDeviceCount</span></span>|<span data-ttu-id="56e37-152">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-152">Int32</span></span>|<span data-ttu-id="56e37-153">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="56e37-153">Number of error devices</span></span>|
|<span data-ttu-id="56e37-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-154">conflictDeviceCount</span></span>|<span data-ttu-id="56e37-155">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-155">Int32</span></span>|<span data-ttu-id="56e37-156">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="56e37-156">Number of conflict devices</span></span>|
|<span data-ttu-id="56e37-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56e37-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="56e37-158">Int32</span><span class="sxs-lookup"><span data-stu-id="56e37-158">Int32</span></span>|<span data-ttu-id="56e37-159">Anzahl der nicht zugewiesenen Geräte</span><span class="sxs-lookup"><span data-stu-id="56e37-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="56e37-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="56e37-160">Response</span></span>
<span data-ttu-id="56e37-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="56e37-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e37-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56e37-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="56e37-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56e37-163">Request</span></span>
<span data-ttu-id="56e37-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56e37-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 246

{
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

### <a name="response"></a><span data-ttu-id="56e37-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="56e37-165">Response</span></span>
<span data-ttu-id="56e37-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56e37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






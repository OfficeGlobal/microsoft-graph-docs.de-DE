---
title: deviceEnrollmentPlatformRestrictionsConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
ms.openlocfilehash: e28bea6cc182684ec10abddf97801772c111bf0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060516"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="11374-103">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="11374-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="11374-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11374-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11374-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11374-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11374-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11374-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11374-107">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11374-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11374-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11374-108">Prerequisites</span></span>
<span data-ttu-id="11374-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11374-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11374-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11374-111">Permission type</span></span>|<span data-ttu-id="11374-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11374-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11374-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11374-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11374-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11374-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11374-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11374-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11374-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11374-116">Not supported.</span></span>|
|<span data-ttu-id="11374-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11374-117">Application</span></span>|<span data-ttu-id="11374-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11374-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11374-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11374-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="11374-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11374-120">Request headers</span></span>
|<span data-ttu-id="11374-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="11374-121">Header</span></span>|<span data-ttu-id="11374-122">Wert</span><span class="sxs-lookup"><span data-stu-id="11374-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11374-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11374-123">Authorization</span></span>|<span data-ttu-id="11374-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11374-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11374-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11374-125">Accept</span></span>|<span data-ttu-id="11374-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11374-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11374-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11374-127">Request body</span></span>
<span data-ttu-id="11374-128">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="11374-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="11374-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="11374-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="11374-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11374-130">Property</span></span>|<span data-ttu-id="11374-131">Typ</span><span class="sxs-lookup"><span data-stu-id="11374-131">Type</span></span>|<span data-ttu-id="11374-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11374-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11374-133">id</span><span class="sxs-lookup"><span data-stu-id="11374-133">id</span></span>|<span data-ttu-id="11374-134">String</span><span class="sxs-lookup"><span data-stu-id="11374-134">String</span></span>|<span data-ttu-id="11374-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11374-136">displayName</span></span>|<span data-ttu-id="11374-137">String</span><span class="sxs-lookup"><span data-stu-id="11374-137">String</span></span>|<span data-ttu-id="11374-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-139">description</span><span class="sxs-lookup"><span data-stu-id="11374-139">description</span></span>|<span data-ttu-id="11374-140">String</span><span class="sxs-lookup"><span data-stu-id="11374-140">String</span></span>|<span data-ttu-id="11374-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="11374-142">priority</span></span>|<span data-ttu-id="11374-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11374-143">Int32</span></span>|<span data-ttu-id="11374-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11374-145">createdDateTime</span></span>|<span data-ttu-id="11374-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11374-146">DateTimeOffset</span></span>|<span data-ttu-id="11374-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11374-148">lastModifiedDateTime</span></span>|<span data-ttu-id="11374-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11374-149">DateTimeOffset</span></span>|<span data-ttu-id="11374-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-151">Version</span><span class="sxs-lookup"><span data-stu-id="11374-151">version</span></span>|<span data-ttu-id="11374-152">Int32</span><span class="sxs-lookup"><span data-stu-id="11374-152">Int32</span></span>|<span data-ttu-id="11374-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11374-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11374-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-154">iosRestriction</span></span>|[<span data-ttu-id="11374-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-156">Not yet documented</span></span>|
|<span data-ttu-id="11374-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-157">windowsRestriction</span></span>|[<span data-ttu-id="11374-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-159">Not yet documented</span></span>|
|<span data-ttu-id="11374-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="11374-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-162">Not yet documented</span></span>|
|<span data-ttu-id="11374-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-163">androidRestriction</span></span>|[<span data-ttu-id="11374-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-165">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-165">Not yet documented</span></span>|
|<span data-ttu-id="11374-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="11374-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-168">Not yet documented</span></span>|
|<span data-ttu-id="11374-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-169">macRestriction</span></span>|[<span data-ttu-id="11374-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-171">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-171">Not yet documented</span></span>|
|<span data-ttu-id="11374-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-172">macOSRestriction</span></span>|[<span data-ttu-id="11374-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11374-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11374-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="11374-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="11374-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="11374-175">Response</span></span>
<span data-ttu-id="11374-176">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="11374-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11374-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11374-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="11374-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11374-178">Request</span></span>
<span data-ttu-id="11374-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11374-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 2295

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="11374-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="11374-180">Response</span></span>
<span data-ttu-id="11374-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11374-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2403

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```






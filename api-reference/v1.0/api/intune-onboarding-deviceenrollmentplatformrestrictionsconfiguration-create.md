---
title: deviceEnrollmentPlatformRestrictionsConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28a59aad2d47c87a2a8eafc25d3def37b60fee92
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874606"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="e1238-103">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="e1238-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="e1238-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1238-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1238-105">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1238-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1238-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1238-106">Prerequisites</span></span>
<span data-ttu-id="e1238-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1238-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1238-109">Permission type</span></span>|<span data-ttu-id="e1238-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1238-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1238-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1238-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1238-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1238-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1238-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1238-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1238-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1238-114">Not supported.</span></span>|
|<span data-ttu-id="e1238-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1238-115">Application</span></span>|<span data-ttu-id="e1238-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1238-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1238-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1238-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1238-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1238-118">Request headers</span></span>
|<span data-ttu-id="e1238-119">Header</span><span class="sxs-lookup"><span data-stu-id="e1238-119">Header</span></span>|<span data-ttu-id="e1238-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e1238-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1238-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1238-121">Authorization</span></span>|<span data-ttu-id="e1238-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1238-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1238-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1238-123">Accept</span></span>|<span data-ttu-id="e1238-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1238-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1238-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1238-125">Request body</span></span>
<span data-ttu-id="e1238-126">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e1238-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="e1238-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e1238-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="e1238-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1238-128">Property</span></span>|<span data-ttu-id="e1238-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e1238-129">Type</span></span>|<span data-ttu-id="e1238-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1238-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1238-131">id</span><span class="sxs-lookup"><span data-stu-id="e1238-131">id</span></span>|<span data-ttu-id="e1238-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1238-132">String</span></span>|<span data-ttu-id="e1238-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e1238-134">displayName</span></span>|<span data-ttu-id="e1238-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1238-135">String</span></span>|<span data-ttu-id="e1238-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-137">description</span><span class="sxs-lookup"><span data-stu-id="e1238-137">description</span></span>|<span data-ttu-id="e1238-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1238-138">String</span></span>|<span data-ttu-id="e1238-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="e1238-140">priority</span></span>|<span data-ttu-id="e1238-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e1238-141">Int32</span></span>|<span data-ttu-id="e1238-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1238-143">createdDateTime</span></span>|<span data-ttu-id="e1238-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1238-144">DateTimeOffset</span></span>|<span data-ttu-id="e1238-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1238-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e1238-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1238-147">DateTimeOffset</span></span>|<span data-ttu-id="e1238-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-149">Version</span><span class="sxs-lookup"><span data-stu-id="e1238-149">version</span></span>|<span data-ttu-id="e1238-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e1238-150">Int32</span></span>|<span data-ttu-id="e1238-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1238-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="e1238-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-152">iosRestriction</span></span>|[<span data-ttu-id="e1238-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e1238-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1238-154">Not yet documented</span></span>|
|<span data-ttu-id="e1238-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-155">windowsRestriction</span></span>|[<span data-ttu-id="e1238-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e1238-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1238-157">Not yet documented</span></span>|
|<span data-ttu-id="e1238-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="e1238-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e1238-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1238-160">Not yet documented</span></span>|
|<span data-ttu-id="e1238-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-161">androidRestriction</span></span>|[<span data-ttu-id="e1238-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e1238-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1238-163">Not yet documented</span></span>|
|<span data-ttu-id="e1238-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-164">macOSRestriction</span></span>|[<span data-ttu-id="e1238-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e1238-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="e1238-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e1238-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e1238-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1238-167">Response</span></span>
<span data-ttu-id="e1238-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e1238-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1238-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1238-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1238-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1238-170">Request</span></span>
<span data-ttu-id="e1238-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1238-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1650

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="e1238-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1238-172">Response</span></span>
<span data-ttu-id="e1238-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1238-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1822

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
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




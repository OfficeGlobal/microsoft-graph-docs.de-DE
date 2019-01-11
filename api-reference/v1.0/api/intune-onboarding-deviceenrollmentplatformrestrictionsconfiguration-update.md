---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3794933b6dabbc9f6a6bfc4957ff0e9a795c3f80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849469"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="264fc-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="264fc-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="264fc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="264fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="264fc-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="264fc-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="264fc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="264fc-106">Prerequisites</span></span>
<span data-ttu-id="264fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="264fc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="264fc-109">Permission type</span></span>|<span data-ttu-id="264fc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="264fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264fc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="264fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="264fc-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264fc-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="264fc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="264fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264fc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="264fc-114">Not supported.</span></span>|
|<span data-ttu-id="264fc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="264fc-115">Application</span></span>|<span data-ttu-id="264fc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="264fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="264fc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="264fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="264fc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="264fc-118">Request headers</span></span>
|<span data-ttu-id="264fc-119">Header</span><span class="sxs-lookup"><span data-stu-id="264fc-119">Header</span></span>|<span data-ttu-id="264fc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="264fc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="264fc-121">Authorization</span></span>|<span data-ttu-id="264fc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="264fc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264fc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="264fc-123">Accept</span></span>|<span data-ttu-id="264fc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="264fc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264fc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="264fc-125">Request body</span></span>
<span data-ttu-id="264fc-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="264fc-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="264fc-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="264fc-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="264fc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="264fc-128">Property</span></span>|<span data-ttu-id="264fc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="264fc-129">Type</span></span>|<span data-ttu-id="264fc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="264fc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="264fc-131">id</span><span class="sxs-lookup"><span data-stu-id="264fc-131">id</span></span>|<span data-ttu-id="264fc-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="264fc-132">String</span></span>|<span data-ttu-id="264fc-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="264fc-134">displayName</span></span>|<span data-ttu-id="264fc-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="264fc-135">String</span></span>|<span data-ttu-id="264fc-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-137">description</span><span class="sxs-lookup"><span data-stu-id="264fc-137">description</span></span>|<span data-ttu-id="264fc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="264fc-138">String</span></span>|<span data-ttu-id="264fc-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="264fc-140">priority</span></span>|<span data-ttu-id="264fc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="264fc-141">Int32</span></span>|<span data-ttu-id="264fc-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="264fc-143">createdDateTime</span></span>|<span data-ttu-id="264fc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264fc-144">DateTimeOffset</span></span>|<span data-ttu-id="264fc-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="264fc-146">lastModifiedDateTime</span></span>|<span data-ttu-id="264fc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264fc-147">DateTimeOffset</span></span>|<span data-ttu-id="264fc-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-149">Version</span><span class="sxs-lookup"><span data-stu-id="264fc-149">version</span></span>|<span data-ttu-id="264fc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="264fc-150">Int32</span></span>|<span data-ttu-id="264fc-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="264fc-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="264fc-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-152">iosRestriction</span></span>|[<span data-ttu-id="264fc-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="264fc-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="264fc-154">Not yet documented</span></span>|
|<span data-ttu-id="264fc-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-155">windowsRestriction</span></span>|[<span data-ttu-id="264fc-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="264fc-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="264fc-157">Not yet documented</span></span>|
|<span data-ttu-id="264fc-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="264fc-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="264fc-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="264fc-160">Not yet documented</span></span>|
|<span data-ttu-id="264fc-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-161">androidRestriction</span></span>|[<span data-ttu-id="264fc-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="264fc-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="264fc-163">Not yet documented</span></span>|
|<span data-ttu-id="264fc-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-164">macOSRestriction</span></span>|[<span data-ttu-id="264fc-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="264fc-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="264fc-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="264fc-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="264fc-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="264fc-167">Response</span></span>
<span data-ttu-id="264fc-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="264fc-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264fc-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="264fc-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="264fc-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="264fc-170">Request</span></span>
<span data-ttu-id="264fc-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="264fc-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="264fc-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="264fc-172">Response</span></span>
<span data-ttu-id="264fc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="264fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




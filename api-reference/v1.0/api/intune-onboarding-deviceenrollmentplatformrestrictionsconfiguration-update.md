---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: dc7ac904df5ae18b0476cfeeb2d1c98a6533a7c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308204"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="5830c-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5830c-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="5830c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5830c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5830c-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5830c-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5830c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5830c-106">Prerequisites</span></span>
<span data-ttu-id="5830c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5830c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5830c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5830c-109">Permission type</span></span>|<span data-ttu-id="5830c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5830c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5830c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5830c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5830c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5830c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5830c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5830c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5830c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5830c-114">Not supported.</span></span>|
|<span data-ttu-id="5830c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5830c-115">Application</span></span>|<span data-ttu-id="5830c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5830c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5830c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5830c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5830c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5830c-118">Request headers</span></span>
|<span data-ttu-id="5830c-119">Header</span><span class="sxs-lookup"><span data-stu-id="5830c-119">Header</span></span>|<span data-ttu-id="5830c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5830c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5830c-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5830c-121">Authorization</span></span>|<span data-ttu-id="5830c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5830c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5830c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5830c-123">Accept</span></span>|<span data-ttu-id="5830c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5830c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5830c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5830c-125">Request body</span></span>
<span data-ttu-id="5830c-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5830c-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="5830c-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5830c-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="5830c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5830c-128">Property</span></span>|<span data-ttu-id="5830c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5830c-129">Type</span></span>|<span data-ttu-id="5830c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5830c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5830c-131">id</span><span class="sxs-lookup"><span data-stu-id="5830c-131">id</span></span>|<span data-ttu-id="5830c-132">String</span><span class="sxs-lookup"><span data-stu-id="5830c-132">String</span></span>|<span data-ttu-id="5830c-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5830c-134">displayName</span></span>|<span data-ttu-id="5830c-135">String</span><span class="sxs-lookup"><span data-stu-id="5830c-135">String</span></span>|<span data-ttu-id="5830c-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-137">description</span><span class="sxs-lookup"><span data-stu-id="5830c-137">description</span></span>|<span data-ttu-id="5830c-138">String</span><span class="sxs-lookup"><span data-stu-id="5830c-138">String</span></span>|<span data-ttu-id="5830c-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="5830c-140">priority</span></span>|<span data-ttu-id="5830c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5830c-141">Int32</span></span>|<span data-ttu-id="5830c-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5830c-143">createdDateTime</span></span>|<span data-ttu-id="5830c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5830c-144">DateTimeOffset</span></span>|<span data-ttu-id="5830c-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5830c-146">lastModifiedDateTime</span></span>|<span data-ttu-id="5830c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5830c-147">DateTimeOffset</span></span>|<span data-ttu-id="5830c-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-149">Version</span><span class="sxs-lookup"><span data-stu-id="5830c-149">version</span></span>|<span data-ttu-id="5830c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5830c-150">Int32</span></span>|<span data-ttu-id="5830c-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5830c-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5830c-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-152">iosRestriction</span></span>|[<span data-ttu-id="5830c-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5830c-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5830c-154">Not yet documented</span></span>|
|<span data-ttu-id="5830c-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-155">windowsRestriction</span></span>|[<span data-ttu-id="5830c-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5830c-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5830c-157">Not yet documented</span></span>|
|<span data-ttu-id="5830c-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="5830c-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5830c-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5830c-160">Not yet documented</span></span>|
|<span data-ttu-id="5830c-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-161">androidRestriction</span></span>|[<span data-ttu-id="5830c-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5830c-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5830c-163">Not yet documented</span></span>|
|<span data-ttu-id="5830c-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-164">macOSRestriction</span></span>|[<span data-ttu-id="5830c-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="5830c-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="5830c-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="5830c-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5830c-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="5830c-167">Response</span></span>
<span data-ttu-id="5830c-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5830c-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5830c-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5830c-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="5830c-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5830c-170">Request</span></span>
<span data-ttu-id="5830c-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5830c-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5830c-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="5830c-172">Response</span></span>
<span data-ttu-id="5830c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5830c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




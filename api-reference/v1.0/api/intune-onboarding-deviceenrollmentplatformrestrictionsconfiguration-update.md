---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e1e8235bd6c98abaee64960bf29e12b0226bd479
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982498"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="1edde-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1edde-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="1edde-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1edde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1edde-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1edde-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1edde-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1edde-106">Prerequisites</span></span>
<span data-ttu-id="1edde-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1edde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1edde-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1edde-109">Permission type</span></span>|<span data-ttu-id="1edde-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1edde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1edde-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1edde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1edde-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1edde-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1edde-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1edde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1edde-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1edde-114">Not supported.</span></span>|
|<span data-ttu-id="1edde-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1edde-115">Application</span></span>|<span data-ttu-id="1edde-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1edde-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1edde-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1edde-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1edde-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1edde-118">Request headers</span></span>
|<span data-ttu-id="1edde-119">Header</span><span class="sxs-lookup"><span data-stu-id="1edde-119">Header</span></span>|<span data-ttu-id="1edde-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1edde-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1edde-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1edde-121">Authorization</span></span>|<span data-ttu-id="1edde-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1edde-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1edde-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1edde-123">Accept</span></span>|<span data-ttu-id="1edde-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1edde-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1edde-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1edde-125">Request body</span></span>
<span data-ttu-id="1edde-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1edde-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="1edde-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1edde-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="1edde-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1edde-128">Property</span></span>|<span data-ttu-id="1edde-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1edde-129">Type</span></span>|<span data-ttu-id="1edde-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1edde-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1edde-131">id</span><span class="sxs-lookup"><span data-stu-id="1edde-131">id</span></span>|<span data-ttu-id="1edde-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1edde-132">String</span></span>|<span data-ttu-id="1edde-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1edde-134">displayName</span></span>|<span data-ttu-id="1edde-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1edde-135">String</span></span>|<span data-ttu-id="1edde-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-137">description</span><span class="sxs-lookup"><span data-stu-id="1edde-137">description</span></span>|<span data-ttu-id="1edde-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1edde-138">String</span></span>|<span data-ttu-id="1edde-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="1edde-140">priority</span></span>|<span data-ttu-id="1edde-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1edde-141">Int32</span></span>|<span data-ttu-id="1edde-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1edde-143">createdDateTime</span></span>|<span data-ttu-id="1edde-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1edde-144">DateTimeOffset</span></span>|<span data-ttu-id="1edde-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1edde-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1edde-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1edde-147">DateTimeOffset</span></span>|<span data-ttu-id="1edde-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-149">Version</span><span class="sxs-lookup"><span data-stu-id="1edde-149">version</span></span>|<span data-ttu-id="1edde-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1edde-150">Int32</span></span>|<span data-ttu-id="1edde-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1edde-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1edde-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-152">iosRestriction</span></span>|[<span data-ttu-id="1edde-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1edde-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1edde-154">Not yet documented</span></span>|
|<span data-ttu-id="1edde-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-155">windowsRestriction</span></span>|[<span data-ttu-id="1edde-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1edde-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1edde-157">Not yet documented</span></span>|
|<span data-ttu-id="1edde-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="1edde-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1edde-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1edde-160">Not yet documented</span></span>|
|<span data-ttu-id="1edde-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-161">androidRestriction</span></span>|[<span data-ttu-id="1edde-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1edde-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1edde-163">Not yet documented</span></span>|
|<span data-ttu-id="1edde-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-164">macOSRestriction</span></span>|[<span data-ttu-id="1edde-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1edde-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="1edde-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1edde-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1edde-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="1edde-167">Response</span></span>
<span data-ttu-id="1edde-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1edde-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1edde-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1edde-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="1edde-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1edde-170">Request</span></span>
<span data-ttu-id="1edde-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1edde-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1edde-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="1edde-172">Response</span></span>
<span data-ttu-id="1edde-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1edde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




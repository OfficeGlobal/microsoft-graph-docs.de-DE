---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 970462a8f993e8ef01f5c1359e865b625bfec611
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402300"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="28355-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28355-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="28355-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="28355-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28355-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28355-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28355-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28355-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28355-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28355-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28355-108">Prerequisites</span></span>
<span data-ttu-id="28355-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="28355-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28355-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28355-111">Permission type</span></span>|<span data-ttu-id="28355-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28355-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28355-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28355-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28355-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28355-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28355-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28355-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28355-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28355-116">Not supported.</span></span>|
|<span data-ttu-id="28355-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28355-117">Application</span></span>|<span data-ttu-id="28355-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28355-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28355-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28355-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="28355-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28355-120">Request headers</span></span>
|<span data-ttu-id="28355-121">Header</span><span class="sxs-lookup"><span data-stu-id="28355-121">Header</span></span>|<span data-ttu-id="28355-122">Wert</span><span class="sxs-lookup"><span data-stu-id="28355-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28355-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="28355-123">Authorization</span></span>|<span data-ttu-id="28355-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28355-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28355-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28355-125">Accept</span></span>|<span data-ttu-id="28355-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28355-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28355-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28355-127">Request body</span></span>
<span data-ttu-id="28355-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="28355-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="28355-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="28355-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="28355-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28355-130">Property</span></span>|<span data-ttu-id="28355-131">Typ</span><span class="sxs-lookup"><span data-stu-id="28355-131">Type</span></span>|<span data-ttu-id="28355-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28355-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28355-133">id</span><span class="sxs-lookup"><span data-stu-id="28355-133">id</span></span>|<span data-ttu-id="28355-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28355-134">String</span></span>|<span data-ttu-id="28355-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-136">displayName</span><span class="sxs-lookup"><span data-stu-id="28355-136">displayName</span></span>|<span data-ttu-id="28355-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28355-137">String</span></span>|<span data-ttu-id="28355-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-139">description</span><span class="sxs-lookup"><span data-stu-id="28355-139">description</span></span>|<span data-ttu-id="28355-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28355-140">String</span></span>|<span data-ttu-id="28355-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="28355-142">priority</span></span>|<span data-ttu-id="28355-143">Int32</span><span class="sxs-lookup"><span data-stu-id="28355-143">Int32</span></span>|<span data-ttu-id="28355-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28355-145">createdDateTime</span></span>|<span data-ttu-id="28355-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28355-146">DateTimeOffset</span></span>|<span data-ttu-id="28355-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28355-148">lastModifiedDateTime</span></span>|<span data-ttu-id="28355-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28355-149">DateTimeOffset</span></span>|<span data-ttu-id="28355-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-151">Version</span><span class="sxs-lookup"><span data-stu-id="28355-151">version</span></span>|<span data-ttu-id="28355-152">Int32</span><span class="sxs-lookup"><span data-stu-id="28355-152">Int32</span></span>|<span data-ttu-id="28355-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="28355-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="28355-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-154">iosRestriction</span></span>|[<span data-ttu-id="28355-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-156">Not yet documented</span></span>|
|<span data-ttu-id="28355-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-157">windowsRestriction</span></span>|[<span data-ttu-id="28355-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-159">Not yet documented</span></span>|
|<span data-ttu-id="28355-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="28355-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-162">Not yet documented</span></span>|
|<span data-ttu-id="28355-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-163">androidRestriction</span></span>|[<span data-ttu-id="28355-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-165">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-165">Not yet documented</span></span>|
|<span data-ttu-id="28355-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="28355-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-168">Not yet documented</span></span>|
|<span data-ttu-id="28355-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-169">macRestriction</span></span>|[<span data-ttu-id="28355-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-171">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-171">Not yet documented</span></span>|
|<span data-ttu-id="28355-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-172">macOSRestriction</span></span>|[<span data-ttu-id="28355-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="28355-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="28355-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28355-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="28355-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="28355-175">Response</span></span>
<span data-ttu-id="28355-176">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28355-176">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28355-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28355-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="28355-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28355-178">Request</span></span>
<span data-ttu-id="28355-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28355-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

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

### <a name="response"></a><span data-ttu-id="28355-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="28355-180">Response</span></span>
<span data-ttu-id="28355-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28355-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





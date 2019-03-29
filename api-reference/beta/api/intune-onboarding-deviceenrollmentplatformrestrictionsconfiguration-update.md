---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7432e9bd253499ac225ba6f033dd6af5b43e266
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967727"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="865c1-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="865c1-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="865c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="865c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="865c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="865c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="865c1-106">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="865c1-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="865c1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="865c1-107">Prerequisites</span></span>
<span data-ttu-id="865c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="865c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="865c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="865c1-110">Permission type</span></span>|<span data-ttu-id="865c1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="865c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="865c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="865c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="865c1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="865c1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="865c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="865c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="865c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="865c1-115">Not supported.</span></span>|
|<span data-ttu-id="865c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="865c1-116">Application</span></span>|<span data-ttu-id="865c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="865c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="865c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="865c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="865c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="865c1-119">Request headers</span></span>
|<span data-ttu-id="865c1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="865c1-120">Header</span></span>|<span data-ttu-id="865c1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="865c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="865c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="865c1-122">Authorization</span></span>|<span data-ttu-id="865c1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="865c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="865c1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="865c1-124">Accept</span></span>|<span data-ttu-id="865c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="865c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="865c1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="865c1-126">Request body</span></span>
<span data-ttu-id="865c1-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="865c1-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="865c1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="865c1-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="865c1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="865c1-129">Property</span></span>|<span data-ttu-id="865c1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="865c1-130">Type</span></span>|<span data-ttu-id="865c1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="865c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="865c1-132">id</span><span class="sxs-lookup"><span data-stu-id="865c1-132">id</span></span>|<span data-ttu-id="865c1-133">String</span><span class="sxs-lookup"><span data-stu-id="865c1-133">String</span></span>|<span data-ttu-id="865c1-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="865c1-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="865c1-135">displayName</span></span>|<span data-ttu-id="865c1-136">String</span><span class="sxs-lookup"><span data-stu-id="865c1-136">String</span></span>|<span data-ttu-id="865c1-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-138">description</span><span class="sxs-lookup"><span data-stu-id="865c1-138">description</span></span>|<span data-ttu-id="865c1-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="865c1-139">String</span></span>|<span data-ttu-id="865c1-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="865c1-141">priority</span></span>|<span data-ttu-id="865c1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="865c1-142">Int32</span></span>|<span data-ttu-id="865c1-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="865c1-144">createdDateTime</span></span>|<span data-ttu-id="865c1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="865c1-145">DateTimeOffset</span></span>|<span data-ttu-id="865c1-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="865c1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="865c1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="865c1-148">DateTimeOffset</span></span>|<span data-ttu-id="865c1-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-150">Version</span><span class="sxs-lookup"><span data-stu-id="865c1-150">version</span></span>|<span data-ttu-id="865c1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="865c1-151">Int32</span></span>|<span data-ttu-id="865c1-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="865c1-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="865c1-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-153">iosRestriction</span></span>|[<span data-ttu-id="865c1-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-155">Not yet documented</span></span>|
|<span data-ttu-id="865c1-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-156">windowsRestriction</span></span>|[<span data-ttu-id="865c1-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-158">Not yet documented</span></span>|
|<span data-ttu-id="865c1-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="865c1-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-161">Not yet documented</span></span>|
|<span data-ttu-id="865c1-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-162">androidRestriction</span></span>|[<span data-ttu-id="865c1-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-164">Not yet documented</span></span>|
|<span data-ttu-id="865c1-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="865c1-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-167">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-167">Not yet documented</span></span>|
|<span data-ttu-id="865c1-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-168">macRestriction</span></span>|[<span data-ttu-id="865c1-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-170">Not yet documented</span></span>|
|<span data-ttu-id="865c1-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-171">macOSRestriction</span></span>|[<span data-ttu-id="865c1-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="865c1-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="865c1-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="865c1-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="865c1-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="865c1-174">Response</span></span>
<span data-ttu-id="865c1-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="865c1-175">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="865c1-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="865c1-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="865c1-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="865c1-177">Request</span></span>
<span data-ttu-id="865c1-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="865c1-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="865c1-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="865c1-179">Response</span></span>
<span data-ttu-id="865c1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="865c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





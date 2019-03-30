---
title: deviceEnrollmentPlatformRestrictionsConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9b7cdaa623ecdcc61c4c162cd7af13b3722f533
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987167"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="3d97e-103">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="3d97e-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="3d97e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d97e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d97e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3d97e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d97e-106">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d97e-106">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d97e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d97e-107">Prerequisites</span></span>
<span data-ttu-id="3d97e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d97e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d97e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d97e-110">Permission type</span></span>|<span data-ttu-id="3d97e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d97e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d97e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d97e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d97e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d97e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d97e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d97e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d97e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d97e-115">Not supported.</span></span>|
|<span data-ttu-id="3d97e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d97e-116">Application</span></span>|<span data-ttu-id="3d97e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d97e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d97e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d97e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d97e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d97e-119">Request headers</span></span>
|<span data-ttu-id="3d97e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d97e-120">Header</span></span>|<span data-ttu-id="3d97e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3d97e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d97e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d97e-122">Authorization</span></span>|<span data-ttu-id="3d97e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d97e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d97e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d97e-124">Accept</span></span>|<span data-ttu-id="3d97e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d97e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d97e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d97e-126">Request body</span></span>
<span data-ttu-id="3d97e-127">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3d97e-127">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="3d97e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3d97e-128">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="3d97e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d97e-129">Property</span></span>|<span data-ttu-id="3d97e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3d97e-130">Type</span></span>|<span data-ttu-id="3d97e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d97e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d97e-132">id</span><span class="sxs-lookup"><span data-stu-id="3d97e-132">id</span></span>|<span data-ttu-id="3d97e-133">String</span><span class="sxs-lookup"><span data-stu-id="3d97e-133">String</span></span>|<span data-ttu-id="3d97e-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="3d97e-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3d97e-135">displayName</span></span>|<span data-ttu-id="3d97e-136">String</span><span class="sxs-lookup"><span data-stu-id="3d97e-136">String</span></span>|<span data-ttu-id="3d97e-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-138">description</span><span class="sxs-lookup"><span data-stu-id="3d97e-138">description</span></span>|<span data-ttu-id="3d97e-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d97e-139">String</span></span>|<span data-ttu-id="3d97e-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="3d97e-141">priority</span></span>|<span data-ttu-id="3d97e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3d97e-142">Int32</span></span>|<span data-ttu-id="3d97e-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d97e-144">createdDateTime</span></span>|<span data-ttu-id="3d97e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d97e-145">DateTimeOffset</span></span>|<span data-ttu-id="3d97e-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d97e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="3d97e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d97e-148">DateTimeOffset</span></span>|<span data-ttu-id="3d97e-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-150">Version</span><span class="sxs-lookup"><span data-stu-id="3d97e-150">version</span></span>|<span data-ttu-id="3d97e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3d97e-151">Int32</span></span>|<span data-ttu-id="3d97e-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d97e-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d97e-153">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-153">iosRestriction</span></span>|[<span data-ttu-id="3d97e-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-155">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-155">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-156">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-156">windowsRestriction</span></span>|[<span data-ttu-id="3d97e-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-158">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-158">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-159">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-159">windowsMobileRestriction</span></span>|[<span data-ttu-id="3d97e-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-161">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-161">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-162">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-162">androidRestriction</span></span>|[<span data-ttu-id="3d97e-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-164">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-164">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-165">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-165">androidForWorkRestriction</span></span>|[<span data-ttu-id="3d97e-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-167">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-167">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-168">macRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-168">macRestriction</span></span>|[<span data-ttu-id="3d97e-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-170">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-170">Not yet documented</span></span>|
|<span data-ttu-id="3d97e-171">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-171">macOSRestriction</span></span>|[<span data-ttu-id="3d97e-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d97e-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d97e-173">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3d97e-173">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3d97e-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d97e-174">Response</span></span>
<span data-ttu-id="3d97e-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3d97e-175">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d97e-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d97e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d97e-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d97e-177">Request</span></span>
<span data-ttu-id="3d97e-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d97e-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="3d97e-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d97e-179">Response</span></span>
<span data-ttu-id="3d97e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d97e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: deviceEnrollmentPlatformRestrictionsConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 204b18b654e8cc13e1808d27643cd477d188a0b0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988952"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="b1134-103">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="b1134-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="b1134-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b1134-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1134-105">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1134-105">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1134-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1134-106">Prerequisites</span></span>
<span data-ttu-id="b1134-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1134-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1134-109">Permission type</span></span>|<span data-ttu-id="b1134-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1134-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1134-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1134-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1134-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1134-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1134-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1134-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1134-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1134-114">Not supported.</span></span>|
|<span data-ttu-id="b1134-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1134-115">Application</span></span>|<span data-ttu-id="b1134-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1134-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1134-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1134-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b1134-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1134-118">Request headers</span></span>
|<span data-ttu-id="b1134-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1134-119">Header</span></span>|<span data-ttu-id="b1134-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b1134-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1134-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1134-121">Authorization</span></span>|<span data-ttu-id="b1134-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1134-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1134-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b1134-123">Accept</span></span>|<span data-ttu-id="b1134-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1134-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1134-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1134-125">Request body</span></span>
<span data-ttu-id="b1134-126">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b1134-126">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="b1134-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b1134-127">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="b1134-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1134-128">Property</span></span>|<span data-ttu-id="b1134-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b1134-129">Type</span></span>|<span data-ttu-id="b1134-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1134-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1134-131">id</span><span class="sxs-lookup"><span data-stu-id="b1134-131">id</span></span>|<span data-ttu-id="b1134-132">String</span><span class="sxs-lookup"><span data-stu-id="b1134-132">String</span></span>|<span data-ttu-id="b1134-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b1134-134">displayName</span></span>|<span data-ttu-id="b1134-135">String</span><span class="sxs-lookup"><span data-stu-id="b1134-135">String</span></span>|<span data-ttu-id="b1134-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-137">description</span><span class="sxs-lookup"><span data-stu-id="b1134-137">description</span></span>|<span data-ttu-id="b1134-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1134-138">String</span></span>|<span data-ttu-id="b1134-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="b1134-140">priority</span></span>|<span data-ttu-id="b1134-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b1134-141">Int32</span></span>|<span data-ttu-id="b1134-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1134-143">createdDateTime</span></span>|<span data-ttu-id="b1134-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1134-144">DateTimeOffset</span></span>|<span data-ttu-id="b1134-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1134-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b1134-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1134-147">DateTimeOffset</span></span>|<span data-ttu-id="b1134-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-149">Version</span><span class="sxs-lookup"><span data-stu-id="b1134-149">version</span></span>|<span data-ttu-id="b1134-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b1134-150">Int32</span></span>|<span data-ttu-id="b1134-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1134-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b1134-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-152">iosRestriction</span></span>|[<span data-ttu-id="b1134-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b1134-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b1134-154">Not yet documented</span></span>|
|<span data-ttu-id="b1134-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-155">windowsRestriction</span></span>|[<span data-ttu-id="b1134-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b1134-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b1134-157">Not yet documented</span></span>|
|<span data-ttu-id="b1134-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="b1134-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b1134-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b1134-160">Not yet documented</span></span>|
|<span data-ttu-id="b1134-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-161">androidRestriction</span></span>|[<span data-ttu-id="b1134-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b1134-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b1134-163">Not yet documented</span></span>|
|<span data-ttu-id="b1134-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-164">macOSRestriction</span></span>|[<span data-ttu-id="b1134-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1134-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="b1134-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b1134-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1134-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1134-167">Response</span></span>
<span data-ttu-id="b1134-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b1134-168">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1134-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1134-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1134-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1134-170">Request</span></span>
<span data-ttu-id="b1134-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1134-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1134-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1134-172">Response</span></span>
<span data-ttu-id="b1134-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1134-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




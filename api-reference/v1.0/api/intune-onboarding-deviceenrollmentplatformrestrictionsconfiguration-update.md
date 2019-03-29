---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92ed097d4b086708264346bcc029277f5f9b1ee5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959600"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="ab49a-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ab49a-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="ab49a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ab49a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab49a-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ab49a-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab49a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab49a-106">Prerequisites</span></span>
<span data-ttu-id="ab49a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab49a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab49a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab49a-109">Permission type</span></span>|<span data-ttu-id="ab49a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab49a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab49a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab49a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab49a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab49a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab49a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab49a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab49a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab49a-114">Not supported.</span></span>|
|<span data-ttu-id="ab49a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab49a-115">Application</span></span>|<span data-ttu-id="ab49a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab49a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab49a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab49a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab49a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab49a-118">Request headers</span></span>
|<span data-ttu-id="ab49a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ab49a-119">Header</span></span>|<span data-ttu-id="ab49a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ab49a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab49a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab49a-121">Authorization</span></span>|<span data-ttu-id="ab49a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab49a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab49a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ab49a-123">Accept</span></span>|<span data-ttu-id="ab49a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab49a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab49a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab49a-125">Request body</span></span>
<span data-ttu-id="ab49a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ab49a-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="ab49a-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ab49a-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="ab49a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ab49a-128">Property</span></span>|<span data-ttu-id="ab49a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ab49a-129">Type</span></span>|<span data-ttu-id="ab49a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ab49a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab49a-131">id</span><span class="sxs-lookup"><span data-stu-id="ab49a-131">id</span></span>|<span data-ttu-id="ab49a-132">String</span><span class="sxs-lookup"><span data-stu-id="ab49a-132">String</span></span>|<span data-ttu-id="ab49a-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ab49a-134">displayName</span></span>|<span data-ttu-id="ab49a-135">String</span><span class="sxs-lookup"><span data-stu-id="ab49a-135">String</span></span>|<span data-ttu-id="ab49a-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-137">description</span><span class="sxs-lookup"><span data-stu-id="ab49a-137">description</span></span>|<span data-ttu-id="ab49a-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ab49a-138">String</span></span>|<span data-ttu-id="ab49a-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="ab49a-140">priority</span></span>|<span data-ttu-id="ab49a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ab49a-141">Int32</span></span>|<span data-ttu-id="ab49a-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab49a-143">createdDateTime</span></span>|<span data-ttu-id="ab49a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab49a-144">DateTimeOffset</span></span>|<span data-ttu-id="ab49a-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab49a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="ab49a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab49a-147">DateTimeOffset</span></span>|<span data-ttu-id="ab49a-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-149">Version</span><span class="sxs-lookup"><span data-stu-id="ab49a-149">version</span></span>|<span data-ttu-id="ab49a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ab49a-150">Int32</span></span>|<span data-ttu-id="ab49a-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab49a-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ab49a-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-152">iosRestriction</span></span>|[<span data-ttu-id="ab49a-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ab49a-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ab49a-154">Not yet documented</span></span>|
|<span data-ttu-id="ab49a-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-155">windowsRestriction</span></span>|[<span data-ttu-id="ab49a-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ab49a-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ab49a-157">Not yet documented</span></span>|
|<span data-ttu-id="ab49a-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="ab49a-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ab49a-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ab49a-160">Not yet documented</span></span>|
|<span data-ttu-id="ab49a-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-161">androidRestriction</span></span>|[<span data-ttu-id="ab49a-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ab49a-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ab49a-163">Not yet documented</span></span>|
|<span data-ttu-id="ab49a-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-164">macOSRestriction</span></span>|[<span data-ttu-id="ab49a-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ab49a-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ab49a-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ab49a-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ab49a-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab49a-167">Response</span></span>
<span data-ttu-id="ab49a-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ab49a-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab49a-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab49a-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab49a-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab49a-170">Request</span></span>
<span data-ttu-id="ab49a-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab49a-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab49a-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab49a-172">Response</span></span>
<span data-ttu-id="ab49a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab49a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




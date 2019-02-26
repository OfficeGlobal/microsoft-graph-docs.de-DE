---
title: DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8b877e81512bf6994cc29b9bcec1e7f943f98c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255899"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="0e974-103">DeviceEnrollmentPlatformRestrictionsConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0e974-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="0e974-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0e974-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e974-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e974-105">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e974-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e974-106">Prerequisites</span></span>
<span data-ttu-id="0e974-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e974-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e974-109">Permission type</span></span>|<span data-ttu-id="0e974-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e974-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e974-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e974-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e974-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e974-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0e974-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e974-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e974-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e974-114">Not supported.</span></span>|
|<span data-ttu-id="0e974-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e974-115">Application</span></span>|<span data-ttu-id="0e974-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e974-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e974-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e974-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e974-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e974-118">Request headers</span></span>
|<span data-ttu-id="0e974-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0e974-119">Header</span></span>|<span data-ttu-id="0e974-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0e974-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e974-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e974-121">Authorization</span></span>|<span data-ttu-id="0e974-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e974-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e974-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e974-123">Accept</span></span>|<span data-ttu-id="0e974-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e974-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e974-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e974-125">Request body</span></span>
<span data-ttu-id="0e974-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0e974-126">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="0e974-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0e974-127">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="0e974-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e974-128">Property</span></span>|<span data-ttu-id="0e974-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0e974-129">Type</span></span>|<span data-ttu-id="0e974-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e974-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e974-131">id</span><span class="sxs-lookup"><span data-stu-id="0e974-131">id</span></span>|<span data-ttu-id="0e974-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e974-132">String</span></span>|<span data-ttu-id="0e974-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0e974-134">displayName</span></span>|<span data-ttu-id="0e974-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e974-135">String</span></span>|<span data-ttu-id="0e974-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-137">description</span><span class="sxs-lookup"><span data-stu-id="0e974-137">description</span></span>|<span data-ttu-id="0e974-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e974-138">String</span></span>|<span data-ttu-id="0e974-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="0e974-140">priority</span></span>|<span data-ttu-id="0e974-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0e974-141">Int32</span></span>|<span data-ttu-id="0e974-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e974-143">createdDateTime</span></span>|<span data-ttu-id="0e974-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e974-144">DateTimeOffset</span></span>|<span data-ttu-id="0e974-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e974-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0e974-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e974-147">DateTimeOffset</span></span>|<span data-ttu-id="0e974-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-149">Version</span><span class="sxs-lookup"><span data-stu-id="0e974-149">version</span></span>|<span data-ttu-id="0e974-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0e974-150">Int32</span></span>|<span data-ttu-id="0e974-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e974-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0e974-152">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-152">iosRestriction</span></span>|[<span data-ttu-id="0e974-153">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-153">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0e974-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e974-154">Not yet documented</span></span>|
|<span data-ttu-id="0e974-155">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-155">windowsRestriction</span></span>|[<span data-ttu-id="0e974-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0e974-157">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e974-157">Not yet documented</span></span>|
|<span data-ttu-id="0e974-158">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-158">windowsMobileRestriction</span></span>|[<span data-ttu-id="0e974-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0e974-160">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e974-160">Not yet documented</span></span>|
|<span data-ttu-id="0e974-161">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-161">androidRestriction</span></span>|[<span data-ttu-id="0e974-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0e974-163">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e974-163">Not yet documented</span></span>|
|<span data-ttu-id="0e974-164">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-164">macOSRestriction</span></span>|[<span data-ttu-id="0e974-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="0e974-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="0e974-166">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="0e974-166">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0e974-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e974-167">Response</span></span>
<span data-ttu-id="0e974-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0e974-168">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e974-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e974-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e974-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e974-170">Request</span></span>
<span data-ttu-id="0e974-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e974-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e974-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e974-172">Response</span></span>
<span data-ttu-id="0e974-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e974-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




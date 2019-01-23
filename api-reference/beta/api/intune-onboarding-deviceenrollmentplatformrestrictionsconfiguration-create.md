---
title: deviceEnrollmentPlatformRestrictionsConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentPlatformRestrictionsConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b2910d8b87535464f449a8649173102aab8b134
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407277"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="3e6e2-103">deviceEnrollmentPlatformRestrictionsConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="3e6e2-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="3e6e2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e6e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e6e2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e6e2-107">Erstellen eines neuen [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e6e2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e6e2-108">Prerequisites</span></span>
<span data-ttu-id="3e6e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e6e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3e6e2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e6e2-111">Permission type</span></span>|<span data-ttu-id="3e6e2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e6e2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e6e2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e6e2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e6e2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e6e2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e6e2-116">Not supported.</span></span>|
|<span data-ttu-id="3e6e2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e6e2-117">Application</span></span>|<span data-ttu-id="3e6e2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e6e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e6e2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e6e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e6e2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e6e2-120">Request headers</span></span>
|<span data-ttu-id="3e6e2-121">Header</span><span class="sxs-lookup"><span data-stu-id="3e6e2-121">Header</span></span>|<span data-ttu-id="3e6e2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3e6e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e6e2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3e6e2-123">Authorization</span></span>|<span data-ttu-id="3e6e2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3e6e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e6e2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3e6e2-125">Accept</span></span>|<span data-ttu-id="3e6e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e6e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e6e2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e6e2-127">Request body</span></span>
<span data-ttu-id="3e6e2-128">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceEnrollmentPlatformRestrictionsConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="3e6e2-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentPlatformRestrictionsConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="3e6e2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e6e2-130">Property</span></span>|<span data-ttu-id="3e6e2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3e6e2-131">Type</span></span>|<span data-ttu-id="3e6e2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e6e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e6e2-133">id</span><span class="sxs-lookup"><span data-stu-id="3e6e2-133">id</span></span>|<span data-ttu-id="3e6e2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e6e2-134">String</span></span>|<span data-ttu-id="3e6e2-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e6e2-136">displayName</span></span>|<span data-ttu-id="3e6e2-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e6e2-137">String</span></span>|<span data-ttu-id="3e6e2-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-139">description</span><span class="sxs-lookup"><span data-stu-id="3e6e2-139">description</span></span>|<span data-ttu-id="3e6e2-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e6e2-140">String</span></span>|<span data-ttu-id="3e6e2-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="3e6e2-142">priority</span></span>|<span data-ttu-id="3e6e2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3e6e2-143">Int32</span></span>|<span data-ttu-id="3e6e2-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e6e2-145">createdDateTime</span></span>|<span data-ttu-id="3e6e2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e6e2-146">DateTimeOffset</span></span>|<span data-ttu-id="3e6e2-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e6e2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="3e6e2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e6e2-149">DateTimeOffset</span></span>|<span data-ttu-id="3e6e2-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-151">Version</span><span class="sxs-lookup"><span data-stu-id="3e6e2-151">version</span></span>|<span data-ttu-id="3e6e2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3e6e2-152">Int32</span></span>|<span data-ttu-id="3e6e2-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e6e2-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e6e2-154">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-154">iosRestriction</span></span>|[<span data-ttu-id="3e6e2-155">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-155">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-156">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-156">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-157">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-157">windowsRestriction</span></span>|[<span data-ttu-id="3e6e2-158">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-158">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-159">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-159">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-160">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-160">windowsMobileRestriction</span></span>|[<span data-ttu-id="3e6e2-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-162">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-162">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-163">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-163">androidRestriction</span></span>|[<span data-ttu-id="3e6e2-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-165">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-165">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-166">androidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-166">androidForWorkRestriction</span></span>|[<span data-ttu-id="3e6e2-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-168">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-168">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-169">macRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-169">macRestriction</span></span>|[<span data-ttu-id="3e6e2-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-171">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-171">Not yet documented</span></span>|
|<span data-ttu-id="3e6e2-172">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-172">macOSRestriction</span></span>|[<span data-ttu-id="3e6e2-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3e6e2-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3e6e2-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-174">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3e6e2-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e6e2-175">Response</span></span>
<span data-ttu-id="3e6e2-176">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-176">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e6e2-177">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e6e2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e6e2-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e6e2-178">Request</span></span>
<span data-ttu-id="3e6e2-179">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e6e2-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e6e2-180">Response</span></span>
<span data-ttu-id="3e6e2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e6e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





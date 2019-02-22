---
title: WindowsOfficeClientSecurityConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windowsOfficeClientSecurityConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ff4df803272ef4c3d3ec8f07d553fe7abddbb65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162776"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="0fef4-103">WindowsOfficeClientSecurityConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0fef4-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="0fef4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fef4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fef4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0fef4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fef4-106">Aktualisieren der Eigenschaften eines [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0fef4-106">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fef4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0fef4-107">Prerequisites</span></span>
<span data-ttu-id="0fef4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fef4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0fef4-110">Permission type</span></span>|<span data-ttu-id="0fef4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0fef4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fef4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0fef4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fef4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fef4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fef4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0fef4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fef4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fef4-115">Not supported.</span></span>|
|<span data-ttu-id="0fef4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0fef4-116">Application</span></span>|<span data-ttu-id="0fef4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0fef4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fef4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fef4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0fef4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0fef4-119">Request headers</span></span>
|<span data-ttu-id="0fef4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0fef4-120">Header</span></span>|<span data-ttu-id="0fef4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0fef4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fef4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fef4-122">Authorization</span></span>|<span data-ttu-id="0fef4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0fef4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fef4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0fef4-124">Accept</span></span>|<span data-ttu-id="0fef4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fef4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fef4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0fef4-126">Request body</span></span>
<span data-ttu-id="0fef4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0fef4-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="0fef4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0fef4-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="0fef4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fef4-129">Property</span></span>|<span data-ttu-id="0fef4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0fef4-130">Type</span></span>|<span data-ttu-id="0fef4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fef4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fef4-132">id</span><span class="sxs-lookup"><span data-stu-id="0fef4-132">id</span></span>|<span data-ttu-id="0fef4-133">string</span><span class="sxs-lookup"><span data-stu-id="0fef4-133">String</span></span>|<span data-ttu-id="0fef4-134">ID der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="0fef4-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="0fef4-135">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="0fef4-136">userPreferencePayload</span></span>|<span data-ttu-id="0fef4-137">Stream</span><span class="sxs-lookup"><span data-stu-id="0fef4-137">Stream</span></span>|<span data-ttu-id="0fef4-138">Einstellungs Einstellungen JSON-Zeichenfolge im Binärformat können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="0fef4-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="0fef4-139">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="0fef4-140">policyPayload</span></span>|<span data-ttu-id="0fef4-141">Stream</span><span class="sxs-lookup"><span data-stu-id="0fef4-141">Stream</span></span>|<span data-ttu-id="0fef4-142">JSON-Zeichenfolge für Richtlinieneinstellungen im Binärformat können diese Werte nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="0fef4-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="0fef4-143">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-144">description</span><span class="sxs-lookup"><span data-stu-id="0fef4-144">description</span></span>|<span data-ttu-id="0fef4-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fef4-145">String</span></span>|<span data-ttu-id="0fef4-146">Administrator: Beschreibung der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="0fef4-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="0fef4-147">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0fef4-148">displayName</span></span>|<span data-ttu-id="0fef4-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fef4-149">String</span></span>|<span data-ttu-id="0fef4-150">Vom Administrator bereitgestellter Name der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="0fef4-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="0fef4-151">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-152">assignments</span><span class="sxs-lookup"><span data-stu-id="0fef4-152">assignments</span></span>|<span data-ttu-id="0fef4-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0fef4-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0fef4-154">Die Liste der Gruppenzuweisungen für die Richtlinie..</span><span class="sxs-lookup"><span data-stu-id="0fef4-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="0fef4-155">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-156">Priorität</span><span class="sxs-lookup"><span data-stu-id="0fef4-156">priority</span></span>|<span data-ttu-id="0fef4-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0fef4-157">Int32</span></span>|<span data-ttu-id="0fef4-158">Der Prioritätswert sollte für jede Richtlinie unter einem Mandanten eindeutig sein und für die Konfliktlösung verwendet werden, niedrigere Werte bedeuten eine hohe Priorität.</span><span class="sxs-lookup"><span data-stu-id="0fef4-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="0fef4-159">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fef4-160">lastModifiedDateTime</span></span>|<span data-ttu-id="0fef4-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="0fef4-161">DateTime</span></span>|<span data-ttu-id="0fef4-162">Datum der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="0fef4-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="0fef4-163">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0fef4-164">userCheckinSummary</span></span>|[<span data-ttu-id="0fef4-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0fef4-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0fef4-166">Zusammenfassung der Benutzer Einchecken für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="0fef4-166">User check-in summary for the policy.</span></span> <span data-ttu-id="0fef4-167">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0fef4-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="0fef4-168">checkinStatuses</span></span>|<span data-ttu-id="0fef4-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="0fef4-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0fef4-170">Liste der Office-Client Eincheckstatus.</span><span class="sxs-lookup"><span data-stu-id="0fef4-170">List of office Client check-in status.</span></span> <span data-ttu-id="0fef4-171">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fef4-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0fef4-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fef4-172">Response</span></span>
<span data-ttu-id="0fef4-173">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0fef4-173">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fef4-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0fef4-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fef4-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0fef4-175">Request</span></span>
<span data-ttu-id="0fef4-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0fef4-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0fef4-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="0fef4-177">Response</span></span>
<span data-ttu-id="0fef4-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0fef4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```




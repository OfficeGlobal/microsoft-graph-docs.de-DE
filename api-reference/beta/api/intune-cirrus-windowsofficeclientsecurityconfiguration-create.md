---
title: WindowsOfficeClientSecurityConfiguration erstellen
description: Erstellen eines neuen windowsOfficeClientSecurityConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5100321365afac461de5602bb8a1c96d6f3f1564
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167249"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="faf93-103">WindowsOfficeClientSecurityConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="faf93-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="faf93-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="faf93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faf93-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="faf93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faf93-106">Erstellen eines neuen [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="faf93-106">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faf93-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="faf93-107">Prerequisites</span></span>
<span data-ttu-id="faf93-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf93-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="faf93-110">Permission type</span></span>|<span data-ttu-id="faf93-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="faf93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf93-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="faf93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="faf93-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf93-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faf93-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="faf93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf93-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faf93-115">Not supported.</span></span>|
|<span data-ttu-id="faf93-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="faf93-116">Application</span></span>|<span data-ttu-id="faf93-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faf93-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faf93-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="faf93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="faf93-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="faf93-119">Request headers</span></span>
|<span data-ttu-id="faf93-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="faf93-120">Header</span></span>|<span data-ttu-id="faf93-121">Wert</span><span class="sxs-lookup"><span data-stu-id="faf93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faf93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="faf93-122">Authorization</span></span>|<span data-ttu-id="faf93-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="faf93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faf93-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="faf93-124">Accept</span></span>|<span data-ttu-id="faf93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="faf93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf93-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="faf93-126">Request body</span></span>
<span data-ttu-id="faf93-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="faf93-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="faf93-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="faf93-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="faf93-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="faf93-129">Property</span></span>|<span data-ttu-id="faf93-130">Typ</span><span class="sxs-lookup"><span data-stu-id="faf93-130">Type</span></span>|<span data-ttu-id="faf93-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="faf93-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf93-132">id</span><span class="sxs-lookup"><span data-stu-id="faf93-132">id</span></span>|<span data-ttu-id="faf93-133">string</span><span class="sxs-lookup"><span data-stu-id="faf93-133">String</span></span>|<span data-ttu-id="faf93-134">ID der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="faf93-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="faf93-135">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="faf93-136">userPreferencePayload</span></span>|<span data-ttu-id="faf93-137">Stream</span><span class="sxs-lookup"><span data-stu-id="faf93-137">Stream</span></span>|<span data-ttu-id="faf93-138">Einstellungs Einstellungen JSON-Zeichenfolge im Binärformat können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="faf93-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="faf93-139">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-140">policyPayload</span><span class="sxs-lookup"><span data-stu-id="faf93-140">policyPayload</span></span>|<span data-ttu-id="faf93-141">Stream</span><span class="sxs-lookup"><span data-stu-id="faf93-141">Stream</span></span>|<span data-ttu-id="faf93-142">JSON-Zeichenfolge für Richtlinieneinstellungen im Binärformat können diese Werte nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="faf93-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="faf93-143">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-144">description</span><span class="sxs-lookup"><span data-stu-id="faf93-144">description</span></span>|<span data-ttu-id="faf93-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="faf93-145">String</span></span>|<span data-ttu-id="faf93-146">Administrator: Beschreibung der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="faf93-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="faf93-147">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-148">displayName</span><span class="sxs-lookup"><span data-stu-id="faf93-148">displayName</span></span>|<span data-ttu-id="faf93-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="faf93-149">String</span></span>|<span data-ttu-id="faf93-150">Vom Administrator bereitgestellter Name der Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="faf93-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="faf93-151">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-152">assignments</span><span class="sxs-lookup"><span data-stu-id="faf93-152">assignments</span></span>|<span data-ttu-id="faf93-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="faf93-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="faf93-154">Die Liste der Gruppenzuweisungen für die Richtlinie..</span><span class="sxs-lookup"><span data-stu-id="faf93-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="faf93-155">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-156">Priorität</span><span class="sxs-lookup"><span data-stu-id="faf93-156">priority</span></span>|<span data-ttu-id="faf93-157">Int32</span><span class="sxs-lookup"><span data-stu-id="faf93-157">Int32</span></span>|<span data-ttu-id="faf93-158">Der Prioritätswert sollte für jede Richtlinie unter einem Mandanten eindeutig sein und für die Konfliktlösung verwendet werden, niedrigere Werte bedeuten eine hohe Priorität.</span><span class="sxs-lookup"><span data-stu-id="faf93-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="faf93-159">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faf93-160">lastModifiedDateTime</span></span>|<span data-ttu-id="faf93-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="faf93-161">DateTime</span></span>|<span data-ttu-id="faf93-162">Datum der letzten Änderung der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="faf93-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="faf93-163">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-164">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="faf93-164">userCheckinSummary</span></span>|[<span data-ttu-id="faf93-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="faf93-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="faf93-166">Zusammenfassung der Benutzer Einchecken für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="faf93-166">User check-in summary for the policy.</span></span> <span data-ttu-id="faf93-167">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="faf93-168">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="faf93-168">checkinStatuses</span></span>|<span data-ttu-id="faf93-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="faf93-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="faf93-170">Liste der Office-Client Eincheckstatus.</span><span class="sxs-lookup"><span data-stu-id="faf93-170">List of office Client check-in status.</span></span> <span data-ttu-id="faf93-171">Geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faf93-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="faf93-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="faf93-172">Response</span></span>
<span data-ttu-id="faf93-173">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="faf93-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf93-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="faf93-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="faf93-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="faf93-175">Request</span></span>
<span data-ttu-id="faf93-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="faf93-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
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

### <a name="response"></a><span data-ttu-id="faf93-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="faf93-177">Response</span></span>
<span data-ttu-id="faf93-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="faf93-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




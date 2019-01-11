---
title: WindowsOfficeClientSecurityConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsOfficeClientSecurityConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 52db50c1014833468b9eee435e06c96153aa5fc5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853389"
---
# <a name="update-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="58c40-103">WindowsOfficeClientSecurityConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58c40-103">Update windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="58c40-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58c40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58c40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58c40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58c40-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58c40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58c40-107">Aktualisieren Sie die Eigenschaften eines [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58c40-107">Update the properties of a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58c40-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58c40-108">Prerequisites</span></span>
<span data-ttu-id="58c40-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58c40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58c40-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58c40-111">Permission type</span></span>|<span data-ttu-id="58c40-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58c40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58c40-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58c40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58c40-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c40-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58c40-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58c40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58c40-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58c40-116">Not supported.</span></span>|
|<span data-ttu-id="58c40-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58c40-117">Application</span></span>|<span data-ttu-id="58c40-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58c40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58c40-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58c40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58c40-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58c40-120">Request headers</span></span>
|<span data-ttu-id="58c40-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58c40-121">Header</span></span>|<span data-ttu-id="58c40-122">Wert</span><span class="sxs-lookup"><span data-stu-id="58c40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58c40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58c40-123">Authorization</span></span>|<span data-ttu-id="58c40-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58c40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58c40-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58c40-125">Accept</span></span>|<span data-ttu-id="58c40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58c40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58c40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58c40-127">Request body</span></span>
<span data-ttu-id="58c40-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="58c40-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="58c40-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="58c40-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="58c40-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58c40-130">Property</span></span>|<span data-ttu-id="58c40-131">Typ</span><span class="sxs-lookup"><span data-stu-id="58c40-131">Type</span></span>|<span data-ttu-id="58c40-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58c40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c40-133">id</span><span class="sxs-lookup"><span data-stu-id="58c40-133">id</span></span>|<span data-ttu-id="58c40-134">String</span><span class="sxs-lookup"><span data-stu-id="58c40-134">String</span></span>|<span data-ttu-id="58c40-135">ID des die Richtlinie Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="58c40-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="58c40-136">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="58c40-137">userPreferencePayload</span></span>|<span data-ttu-id="58c40-138">Stream</span><span class="sxs-lookup"><span data-stu-id="58c40-138">Stream</span></span>|<span data-ttu-id="58c40-139">Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="58c40-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="58c40-140">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="58c40-141">policyPayload</span></span>|<span data-ttu-id="58c40-142">Stream</span><span class="sxs-lookup"><span data-stu-id="58c40-142">Stream</span></span>|<span data-ttu-id="58c40-143">Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="58c40-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="58c40-144">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-145">description</span><span class="sxs-lookup"><span data-stu-id="58c40-145">description</span></span>|<span data-ttu-id="58c40-146">String</span><span class="sxs-lookup"><span data-stu-id="58c40-146">String</span></span>|<span data-ttu-id="58c40-147">Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="58c40-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="58c40-148">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-149">displayName</span><span class="sxs-lookup"><span data-stu-id="58c40-149">displayName</span></span>|<span data-ttu-id="58c40-150">String</span><span class="sxs-lookup"><span data-stu-id="58c40-150">String</span></span>|<span data-ttu-id="58c40-151">Admin Namen der Richtlinie ein Office-Client-Konfiguration bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="58c40-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="58c40-152">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-153">assignments</span><span class="sxs-lookup"><span data-stu-id="58c40-153">assignments</span></span>|<span data-ttu-id="58c40-154">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="58c40-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="58c40-155">Die Liste der zugewiesenen Gruppe für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="58c40-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="58c40-156">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-157">Priorität</span><span class="sxs-lookup"><span data-stu-id="58c40-157">priority</span></span>|<span data-ttu-id="58c40-158">Int32</span><span class="sxs-lookup"><span data-stu-id="58c40-158">Int32</span></span>|<span data-ttu-id="58c40-159">Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.</span><span class="sxs-lookup"><span data-stu-id="58c40-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="58c40-160">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58c40-161">lastModifiedDateTime</span></span>|<span data-ttu-id="58c40-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="58c40-162">DateTime</span></span>|<span data-ttu-id="58c40-163">Zuletzt geänderte Datetime-Stempel der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="58c40-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="58c40-164">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="58c40-165">userCheckinSummary</span></span>|[<span data-ttu-id="58c40-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="58c40-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="58c40-167">Benutzer Einchecken Zusammenfassung für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="58c40-167">User check-in summary for the policy.</span></span> <span data-ttu-id="58c40-168">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="58c40-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="58c40-169">checkinStatuses</span></span>|<span data-ttu-id="58c40-170">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="58c40-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="58c40-171">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="58c40-171">List of office Client check-in status.</span></span> <span data-ttu-id="58c40-172">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58c40-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="58c40-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="58c40-173">Response</span></span>
<span data-ttu-id="58c40-174">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="58c40-174">If successful, this method returns a `200 OK` response code and an updated [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58c40-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58c40-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="58c40-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58c40-176">Request</span></span>
<span data-ttu-id="58c40-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58c40-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58c40-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="58c40-178">Response</span></span>
<span data-ttu-id="58c40-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58c40-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




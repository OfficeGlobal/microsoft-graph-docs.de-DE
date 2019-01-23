---
title: Erstellen von windowsOfficeClientSecurityConfiguration
description: Erstellen eines neuen WindowsOfficeClientSecurityConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fedc5897f5cc3422de3eb83c8e5d94dcfc56f117
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417322"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="d1f5d-103">Erstellen von windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1f5d-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="d1f5d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1f5d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1f5d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f5d-107">Erstellen eines neuen [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1f5d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d1f5d-108">Prerequisites</span></span>
<span data-ttu-id="d1f5d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f5d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1f5d-111">Permission type</span></span>|<span data-ttu-id="d1f5d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1f5d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1f5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1f5d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1f5d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1f5d-116">Not supported.</span></span>|
|<span data-ttu-id="d1f5d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-117">Application</span></span>|<span data-ttu-id="d1f5d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1f5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1f5d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1f5d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1f5d-120">Request headers</span></span>
|<span data-ttu-id="d1f5d-121">Header</span><span class="sxs-lookup"><span data-stu-id="d1f5d-121">Header</span></span>|<span data-ttu-id="d1f5d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d1f5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1f5d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-123">Authorization</span></span>|<span data-ttu-id="d1f5d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d1f5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1f5d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d1f5d-125">Accept</span></span>|<span data-ttu-id="d1f5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1f5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f5d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1f5d-127">Request body</span></span>
<span data-ttu-id="d1f5d-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="d1f5d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="d1f5d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1f5d-130">Property</span></span>|<span data-ttu-id="d1f5d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d1f5d-131">Type</span></span>|<span data-ttu-id="d1f5d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f5d-133">id</span><span class="sxs-lookup"><span data-stu-id="d1f5d-133">id</span></span>|<span data-ttu-id="d1f5d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1f5d-134">String</span></span>|<span data-ttu-id="d1f5d-135">ID des die Richtlinie Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="d1f5d-136">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="d1f5d-137">userPreferencePayload</span></span>|<span data-ttu-id="d1f5d-138">Stream</span><span class="sxs-lookup"><span data-stu-id="d1f5d-138">Stream</span></span>|<span data-ttu-id="d1f5d-139">Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="d1f5d-140">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="d1f5d-141">policyPayload</span></span>|<span data-ttu-id="d1f5d-142">Stream</span><span class="sxs-lookup"><span data-stu-id="d1f5d-142">Stream</span></span>|<span data-ttu-id="d1f5d-143">Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="d1f5d-144">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-145">description</span><span class="sxs-lookup"><span data-stu-id="d1f5d-145">description</span></span>|<span data-ttu-id="d1f5d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1f5d-146">String</span></span>|<span data-ttu-id="d1f5d-147">Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="d1f5d-148">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-149">displayName</span><span class="sxs-lookup"><span data-stu-id="d1f5d-149">displayName</span></span>|<span data-ttu-id="d1f5d-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1f5d-150">String</span></span>|<span data-ttu-id="d1f5d-151">Admin Namen der Richtlinie ein Office-Client-Konfiguration bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="d1f5d-152">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-153">assignments</span><span class="sxs-lookup"><span data-stu-id="d1f5d-153">assignments</span></span>|<span data-ttu-id="d1f5d-154">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d1f5d-155">Die Liste der zugewiesenen Gruppe für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="d1f5d-156">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-157">Priorität</span><span class="sxs-lookup"><span data-stu-id="d1f5d-157">priority</span></span>|<span data-ttu-id="d1f5d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f5d-158">Int32</span></span>|<span data-ttu-id="d1f5d-159">Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="d1f5d-160">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1f5d-161">lastModifiedDateTime</span></span>|<span data-ttu-id="d1f5d-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="d1f5d-162">DateTime</span></span>|<span data-ttu-id="d1f5d-163">Zuletzt geänderte Datetime-Stempel der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="d1f5d-164">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d1f5d-165">userCheckinSummary</span></span>|[<span data-ttu-id="d1f5d-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d1f5d-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d1f5d-167">Benutzer Einchecken Zusammenfassung für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-167">User check-in summary for the policy.</span></span> <span data-ttu-id="d1f5d-168">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="d1f5d-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="d1f5d-169">checkinStatuses</span></span>|<span data-ttu-id="d1f5d-170">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d1f5d-171">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-171">List of office Client check-in status.</span></span> <span data-ttu-id="d1f5d-172">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f5d-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="d1f5d-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1f5d-173">Response</span></span>
<span data-ttu-id="d1f5d-174">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f5d-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1f5d-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1f5d-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1f5d-176">Request</span></span>
<span data-ttu-id="d1f5d-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1f5d-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1f5d-178">Response</span></span>
<span data-ttu-id="d1f5d-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1f5d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




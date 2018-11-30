---
title: Erstellen von windowsOfficeClientConfiguration
description: Erstellen Sie eine neue Richtlinie nicht sicherheitsrelevante mit Adressieren von Gruppen.
ms.openlocfilehash: add83255d614306677787b3ed35a9792822deec2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058906"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="003d9-103">Erstellen von windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="003d9-103">Create windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="003d9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="003d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="003d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="003d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="003d9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="003d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="003d9-107">Erstellen Sie eine neue Richtlinie nicht sicherheitsrelevante mit Adressieren von Gruppen.</span><span class="sxs-lookup"><span data-stu-id="003d9-107">Create a new non-security policy with targeting groups.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="003d9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="003d9-108">Prerequisites</span></span>
<span data-ttu-id="003d9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003d9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="003d9-111">Permission type</span></span>|<span data-ttu-id="003d9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="003d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="003d9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="003d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="003d9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003d9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="003d9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="003d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="003d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="003d9-116">Not supported.</span></span>|
|<span data-ttu-id="003d9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="003d9-117">Application</span></span>|<span data-ttu-id="003d9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="003d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="003d9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="003d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="003d9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="003d9-120">Request headers</span></span>
|<span data-ttu-id="003d9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="003d9-121">Header</span></span>|<span data-ttu-id="003d9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="003d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="003d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="003d9-123">Authorization</span></span>|<span data-ttu-id="003d9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="003d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="003d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="003d9-125">Accept</span></span>|<span data-ttu-id="003d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="003d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="003d9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="003d9-127">Request body</span></span>
<span data-ttu-id="003d9-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="003d9-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="003d9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="003d9-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="003d9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="003d9-130">Property</span></span>|<span data-ttu-id="003d9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="003d9-131">Type</span></span>|<span data-ttu-id="003d9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003d9-133">id</span><span class="sxs-lookup"><span data-stu-id="003d9-133">id</span></span>|<span data-ttu-id="003d9-134">String</span><span class="sxs-lookup"><span data-stu-id="003d9-134">String</span></span>|<span data-ttu-id="003d9-135">ID des die Richtlinie Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="003d9-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="003d9-136">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="003d9-137">userPreferencePayload</span></span>|<span data-ttu-id="003d9-138">Stream</span><span class="sxs-lookup"><span data-stu-id="003d9-138">Stream</span></span>|<span data-ttu-id="003d9-139">Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="003d9-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="003d9-140">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="003d9-141">policyPayload</span></span>|<span data-ttu-id="003d9-142">Stream</span><span class="sxs-lookup"><span data-stu-id="003d9-142">Stream</span></span>|<span data-ttu-id="003d9-143">Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.</span><span class="sxs-lookup"><span data-stu-id="003d9-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="003d9-144">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-145">description</span><span class="sxs-lookup"><span data-stu-id="003d9-145">description</span></span>|<span data-ttu-id="003d9-146">String</span><span class="sxs-lookup"><span data-stu-id="003d9-146">String</span></span>|<span data-ttu-id="003d9-147">Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.</span><span class="sxs-lookup"><span data-stu-id="003d9-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="003d9-148">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-149">displayName</span><span class="sxs-lookup"><span data-stu-id="003d9-149">displayName</span></span>|<span data-ttu-id="003d9-150">String</span><span class="sxs-lookup"><span data-stu-id="003d9-150">String</span></span>|<span data-ttu-id="003d9-151">Admin Namen der Richtlinie ein Office-Client-Konfiguration bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="003d9-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="003d9-152">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-153">assignments</span><span class="sxs-lookup"><span data-stu-id="003d9-153">assignments</span></span>|<span data-ttu-id="003d9-154">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="003d9-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="003d9-155">Die Liste der zugewiesenen Gruppe für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="003d9-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="003d9-156">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-157">Priorität</span><span class="sxs-lookup"><span data-stu-id="003d9-157">priority</span></span>|<span data-ttu-id="003d9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="003d9-158">Int32</span></span>|<span data-ttu-id="003d9-159">Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.</span><span class="sxs-lookup"><span data-stu-id="003d9-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="003d9-160">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="003d9-161">lastModifiedDateTime</span></span>|<span data-ttu-id="003d9-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="003d9-162">DateTime</span></span>|<span data-ttu-id="003d9-163">Zuletzt geänderte Datetime-Stempel der Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="003d9-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="003d9-164">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="003d9-165">userCheckinSummary</span></span>|[<span data-ttu-id="003d9-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="003d9-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="003d9-167">Benutzer Einchecken Zusammenfassung für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="003d9-167">User check-in summary for the policy.</span></span> <span data-ttu-id="003d9-168">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="003d9-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="003d9-169">checkinStatuses</span></span>|<span data-ttu-id="003d9-170">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="003d9-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="003d9-171">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="003d9-171">List of office Client check-in status.</span></span> <span data-ttu-id="003d9-172">Geerbt von [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="003d9-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="003d9-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="003d9-173">Response</span></span>
<span data-ttu-id="003d9-174">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="003d9-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003d9-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="003d9-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="003d9-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="003d9-176">Request</span></span>
<span data-ttu-id="003d9-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="003d9-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

### <a name="response"></a><span data-ttu-id="003d9-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="003d9-178">Response</span></span>
<span data-ttu-id="003d9-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="003d9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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




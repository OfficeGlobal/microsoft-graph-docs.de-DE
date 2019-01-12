---
title: WindowsOfficeClientConfiguration aktualisieren
description: Eine bestimmte nicht sicherheitsrelevante Richtlinie Nutzlast Patch.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 76179dadc4620617487c66b719626778fa4e4f26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983506"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="0616e-103">WindowsOfficeClientConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0616e-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="0616e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0616e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0616e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0616e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0616e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0616e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0616e-107">Eine bestimmte nicht sicherheitsrelevante Richtlinie Nutzlast Patch.</span><span class="sxs-lookup"><span data-stu-id="0616e-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0616e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0616e-108">Prerequisites</span></span>
<span data-ttu-id="0616e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0616e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0616e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0616e-111">Permission type</span></span>|<span data-ttu-id="0616e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0616e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0616e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0616e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0616e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0616e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0616e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0616e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0616e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0616e-116">Not supported.</span></span>|
|<span data-ttu-id="0616e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0616e-117">Application</span></span>|<span data-ttu-id="0616e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0616e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0616e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0616e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="0616e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0616e-120">Request headers</span></span>
|<span data-ttu-id="0616e-121">Header</span><span class="sxs-lookup"><span data-stu-id="0616e-121">Header</span></span>|<span data-ttu-id="0616e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0616e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0616e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0616e-123">Authorization</span></span>|<span data-ttu-id="0616e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0616e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0616e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0616e-125">Accept</span></span>|<span data-ttu-id="0616e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0616e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0616e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0616e-127">Request body</span></span>
<span data-ttu-id="0616e-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0616e-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="0616e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0616e-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="0616e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0616e-130">Property</span></span>|<span data-ttu-id="0616e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0616e-131">Type</span></span>|<span data-ttu-id="0616e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0616e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0616e-133">id</span><span class="sxs-lookup"><span data-stu-id="0616e-133">id</span></span>|<span data-ttu-id="0616e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0616e-134">String</span></span>|<span data-ttu-id="0616e-135">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="0616e-136">userPreferencePayload</span></span>|<span data-ttu-id="0616e-137">Stream</span><span class="sxs-lookup"><span data-stu-id="0616e-137">Stream</span></span>|<span data-ttu-id="0616e-138">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="0616e-139">policyPayload</span></span>|<span data-ttu-id="0616e-140">Stream</span><span class="sxs-lookup"><span data-stu-id="0616e-140">Stream</span></span>|<span data-ttu-id="0616e-141">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-142">description</span><span class="sxs-lookup"><span data-stu-id="0616e-142">description</span></span>|<span data-ttu-id="0616e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0616e-143">String</span></span>|<span data-ttu-id="0616e-144">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0616e-145">displayName</span></span>|<span data-ttu-id="0616e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0616e-146">String</span></span>|<span data-ttu-id="0616e-147">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-148">Priorität</span><span class="sxs-lookup"><span data-stu-id="0616e-148">priority</span></span>|<span data-ttu-id="0616e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0616e-149">Int32</span></span>|<span data-ttu-id="0616e-150">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0616e-151">userCheckinSummary</span></span>|[<span data-ttu-id="0616e-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0616e-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0616e-153">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0616e-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="0616e-154">checkinStatuses</span></span>|<span data-ttu-id="0616e-155">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0616e-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0616e-156">Noch nicht dokumentiert Inherited aus [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0616e-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0616e-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="0616e-157">Response</span></span>
<span data-ttu-id="0616e-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0616e-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0616e-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0616e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="0616e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0616e-160">Request</span></span>
<span data-ttu-id="0616e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0616e-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0616e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="0616e-162">Response</span></span>
<span data-ttu-id="0616e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0616e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




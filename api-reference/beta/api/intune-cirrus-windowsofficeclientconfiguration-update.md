---
title: WindowsOfficeClientConfiguration aktualisieren
description: Patchen einer bestimmten nichtsicherheitsbezogenen Richtlinien Nutzlast.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d116d846b6540ea2b9e2a91f54a5abdfa81e2409
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139249"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="c0d01-103">WindowsOfficeClientConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c0d01-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="c0d01-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0d01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0d01-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c0d01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0d01-106">Patchen einer bestimmten nichtsicherheitsbezogenen Richtlinien Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="c0d01-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0d01-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0d01-107">Prerequisites</span></span>
<span data-ttu-id="c0d01-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0d01-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0d01-110">Permission type</span></span>|<span data-ttu-id="c0d01-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0d01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0d01-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0d01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0d01-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d01-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0d01-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0d01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0d01-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0d01-115">Not supported.</span></span>|
|<span data-ttu-id="c0d01-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0d01-116">Application</span></span>|<span data-ttu-id="c0d01-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0d01-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0d01-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0d01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="c0d01-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0d01-119">Request headers</span></span>
|<span data-ttu-id="c0d01-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c0d01-120">Header</span></span>|<span data-ttu-id="c0d01-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c0d01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0d01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0d01-122">Authorization</span></span>|<span data-ttu-id="c0d01-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0d01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0d01-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0d01-124">Accept</span></span>|<span data-ttu-id="c0d01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0d01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0d01-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0d01-126">Request body</span></span>
<span data-ttu-id="c0d01-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c0d01-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="c0d01-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c0d01-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="c0d01-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0d01-129">Property</span></span>|<span data-ttu-id="c0d01-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c0d01-130">Type</span></span>|<span data-ttu-id="c0d01-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0d01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0d01-132">id</span><span class="sxs-lookup"><span data-stu-id="c0d01-132">id</span></span>|<span data-ttu-id="c0d01-133">string</span><span class="sxs-lookup"><span data-stu-id="c0d01-133">String</span></span>|<span data-ttu-id="c0d01-134">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-135">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="c0d01-135">userPreferencePayload</span></span>|<span data-ttu-id="c0d01-136">Stream</span><span class="sxs-lookup"><span data-stu-id="c0d01-136">Stream</span></span>|<span data-ttu-id="c0d01-137">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-138">policyPayload</span><span class="sxs-lookup"><span data-stu-id="c0d01-138">policyPayload</span></span>|<span data-ttu-id="c0d01-139">Stream</span><span class="sxs-lookup"><span data-stu-id="c0d01-139">Stream</span></span>|<span data-ttu-id="c0d01-140">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-141">description</span><span class="sxs-lookup"><span data-stu-id="c0d01-141">description</span></span>|<span data-ttu-id="c0d01-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0d01-142">String</span></span>|<span data-ttu-id="c0d01-143">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c0d01-144">displayName</span></span>|<span data-ttu-id="c0d01-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c0d01-145">String</span></span>|<span data-ttu-id="c0d01-146">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-147">Priorität</span><span class="sxs-lookup"><span data-stu-id="c0d01-147">priority</span></span>|<span data-ttu-id="c0d01-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c0d01-148">Int32</span></span>|<span data-ttu-id="c0d01-149">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-150">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c0d01-150">userCheckinSummary</span></span>|[<span data-ttu-id="c0d01-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c0d01-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="c0d01-152">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c0d01-153">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="c0d01-153">checkinStatuses</span></span>|<span data-ttu-id="c0d01-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c0d01-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="c0d01-155">Noch nicht dokumentiert geerbt von [für](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0d01-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c0d01-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0d01-156">Response</span></span>
<span data-ttu-id="c0d01-157">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [für](../resources/intune-cirrus-officeclientconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c0d01-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0d01-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0d01-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0d01-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0d01-159">Request</span></span>
<span data-ttu-id="c0d01-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0d01-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0d01-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0d01-161">Response</span></span>
<span data-ttu-id="c0d01-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0d01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




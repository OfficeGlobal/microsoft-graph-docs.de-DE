---
title: importAppleDeviceIdentityList-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 714459b7ee5ab1dd65bb274ad2315e832ce56436
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141482"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="2f352-103">importAppleDeviceIdentityList-Aktion</span><span class="sxs-lookup"><span data-stu-id="2f352-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="2f352-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f352-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f352-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f352-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f352-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2f352-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f352-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f352-107">Prerequisites</span></span>
<span data-ttu-id="2f352-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f352-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f352-110">Permission type</span></span>|<span data-ttu-id="2f352-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f352-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f352-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f352-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f352-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f352-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f352-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f352-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f352-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f352-115">Not supported.</span></span>|
|<span data-ttu-id="2f352-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f352-116">Application</span></span>|<span data-ttu-id="2f352-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f352-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f352-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f352-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="2f352-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f352-119">Request headers</span></span>
|<span data-ttu-id="2f352-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f352-120">Header</span></span>|<span data-ttu-id="2f352-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2f352-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f352-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f352-122">Authorization</span></span>|<span data-ttu-id="2f352-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f352-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f352-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f352-124">Accept</span></span>|<span data-ttu-id="2f352-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f352-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f352-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f352-126">Request body</span></span>
<span data-ttu-id="2f352-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2f352-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2f352-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2f352-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2f352-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f352-129">Property</span></span>|<span data-ttu-id="2f352-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2f352-130">Type</span></span>|<span data-ttu-id="2f352-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f352-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f352-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2f352-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="2f352-133">[importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="2f352-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="2f352-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2f352-134">Not yet documented</span></span>|
|<span data-ttu-id="2f352-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2f352-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="2f352-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f352-136">Boolean</span></span>|<span data-ttu-id="2f352-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="2f352-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f352-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f352-138">Response</span></span>
<span data-ttu-id="2f352-139">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f352-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f352-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f352-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f352-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f352-141">Request</span></span>
<span data-ttu-id="2f352-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f352-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 756

{
  "importedAppleDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="2f352-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f352-143">Response</span></span>
<span data-ttu-id="2f352-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f352-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





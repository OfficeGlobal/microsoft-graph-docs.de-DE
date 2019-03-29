---
title: importAppleDeviceIdentityList-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac9194ca888b8e46358748754856cdb072d8c12
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967146"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="fc5c5-103">importAppleDeviceIdentityList-Aktion</span><span class="sxs-lookup"><span data-stu-id="fc5c5-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="fc5c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc5c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc5c5-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fc5c5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc5c5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fc5c5-107">Prerequisites</span></span>
<span data-ttu-id="fc5c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc5c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc5c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc5c5-110">Permission type</span></span>|<span data-ttu-id="fc5c5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc5c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc5c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc5c5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc5c5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc5c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc5c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc5c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc5c5-115">Not supported.</span></span>|
|<span data-ttu-id="fc5c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc5c5-116">Application</span></span>|<span data-ttu-id="fc5c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc5c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc5c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc5c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="fc5c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc5c5-119">Request headers</span></span>
|<span data-ttu-id="fc5c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fc5c5-120">Header</span></span>|<span data-ttu-id="fc5c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fc5c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc5c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc5c5-122">Authorization</span></span>|<span data-ttu-id="fc5c5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fc5c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc5c5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fc5c5-124">Accept</span></span>|<span data-ttu-id="fc5c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc5c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc5c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc5c5-126">Request body</span></span>
<span data-ttu-id="fc5c5-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fc5c5-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fc5c5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc5c5-129">Property</span></span>|<span data-ttu-id="fc5c5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fc5c5-130">Type</span></span>|<span data-ttu-id="fc5c5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc5c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc5c5-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="fc5c5-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="fc5c5-133">[importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="fc5c5-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="fc5c5-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-134">Not yet documented</span></span>|
|<span data-ttu-id="fc5c5-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="fc5c5-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="fc5c5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc5c5-136">Boolean</span></span>|<span data-ttu-id="fc5c5-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fc5c5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc5c5-138">Response</span></span>
<span data-ttu-id="fc5c5-139">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc5c5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc5c5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc5c5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc5c5-141">Request</span></span>
<span data-ttu-id="fc5c5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc5c5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc5c5-143">Response</span></span>
<span data-ttu-id="fc5c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc5c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





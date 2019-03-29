---
title: ImportedAppleDeviceIdentityResults aufListen
description: AufListen von Eigenschaften und Beziehungen der importedAppleDeviceIdentityResult-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63ee441c2d8b14a1788f51127542365b06ee17d1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970926"
---
# <a name="list-importedappledeviceidentityresults"></a><span data-ttu-id="d761f-103">ImportedAppleDeviceIdentityResults aufListen</span><span class="sxs-lookup"><span data-stu-id="d761f-103">List importedAppleDeviceIdentityResults</span></span>

> <span data-ttu-id="d761f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d761f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d761f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d761f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d761f-106">AufListen von Eigenschaften und Beziehungen der [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d761f-106">List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d761f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d761f-107">Prerequisites</span></span>
<span data-ttu-id="d761f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d761f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d761f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d761f-110">Permission type</span></span>|<span data-ttu-id="d761f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d761f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d761f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d761f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d761f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d761f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d761f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d761f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d761f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d761f-115">Not supported.</span></span>|
|<span data-ttu-id="d761f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d761f-116">Application</span></span>|<span data-ttu-id="d761f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d761f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d761f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d761f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="d761f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d761f-119">Request headers</span></span>
|<span data-ttu-id="d761f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d761f-120">Header</span></span>|<span data-ttu-id="d761f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d761f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d761f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d761f-122">Authorization</span></span>|<span data-ttu-id="d761f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d761f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d761f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d761f-124">Accept</span></span>|<span data-ttu-id="d761f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d761f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d761f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d761f-126">Request body</span></span>
<span data-ttu-id="d761f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d761f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d761f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d761f-128">Response</span></span>
<span data-ttu-id="d761f-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d761f-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d761f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d761f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d761f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d761f-131">Request</span></span>
<span data-ttu-id="d761f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d761f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="d761f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d761f-133">Response</span></span>
<span data-ttu-id="d761f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d761f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: ImportAppleDeviceIdentityList Aktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d19eec23d8f78fa3b007c59f43c0e320f9161e93
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423909"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="0c29a-103">ImportAppleDeviceIdentityList Aktion</span><span class="sxs-lookup"><span data-stu-id="0c29a-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="0c29a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0c29a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c29a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c29a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c29a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c29a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c29a-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0c29a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c29a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c29a-108">Prerequisites</span></span>
<span data-ttu-id="0c29a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c29a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c29a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c29a-111">Permission type</span></span>|<span data-ttu-id="0c29a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c29a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c29a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c29a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c29a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c29a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c29a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c29a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c29a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c29a-116">Not supported.</span></span>|
|<span data-ttu-id="0c29a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c29a-117">Application</span></span>|<span data-ttu-id="0c29a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c29a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c29a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c29a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="0c29a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c29a-120">Request headers</span></span>
|<span data-ttu-id="0c29a-121">Header</span><span class="sxs-lookup"><span data-stu-id="0c29a-121">Header</span></span>|<span data-ttu-id="0c29a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0c29a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c29a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0c29a-123">Authorization</span></span>|<span data-ttu-id="0c29a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c29a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c29a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c29a-125">Accept</span></span>|<span data-ttu-id="0c29a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c29a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c29a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c29a-127">Request body</span></span>
<span data-ttu-id="0c29a-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="0c29a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0c29a-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0c29a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0c29a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c29a-130">Property</span></span>|<span data-ttu-id="0c29a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0c29a-131">Type</span></span>|<span data-ttu-id="0c29a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c29a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c29a-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="0c29a-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="0c29a-134">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0c29a-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="0c29a-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0c29a-135">Not yet documented</span></span>|
|<span data-ttu-id="0c29a-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="0c29a-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="0c29a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c29a-137">Boolean</span></span>|<span data-ttu-id="0c29a-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0c29a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0c29a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c29a-139">Response</span></span>
<span data-ttu-id="0c29a-140">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0c29a-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c29a-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c29a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c29a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c29a-142">Request</span></span>
<span data-ttu-id="0c29a-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c29a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c29a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c29a-144">Response</span></span>
<span data-ttu-id="0c29a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c29a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





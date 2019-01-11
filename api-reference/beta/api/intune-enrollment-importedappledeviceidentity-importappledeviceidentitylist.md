---
title: ImportAppleDeviceIdentityList Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75a40be8d2ea3ddafadb78f95662dcadf7a9ac01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890601"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="a8b24-103">ImportAppleDeviceIdentityList Aktion</span><span class="sxs-lookup"><span data-stu-id="a8b24-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="a8b24-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8b24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8b24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8b24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8b24-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8b24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8b24-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8b24-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8b24-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8b24-108">Prerequisites</span></span>
<span data-ttu-id="a8b24-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8b24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8b24-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8b24-111">Permission type</span></span>|<span data-ttu-id="a8b24-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8b24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8b24-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8b24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8b24-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8b24-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8b24-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8b24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8b24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8b24-116">Not supported.</span></span>|
|<span data-ttu-id="a8b24-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8b24-117">Application</span></span>|<span data-ttu-id="a8b24-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8b24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8b24-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8b24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="a8b24-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8b24-120">Request headers</span></span>
|<span data-ttu-id="a8b24-121">Header</span><span class="sxs-lookup"><span data-stu-id="a8b24-121">Header</span></span>|<span data-ttu-id="a8b24-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a8b24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8b24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8b24-123">Authorization</span></span>|<span data-ttu-id="a8b24-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8b24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8b24-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a8b24-125">Accept</span></span>|<span data-ttu-id="a8b24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8b24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8b24-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8b24-127">Request body</span></span>
<span data-ttu-id="a8b24-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="a8b24-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8b24-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="a8b24-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8b24-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8b24-130">Property</span></span>|<span data-ttu-id="a8b24-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a8b24-131">Type</span></span>|<span data-ttu-id="a8b24-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8b24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b24-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a8b24-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="a8b24-134">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a8b24-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="a8b24-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8b24-135">Not yet documented</span></span>|
|<span data-ttu-id="a8b24-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a8b24-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="a8b24-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a8b24-137">Boolean</span></span>|<span data-ttu-id="a8b24-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8b24-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a8b24-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8b24-139">Response</span></span>
<span data-ttu-id="a8b24-140">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a8b24-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8b24-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8b24-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8b24-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8b24-142">Request</span></span>
<span data-ttu-id="a8b24-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8b24-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8b24-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8b24-144">Response</span></span>
<span data-ttu-id="a8b24-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8b24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






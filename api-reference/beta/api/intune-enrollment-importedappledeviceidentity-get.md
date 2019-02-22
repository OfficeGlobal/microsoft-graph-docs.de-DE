---
title: Importappledeviceidentitylist abrufen
description: Lesen von Eigenschaften und Beziehungen des Importappledeviceidentitylist-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12c4dcfd7c428a1647ccaec23067feea6ec806f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167564"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="c84e5-103">Importappledeviceidentitylist abrufen</span><span class="sxs-lookup"><span data-stu-id="c84e5-103">Get importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="c84e5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c84e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c84e5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c84e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c84e5-106">Lesen von Eigenschaften und Beziehungen des [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c84e5-106">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c84e5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c84e5-107">Prerequisites</span></span>
<span data-ttu-id="c84e5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c84e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c84e5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c84e5-110">Permission type</span></span>|<span data-ttu-id="c84e5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c84e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c84e5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c84e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c84e5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c84e5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c84e5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c84e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c84e5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c84e5-115">Not supported.</span></span>|
|<span data-ttu-id="c84e5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c84e5-116">Application</span></span>|<span data-ttu-id="c84e5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c84e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c84e5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c84e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c84e5-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c84e5-119">Optional query parameters</span></span>
<span data-ttu-id="c84e5-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c84e5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c84e5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c84e5-121">Request headers</span></span>
|<span data-ttu-id="c84e5-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c84e5-122">Header</span></span>|<span data-ttu-id="c84e5-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c84e5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c84e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c84e5-124">Authorization</span></span>|<span data-ttu-id="c84e5-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c84e5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c84e5-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c84e5-126">Accept</span></span>|<span data-ttu-id="c84e5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c84e5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c84e5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c84e5-128">Request body</span></span>
<span data-ttu-id="c84e5-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c84e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c84e5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c84e5-130">Response</span></span>
<span data-ttu-id="c84e5-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c84e5-131">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84e5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c84e5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c84e5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c84e5-133">Request</span></span>
<span data-ttu-id="c84e5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c84e5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="c84e5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c84e5-135">Response</span></span>
<span data-ttu-id="c84e5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c84e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 648

{
  "value": {
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
}
```





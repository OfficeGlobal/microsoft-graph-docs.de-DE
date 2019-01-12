---
title: Abrufen von importedAppleDeviceIdentityResult
description: Lesen Sie Eigenschaften und Beziehungen des ImportedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dcca0b1da7d377f8d39efa96a3961151600999a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934982"
---
# <a name="get-importedappledeviceidentityresult"></a><span data-ttu-id="2026a-103">Abrufen von importedAppleDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="2026a-103">Get importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="2026a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2026a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2026a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2026a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2026a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2026a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2026a-107">Lesen Sie Eigenschaften und Beziehungen des [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2026a-107">Read properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2026a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2026a-108">Prerequisites</span></span>
<span data-ttu-id="2026a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2026a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2026a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2026a-111">Permission type</span></span>|<span data-ttu-id="2026a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2026a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2026a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2026a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2026a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2026a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2026a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2026a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2026a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2026a-116">Not supported.</span></span>|
|<span data-ttu-id="2026a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2026a-117">Application</span></span>|<span data-ttu-id="2026a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2026a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2026a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2026a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2026a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2026a-120">Optional query parameters</span></span>
<span data-ttu-id="2026a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2026a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2026a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2026a-122">Request headers</span></span>
|<span data-ttu-id="2026a-123">Header</span><span class="sxs-lookup"><span data-stu-id="2026a-123">Header</span></span>|<span data-ttu-id="2026a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="2026a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2026a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2026a-125">Authorization</span></span>|<span data-ttu-id="2026a-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2026a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2026a-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2026a-127">Accept</span></span>|<span data-ttu-id="2026a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2026a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2026a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2026a-129">Request body</span></span>
<span data-ttu-id="2026a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2026a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2026a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2026a-131">Response</span></span>
<span data-ttu-id="2026a-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ImportedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2026a-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2026a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2026a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2026a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2026a-134">Request</span></span>
<span data-ttu-id="2026a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2026a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="2026a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2026a-136">Response</span></span>
<span data-ttu-id="2026a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2026a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
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
}
```






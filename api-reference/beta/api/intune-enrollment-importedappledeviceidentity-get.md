---
title: Abrufen von importedAppleDeviceIdentity
description: Lesen Sie Eigenschaften und Beziehungen des ImportedAppleDeviceIdentity-Objekts.
ms.openlocfilehash: bad76da11545d2fafef6843403077f31d87878a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060084"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="07030-103">Abrufen von importedAppleDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="07030-103">Get importedAppleDeviceIdentity</span></span>

> <span data-ttu-id="07030-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07030-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07030-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07030-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07030-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="07030-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07030-107">Lesen Sie Eigenschaften und Beziehungen des [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="07030-107">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07030-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="07030-108">Prerequisites</span></span>
<span data-ttu-id="07030-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07030-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07030-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07030-111">Permission type</span></span>|<span data-ttu-id="07030-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07030-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07030-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07030-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07030-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="07030-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="07030-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07030-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07030-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07030-116">Not supported.</span></span>|
|<span data-ttu-id="07030-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07030-117">Application</span></span>|<span data-ttu-id="07030-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07030-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07030-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07030-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07030-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="07030-120">Optional query parameters</span></span>
<span data-ttu-id="07030-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="07030-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="07030-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07030-122">Request headers</span></span>
|<span data-ttu-id="07030-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="07030-123">Header</span></span>|<span data-ttu-id="07030-124">Wert</span><span class="sxs-lookup"><span data-stu-id="07030-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07030-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07030-125">Authorization</span></span>|<span data-ttu-id="07030-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="07030-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07030-127">Accept</span><span class="sxs-lookup"><span data-stu-id="07030-127">Accept</span></span>|<span data-ttu-id="07030-128">application/json</span><span class="sxs-lookup"><span data-stu-id="07030-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07030-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07030-129">Request body</span></span>
<span data-ttu-id="07030-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="07030-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07030-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="07030-131">Response</span></span>
<span data-ttu-id="07030-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="07030-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07030-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07030-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="07030-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07030-134">Request</span></span>
<span data-ttu-id="07030-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07030-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="07030-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="07030-136">Response</span></span>
<span data-ttu-id="07030-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07030-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






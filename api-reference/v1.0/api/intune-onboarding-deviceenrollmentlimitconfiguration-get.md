---
title: deviceEnrollmentLimitConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceEnrollmentLimitConfiguration-Objekts.
ms.openlocfilehash: a06a5af5443aecfee9b021584aefcf59020c5b9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020065"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d96e3-103">deviceEnrollmentLimitConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="d96e3-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d96e3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d96e3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d96e3-105">Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d96e3-105">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d96e3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d96e3-106">Prerequisites</span></span>
<span data-ttu-id="d96e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d96e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d96e3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d96e3-109">Permission type</span></span>|<span data-ttu-id="d96e3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d96e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d96e3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d96e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d96e3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d96e3-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d96e3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d96e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d96e3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d96e3-114">Not supported.</span></span>|
|<span data-ttu-id="d96e3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d96e3-115">Application</span></span>|<span data-ttu-id="d96e3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d96e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d96e3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d96e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d96e3-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d96e3-118">Optional query parameters</span></span>
<span data-ttu-id="d96e3-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d96e3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d96e3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d96e3-120">Request headers</span></span>
|<span data-ttu-id="d96e3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d96e3-121">Header</span></span>|<span data-ttu-id="d96e3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d96e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d96e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d96e3-123">Authorization</span></span>|<span data-ttu-id="d96e3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d96e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d96e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d96e3-125">Accept</span></span>|<span data-ttu-id="d96e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d96e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d96e3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d96e3-127">Request body</span></span>
<span data-ttu-id="d96e3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d96e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d96e3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d96e3-129">Response</span></span>
<span data-ttu-id="d96e3-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d96e3-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d96e3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d96e3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d96e3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d96e3-132">Request</span></span>
<span data-ttu-id="d96e3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d96e3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d96e3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d96e3-134">Response</span></span>
<span data-ttu-id="d96e3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d96e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
    "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "limit": 5
  }
}
```



---
title: Abrufen von „enrollmentConfigurationAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs enrollmentConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 05b04b29b41ceb2c3e79e9836a3252ae386d59d3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342721"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="5f5f9-103">Abrufen von „enrollmentConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="5f5f9-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="5f5f9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f5f9-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5f5f9-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f5f9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f5f9-106">Prerequisites</span></span>
<span data-ttu-id="5f5f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f5f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f5f9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f5f9-109">Permission type</span></span>|<span data-ttu-id="5f5f9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f5f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f5f9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f5f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f5f9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f5f9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5f5f9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f5f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f5f9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f5f9-114">Not supported.</span></span>|
|<span data-ttu-id="5f5f9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f5f9-115">Application</span></span>|<span data-ttu-id="5f5f9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f5f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f5f9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f5f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f5f9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5f5f9-118">Optional query parameters</span></span>
<span data-ttu-id="5f5f9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5f5f9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f5f9-120">Request headers</span></span>
|<span data-ttu-id="5f5f9-121">Header</span><span class="sxs-lookup"><span data-stu-id="5f5f9-121">Header</span></span>|<span data-ttu-id="5f5f9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5f5f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f5f9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5f5f9-123">Authorization</span></span>|<span data-ttu-id="5f5f9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f5f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f5f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f5f9-125">Accept</span></span>|<span data-ttu-id="5f5f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f5f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f5f9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f5f9-127">Request body</span></span>
<span data-ttu-id="5f5f9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f5f9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f5f9-129">Response</span></span>
<span data-ttu-id="5f5f9-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f5f9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f5f9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f5f9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f5f9-132">Request</span></span>
<span data-ttu-id="5f5f9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5f5f9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f5f9-134">Response</span></span>
<span data-ttu-id="5f5f9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f5f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
    "id": "705b021c-021c-705b-1c02-5b701c025b70",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




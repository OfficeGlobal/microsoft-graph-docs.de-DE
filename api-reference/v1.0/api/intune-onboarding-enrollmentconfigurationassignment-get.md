---
title: Abrufen von „enrollmentConfigurationAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs enrollmentConfigurationAssignment.
ms.openlocfilehash: e9e9be8484770ae55a3daf7ac9114106a3a4846a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018155"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="f751c-103">Abrufen von „enrollmentConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="f751c-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="f751c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f751c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f751c-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f751c-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f751c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f751c-106">Prerequisites</span></span>
<span data-ttu-id="f751c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f751c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f751c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f751c-109">Permission type</span></span>|<span data-ttu-id="f751c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f751c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f751c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f751c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f751c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f751c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f751c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f751c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f751c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f751c-114">Not supported.</span></span>|
|<span data-ttu-id="f751c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f751c-115">Application</span></span>|<span data-ttu-id="f751c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f751c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f751c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f751c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f751c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f751c-118">Optional query parameters</span></span>
<span data-ttu-id="f751c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f751c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f751c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f751c-120">Request headers</span></span>
|<span data-ttu-id="f751c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f751c-121">Header</span></span>|<span data-ttu-id="f751c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f751c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f751c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f751c-123">Authorization</span></span>|<span data-ttu-id="f751c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f751c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f751c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f751c-125">Accept</span></span>|<span data-ttu-id="f751c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f751c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f751c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f751c-127">Request body</span></span>
<span data-ttu-id="f751c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f751c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f751c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f751c-129">Response</span></span>
<span data-ttu-id="f751c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f751c-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f751c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f751c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f751c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f751c-132">Request</span></span>
<span data-ttu-id="f751c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f751c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f751c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f751c-134">Response</span></span>
<span data-ttu-id="f751c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f751c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



---
title: enrollmentConfigurationAssignments auflisten
description: Auflisten von Eigenschaften und Beziehungen der enrollmentConfigurationAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b60c1e67ea4a294b130ab93dc443b11d8a169aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920331"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="4a523-103">enrollmentConfigurationAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="4a523-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="4a523-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a523-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a523-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a523-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a523-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a523-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a523-107">Auflisten von Eigenschaften und Beziehungen der [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="4a523-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a523-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a523-108">Prerequisites</span></span>
<span data-ttu-id="4a523-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a523-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a523-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a523-111">Permission type</span></span>|<span data-ttu-id="4a523-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a523-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a523-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a523-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a523-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a523-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4a523-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a523-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a523-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a523-116">Not supported.</span></span>|
|<span data-ttu-id="4a523-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a523-117">Application</span></span>|<span data-ttu-id="4a523-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a523-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a523-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a523-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4a523-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a523-120">Request headers</span></span>
|<span data-ttu-id="4a523-121">Header</span><span class="sxs-lookup"><span data-stu-id="4a523-121">Header</span></span>|<span data-ttu-id="4a523-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4a523-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a523-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a523-123">Authorization</span></span>|<span data-ttu-id="4a523-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a523-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a523-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a523-125">Accept</span></span>|<span data-ttu-id="4a523-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a523-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a523-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a523-127">Request body</span></span>
<span data-ttu-id="4a523-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a523-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a523-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a523-129">Response</span></span>
<span data-ttu-id="4a523-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4a523-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a523-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a523-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a523-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a523-132">Request</span></span>
<span data-ttu-id="4a523-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a523-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="4a523-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a523-134">Response</span></span>
<span data-ttu-id="4a523-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a523-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






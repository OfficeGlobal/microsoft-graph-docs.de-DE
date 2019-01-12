---
title: Abrufen von „termsAndConditionsAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1007de1496ed50b6f1d22ff702ea722247f24ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957256"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="8e2dd-103">Abrufen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="8e2dd-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="8e2dd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e2dd-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8e2dd-105">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e2dd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e2dd-106">Prerequisites</span></span>
<span data-ttu-id="8e2dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e2dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e2dd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e2dd-109">Permission type</span></span>|<span data-ttu-id="8e2dd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e2dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e2dd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e2dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e2dd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e2dd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8e2dd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e2dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e2dd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e2dd-114">Not supported.</span></span>|
|<span data-ttu-id="8e2dd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e2dd-115">Application</span></span>|<span data-ttu-id="8e2dd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e2dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e2dd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e2dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e2dd-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8e2dd-118">Optional query parameters</span></span>
<span data-ttu-id="8e2dd-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e2dd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e2dd-120">Request headers</span></span>
|<span data-ttu-id="8e2dd-121">Header</span><span class="sxs-lookup"><span data-stu-id="8e2dd-121">Header</span></span>|<span data-ttu-id="8e2dd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8e2dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e2dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e2dd-123">Authorization</span></span>|<span data-ttu-id="8e2dd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e2dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e2dd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8e2dd-125">Accept</span></span>|<span data-ttu-id="8e2dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e2dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e2dd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e2dd-127">Request body</span></span>
<span data-ttu-id="8e2dd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e2dd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e2dd-129">Response</span></span>
<span data-ttu-id="8e2dd-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e2dd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e2dd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e2dd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e2dd-132">Request</span></span>
<span data-ttu-id="8e2dd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8e2dd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e2dd-134">Response</span></span>
<span data-ttu-id="8e2dd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e2dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




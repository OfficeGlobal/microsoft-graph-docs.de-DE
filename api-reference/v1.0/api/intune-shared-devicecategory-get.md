---
title: Abrufen von „deviceCategory“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c2fac1d5bb242d77a3fbbce110d0bf8e4a2e30e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922452"
---
# <a name="get-devicecategory"></a><span data-ttu-id="acd11-103">Abrufen von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="acd11-103">Get deviceCategory</span></span>



> <span data-ttu-id="acd11-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acd11-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acd11-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="acd11-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acd11-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="acd11-106">Prerequisites</span></span>
<span data-ttu-id="acd11-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd11-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="acd11-109">Permission type</span></span>|<span data-ttu-id="acd11-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="acd11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acd11-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="acd11-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="acd11-112">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="acd11-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="acd11-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd11-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="acd11-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="acd11-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="acd11-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="acd11-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="acd11-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="acd11-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acd11-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acd11-117">Not supported.</span></span>|
|<span data-ttu-id="acd11-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="acd11-118">Application</span></span>|<span data-ttu-id="acd11-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="acd11-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acd11-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd11-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acd11-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="acd11-121">Optional query parameters</span></span>
<span data-ttu-id="acd11-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="acd11-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acd11-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="acd11-123">Request headers</span></span>
|<span data-ttu-id="acd11-124">Header</span><span class="sxs-lookup"><span data-stu-id="acd11-124">Header</span></span>|<span data-ttu-id="acd11-125">Wert</span><span class="sxs-lookup"><span data-stu-id="acd11-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acd11-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="acd11-126">Authorization</span></span>|<span data-ttu-id="acd11-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="acd11-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acd11-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="acd11-128">Accept</span></span>|<span data-ttu-id="acd11-129">application/json</span><span class="sxs-lookup"><span data-stu-id="acd11-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd11-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="acd11-130">Request body</span></span>
<span data-ttu-id="acd11-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="acd11-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd11-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd11-132">Response</span></span>
<span data-ttu-id="acd11-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="acd11-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd11-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="acd11-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="acd11-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="acd11-135">Request</span></span>
<span data-ttu-id="acd11-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="acd11-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="acd11-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="acd11-137">Response</span></span>
<span data-ttu-id="acd11-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="acd11-138">Here is an example of the response.</span></span> <span data-ttu-id="acd11-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="acd11-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="acd11-140">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="acd11-140">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```




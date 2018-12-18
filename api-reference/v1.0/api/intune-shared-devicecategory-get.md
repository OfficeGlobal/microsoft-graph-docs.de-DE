---
title: Abrufen von „deviceCategory“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory.
author: tfitzmac
ms.openlocfilehash: c69e3ecf97889636dd00deab213caf116233f6b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309699"
---
# <a name="get-devicecategory"></a><span data-ttu-id="b3171-103">Abrufen von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="b3171-103">Get deviceCategory</span></span>



> <span data-ttu-id="b3171-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3171-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3171-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b3171-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3171-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3171-106">Prerequisites</span></span>
<span data-ttu-id="b3171-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3171-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3171-109">Permission type</span></span>|<span data-ttu-id="b3171-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3171-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3171-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3171-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b3171-112">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="b3171-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b3171-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3171-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="b3171-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="b3171-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b3171-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3171-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b3171-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3171-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3171-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3171-117">Not supported.</span></span>|
|<span data-ttu-id="b3171-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3171-118">Application</span></span>|<span data-ttu-id="b3171-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3171-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3171-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3171-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3171-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3171-121">Optional query parameters</span></span>
<span data-ttu-id="b3171-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3171-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3171-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3171-123">Request headers</span></span>
|<span data-ttu-id="b3171-124">Header</span><span class="sxs-lookup"><span data-stu-id="b3171-124">Header</span></span>|<span data-ttu-id="b3171-125">Wert</span><span class="sxs-lookup"><span data-stu-id="b3171-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3171-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b3171-126">Authorization</span></span>|<span data-ttu-id="b3171-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3171-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3171-128">Accept</span><span class="sxs-lookup"><span data-stu-id="b3171-128">Accept</span></span>|<span data-ttu-id="b3171-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b3171-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3171-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3171-130">Request body</span></span>
<span data-ttu-id="b3171-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3171-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3171-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3171-132">Response</span></span>
<span data-ttu-id="b3171-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3171-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3171-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3171-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3171-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3171-135">Request</span></span>
<span data-ttu-id="b3171-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3171-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="b3171-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3171-137">Response</span></span>
<span data-ttu-id="b3171-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3171-138">Here is an example of the response.</span></span> <span data-ttu-id="b3171-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="b3171-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b3171-140">Eigenschaften von einer tatsächlichen Aufruf zurückgegeben variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="b3171-140">Properties returned from an actual call vary according to context.</span></span>

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




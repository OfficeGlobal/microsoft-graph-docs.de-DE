---
title: Abrufen von „deviceCategory“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b62523d4a17571c0ff6931b8ee462f21b4a1daa4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174538"
---
# <a name="get-devicecategory"></a><span data-ttu-id="94698-103">Abrufen von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="94698-103">Get deviceCategory</span></span>

> <span data-ttu-id="94698-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="94698-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94698-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94698-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94698-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="94698-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94698-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="94698-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94698-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94698-108">Prerequisites</span></span>

<span data-ttu-id="94698-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94698-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="94698-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94698-111">Permission type</span></span>|<span data-ttu-id="94698-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94698-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94698-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94698-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="94698-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="94698-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="94698-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="94698-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="94698-116">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="94698-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="94698-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="94698-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="94698-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94698-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94698-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94698-119">Not supported.</span></span>|
|<span data-ttu-id="94698-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94698-120">Application</span></span>|<span data-ttu-id="94698-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94698-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94698-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94698-122">HTTP Request</span></span>

<span data-ttu-id="94698-123">**deviceManagement**</span><span class="sxs-lookup"><span data-stu-id="94698-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="94698-124">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="94698-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94698-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="94698-125">Optional query parameters</span></span>

<span data-ttu-id="94698-126">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94698-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94698-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94698-127">Request headers</span></span>

|<span data-ttu-id="94698-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94698-128">Header</span></span>|<span data-ttu-id="94698-129">Wert</span><span class="sxs-lookup"><span data-stu-id="94698-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94698-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="94698-130">Authorization</span></span>|<span data-ttu-id="94698-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94698-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94698-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="94698-132">Accept</span></span>|<span data-ttu-id="94698-133">application/json</span><span class="sxs-lookup"><span data-stu-id="94698-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94698-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94698-134">Request body</span></span>

<span data-ttu-id="94698-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="94698-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94698-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="94698-136">Response</span></span>

<span data-ttu-id="94698-137">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="94698-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94698-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94698-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="94698-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94698-139">Request</span></span>

<span data-ttu-id="94698-140">Hier sind Beispiele für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94698-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="94698-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="94698-141">Response</span></span>

<span data-ttu-id="94698-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="94698-142">Here is an example of the response.</span></span> <span data-ttu-id="94698-143">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="94698-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="94698-144">Von einem tatsächlichen Aufruf zurückgegebene Eigenschaften variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="94698-144">Properties returned from an actual call vary according to context.</span></span>

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




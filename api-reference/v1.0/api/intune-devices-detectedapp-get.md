---
title: Abrufen von „detectedApp“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs detectedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bdad0890f3060827ddd888dd47fa89911912322b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811192"
---
# <a name="get-detectedapp"></a><span data-ttu-id="965ae-103">Abrufen von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="965ae-103">Get detectedApp</span></span>

> <span data-ttu-id="965ae-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="965ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="965ae-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="965ae-105">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="965ae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="965ae-106">Prerequisites</span></span>
<span data-ttu-id="965ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="965ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="965ae-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="965ae-109">Permission type</span></span>|<span data-ttu-id="965ae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="965ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="965ae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="965ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="965ae-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="965ae-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="965ae-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="965ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="965ae-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="965ae-114">Not supported.</span></span>|
|<span data-ttu-id="965ae-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="965ae-115">Application</span></span>|<span data-ttu-id="965ae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="965ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="965ae-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="965ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="965ae-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="965ae-118">Optional query parameters</span></span>
<span data-ttu-id="965ae-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="965ae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="965ae-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="965ae-120">Request headers</span></span>
|<span data-ttu-id="965ae-121">Header</span><span class="sxs-lookup"><span data-stu-id="965ae-121">Header</span></span>|<span data-ttu-id="965ae-122">Wert</span><span class="sxs-lookup"><span data-stu-id="965ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="965ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="965ae-123">Authorization</span></span>|<span data-ttu-id="965ae-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="965ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="965ae-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="965ae-125">Accept</span></span>|<span data-ttu-id="965ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="965ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="965ae-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="965ae-127">Request body</span></span>
<span data-ttu-id="965ae-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="965ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="965ae-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="965ae-129">Response</span></span>
<span data-ttu-id="965ae-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="965ae-130">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="965ae-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="965ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="965ae-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="965ae-132">Request</span></span>
<span data-ttu-id="965ae-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="965ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="965ae-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="965ae-134">Response</span></span>
<span data-ttu-id="965ae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="965ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```




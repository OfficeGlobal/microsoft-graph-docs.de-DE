---
title: Auflisten von „detectedApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs detectedApp auf.
ms.openlocfilehash: 1f56f00d9a872e0d6187522ec795d11ce292225a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018290"
---
# <a name="list-detectedapps"></a><span data-ttu-id="b58f9-103">Auflisten von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="b58f9-103">List detectedApps</span></span>

> <span data-ttu-id="b58f9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b58f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b58f9-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b58f9-105">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b58f9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b58f9-106">Prerequisites</span></span>
<span data-ttu-id="b58f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b58f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b58f9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b58f9-109">Permission type</span></span>|<span data-ttu-id="b58f9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b58f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b58f9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b58f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b58f9-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b58f9-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b58f9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b58f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b58f9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b58f9-114">Not supported.</span></span>|
|<span data-ttu-id="b58f9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b58f9-115">Application</span></span>|<span data-ttu-id="b58f9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b58f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b58f9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b58f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="b58f9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b58f9-118">Request headers</span></span>
|<span data-ttu-id="b58f9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b58f9-119">Header</span></span>|<span data-ttu-id="b58f9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b58f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b58f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b58f9-121">Authorization</span></span>|<span data-ttu-id="b58f9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b58f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b58f9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b58f9-123">Accept</span></span>|<span data-ttu-id="b58f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b58f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b58f9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b58f9-125">Request body</span></span>
<span data-ttu-id="b58f9-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b58f9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b58f9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b58f9-127">Response</span></span>
<span data-ttu-id="b58f9-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b58f9-128">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b58f9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b58f9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b58f9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b58f9-130">Request</span></span>
<span data-ttu-id="b58f9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b58f9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="b58f9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b58f9-132">Response</span></span>
<span data-ttu-id="b58f9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b58f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```




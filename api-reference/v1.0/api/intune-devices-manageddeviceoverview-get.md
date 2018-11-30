---
title: Abrufen von „managedDeviceOverview“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceOverview.
ms.openlocfilehash: b298e99bd0446f3548abf2741e599da9ccebdfe0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017636"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="54833-103">Abrufen von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="54833-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="54833-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54833-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54833-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="54833-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54833-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="54833-106">Prerequisites</span></span>
<span data-ttu-id="54833-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54833-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54833-109">Permission type</span></span>|<span data-ttu-id="54833-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54833-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54833-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54833-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54833-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="54833-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="54833-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54833-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54833-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54833-114">Not supported.</span></span>|
|<span data-ttu-id="54833-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54833-115">Application</span></span>|<span data-ttu-id="54833-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54833-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54833-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="54833-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54833-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="54833-118">Optional query parameters</span></span>
<span data-ttu-id="54833-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="54833-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="54833-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="54833-120">Request headers</span></span>
|<span data-ttu-id="54833-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="54833-121">Header</span></span>|<span data-ttu-id="54833-122">Wert</span><span class="sxs-lookup"><span data-stu-id="54833-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54833-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54833-123">Authorization</span></span>|<span data-ttu-id="54833-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="54833-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54833-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54833-125">Accept</span></span>|<span data-ttu-id="54833-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54833-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54833-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="54833-127">Request body</span></span>
<span data-ttu-id="54833-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="54833-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54833-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="54833-129">Response</span></span>
<span data-ttu-id="54833-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="54833-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54833-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="54833-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="54833-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="54833-132">Request</span></span>
<span data-ttu-id="54833-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="54833-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="54833-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="54833-134">Response</span></span>
<span data-ttu-id="54833-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="54833-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    }
  }
}
```




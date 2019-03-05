---
title: Abrufen von „managedDeviceOverview“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6284ab765df2bfc6060c9b95a76964cfbffa68a5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252420"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="f6942-103">Abrufen von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="f6942-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="f6942-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6942-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6942-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f6942-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6942-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6942-106">Prerequisites</span></span>
<span data-ttu-id="f6942-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6942-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6942-109">Permission type</span></span>|<span data-ttu-id="f6942-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6942-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6942-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6942-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6942-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6942-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f6942-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6942-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6942-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6942-114">Not supported.</span></span>|
|<span data-ttu-id="f6942-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6942-115">Application</span></span>|<span data-ttu-id="f6942-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6942-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6942-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6942-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6942-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6942-118">Optional query parameters</span></span>
<span data-ttu-id="f6942-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6942-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6942-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6942-120">Request headers</span></span>
|<span data-ttu-id="f6942-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6942-121">Header</span></span>|<span data-ttu-id="f6942-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f6942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6942-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6942-123">Authorization</span></span>|<span data-ttu-id="f6942-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6942-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6942-125">Accept</span></span>|<span data-ttu-id="f6942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6942-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6942-127">Request body</span></span>
<span data-ttu-id="f6942-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6942-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6942-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6942-129">Response</span></span>
<span data-ttu-id="f6942-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f6942-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6942-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6942-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6942-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6942-132">Request</span></span>
<span data-ttu-id="f6942-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6942-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="f6942-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6942-134">Response</span></span>
<span data-ttu-id="f6942-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




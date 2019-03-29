---
title: Abrufen von „managedDeviceOverview“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fdbf0b3f7f5f62edd15c0177a9191334e28af92
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979606"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="9f7c4-103">Abrufen von „managedDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="9f7c4-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="9f7c4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f7c4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f7c4-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9f7c4-106">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f7c4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f7c4-107">Prerequisites</span></span>
<span data-ttu-id="9f7c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f7c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f7c4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f7c4-110">Permission type</span></span>|<span data-ttu-id="9f7c4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f7c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f7c4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f7c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f7c4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f7c4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9f7c4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f7c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f7c4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f7c4-115">Not supported.</span></span>|
|<span data-ttu-id="9f7c4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f7c4-116">Application</span></span>|<span data-ttu-id="9f7c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f7c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f7c4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f7c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f7c4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9f7c4-119">Optional query parameters</span></span>
<span data-ttu-id="9f7c4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f7c4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f7c4-121">Request headers</span></span>
|<span data-ttu-id="9f7c4-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f7c4-122">Header</span></span>|<span data-ttu-id="9f7c4-123">Wert</span><span class="sxs-lookup"><span data-stu-id="9f7c4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f7c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f7c4-124">Authorization</span></span>|<span data-ttu-id="9f7c4-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f7c4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f7c4-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f7c4-126">Accept</span></span>|<span data-ttu-id="9f7c4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9f7c4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f7c4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f7c4-128">Request body</span></span>
<span data-ttu-id="9f7c4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f7c4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f7c4-130">Response</span></span>
<span data-ttu-id="9f7c4-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-131">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f7c4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f7c4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f7c4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f7c4-133">Request</span></span>
<span data-ttu-id="9f7c4-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="9f7c4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f7c4-135">Response</span></span>
<span data-ttu-id="9f7c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f7c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1139

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
    },
    "managedDeviceModelsAndManufacturers": {
      "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
      "deviceModels": [
        "Device Models value"
      ],
      "deviceManufacturers": [
        "Device Manufacturers value"
      ]
    },
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





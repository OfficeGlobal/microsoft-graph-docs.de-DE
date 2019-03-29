---
title: Auflisten von „iosUpdateDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosUpdateDeviceStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 681495495892e6d00f692bc8aa6c9afca0706e15
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970618"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="623c5-103">Auflisten von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="623c5-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="623c5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="623c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623c5-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="623c5-105">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="623c5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="623c5-106">Prerequisites</span></span>
<span data-ttu-id="623c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="623c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="623c5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="623c5-109">Permission type</span></span>|<span data-ttu-id="623c5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="623c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="623c5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="623c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="623c5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="623c5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="623c5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="623c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="623c5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="623c5-114">Not supported.</span></span>|
|<span data-ttu-id="623c5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="623c5-115">Application</span></span>|<span data-ttu-id="623c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="623c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="623c5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="623c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="623c5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="623c5-118">Request headers</span></span>
|<span data-ttu-id="623c5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="623c5-119">Header</span></span>|<span data-ttu-id="623c5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="623c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="623c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="623c5-121">Authorization</span></span>|<span data-ttu-id="623c5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="623c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="623c5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="623c5-123">Accept</span></span>|<span data-ttu-id="623c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="623c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="623c5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="623c5-125">Request body</span></span>
<span data-ttu-id="623c5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="623c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="623c5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="623c5-127">Response</span></span>
<span data-ttu-id="623c5-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="623c5-128">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="623c5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="623c5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="623c5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="623c5-130">Request</span></span>
<span data-ttu-id="623c5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="623c5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="623c5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="623c5-132">Response</span></span>
<span data-ttu-id="623c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="623c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




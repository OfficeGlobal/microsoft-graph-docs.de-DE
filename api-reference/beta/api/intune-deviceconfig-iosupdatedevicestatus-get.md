---
title: Abrufen von „iosUpdateDeviceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 082f5f199119a24935a02e4e6de3916516feca1b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962652"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="f6ccc-103">Abrufen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="f6ccc-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="f6ccc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6ccc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ccc-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f6ccc-106">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6ccc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6ccc-107">Prerequisites</span></span>
<span data-ttu-id="f6ccc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6ccc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6ccc-110">Permission type</span></span>|<span data-ttu-id="f6ccc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6ccc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6ccc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6ccc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6ccc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6ccc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6ccc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6ccc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6ccc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6ccc-115">Not supported.</span></span>|
|<span data-ttu-id="f6ccc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6ccc-116">Application</span></span>|<span data-ttu-id="f6ccc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6ccc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6ccc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6ccc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6ccc-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6ccc-119">Optional query parameters</span></span>
<span data-ttu-id="f6ccc-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6ccc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6ccc-121">Request headers</span></span>
|<span data-ttu-id="f6ccc-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6ccc-122">Header</span></span>|<span data-ttu-id="f6ccc-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f6ccc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6ccc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6ccc-124">Authorization</span></span>|<span data-ttu-id="f6ccc-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6ccc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6ccc-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6ccc-126">Accept</span></span>|<span data-ttu-id="f6ccc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6ccc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6ccc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6ccc-128">Request body</span></span>
<span data-ttu-id="f6ccc-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6ccc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6ccc-130">Response</span></span>
<span data-ttu-id="f6ccc-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-131">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6ccc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6ccc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6ccc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6ccc-133">Request</span></span>
<span data-ttu-id="f6ccc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="f6ccc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6ccc-135">Response</span></span>
<span data-ttu-id="f6ccc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6ccc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "63a79499-9499-63a7-9994-a7639994a763",
    "installStatus": "available",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





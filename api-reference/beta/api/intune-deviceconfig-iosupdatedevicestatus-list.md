---
title: Auflisten von „iosUpdateDeviceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosUpdateDeviceStatus auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 66259147312b0174fc00d95d599984723fec352b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403889"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="b829f-103">Auflisten von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="b829f-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="b829f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b829f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b829f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b829f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b829f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b829f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b829f-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b829f-107">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b829f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b829f-108">Prerequisites</span></span>
<span data-ttu-id="b829f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b829f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b829f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b829f-111">Permission type</span></span>|<span data-ttu-id="b829f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b829f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b829f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b829f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b829f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b829f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b829f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b829f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b829f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b829f-116">Not supported.</span></span>|
|<span data-ttu-id="b829f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b829f-117">Application</span></span>|<span data-ttu-id="b829f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b829f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b829f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b829f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b829f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b829f-120">Request headers</span></span>
|<span data-ttu-id="b829f-121">Header</span><span class="sxs-lookup"><span data-stu-id="b829f-121">Header</span></span>|<span data-ttu-id="b829f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b829f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b829f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b829f-123">Authorization</span></span>|<span data-ttu-id="b829f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b829f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b829f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b829f-125">Accept</span></span>|<span data-ttu-id="b829f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b829f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b829f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b829f-127">Request body</span></span>
<span data-ttu-id="b829f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b829f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b829f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b829f-129">Response</span></span>
<span data-ttu-id="b829f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b829f-130">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b829f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b829f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b829f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b829f-132">Request</span></span>
<span data-ttu-id="b829f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b829f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="b829f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b829f-134">Response</span></span>
<span data-ttu-id="b829f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b829f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

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
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





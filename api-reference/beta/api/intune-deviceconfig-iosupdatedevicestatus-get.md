---
title: Abrufen von „iosUpdateDeviceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 679cc7de95f6c70bead957a77b7bcac8a3ae8abe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858744"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="e8dc0-103">Abrufen von „iosUpdateDeviceStatus“</span><span class="sxs-lookup"><span data-stu-id="e8dc0-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="e8dc0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8dc0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8dc0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8dc0-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="e8dc0-107">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8dc0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e8dc0-108">Prerequisites</span></span>
<span data-ttu-id="e8dc0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8dc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8dc0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8dc0-111">Permission type</span></span>|<span data-ttu-id="e8dc0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8dc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8dc0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8dc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8dc0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8dc0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e8dc0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8dc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8dc0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8dc0-116">Not supported.</span></span>|
|<span data-ttu-id="e8dc0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8dc0-117">Application</span></span>|<span data-ttu-id="e8dc0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8dc0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8dc0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8dc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8dc0-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e8dc0-120">Optional query parameters</span></span>
<span data-ttu-id="e8dc0-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8dc0-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8dc0-122">Request headers</span></span>
|<span data-ttu-id="e8dc0-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e8dc0-123">Header</span></span>|<span data-ttu-id="e8dc0-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e8dc0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8dc0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8dc0-125">Authorization</span></span>|<span data-ttu-id="e8dc0-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e8dc0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8dc0-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e8dc0-127">Accept</span></span>|<span data-ttu-id="e8dc0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8dc0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dc0-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8dc0-129">Request body</span></span>
<span data-ttu-id="e8dc0-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8dc0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8dc0-131">Response</span></span>
<span data-ttu-id="e8dc0-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-132">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8dc0-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8dc0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8dc0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8dc0-134">Request</span></span>
<span data-ttu-id="e8dc0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="e8dc0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8dc0-136">Response</span></span>
<span data-ttu-id="e8dc0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






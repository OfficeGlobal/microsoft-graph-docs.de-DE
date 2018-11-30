---
title: Abrufen von „deviceConfigurationDeviceStateSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStateSummary.
ms.openlocfilehash: ca280048ccd880241fab88ab41e82df17a088f64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018237"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="1354b-103">Abrufen von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="1354b-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="1354b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1354b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1354b-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1354b-105">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1354b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1354b-106">Prerequisites</span></span>
<span data-ttu-id="1354b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1354b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1354b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1354b-109">Permission type</span></span>|<span data-ttu-id="1354b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1354b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1354b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1354b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1354b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1354b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1354b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1354b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1354b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1354b-114">Not supported.</span></span>|
|<span data-ttu-id="1354b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1354b-115">Application</span></span>|<span data-ttu-id="1354b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1354b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1354b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1354b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1354b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1354b-118">Optional query parameters</span></span>
<span data-ttu-id="1354b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1354b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1354b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1354b-120">Request headers</span></span>
|<span data-ttu-id="1354b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1354b-121">Header</span></span>|<span data-ttu-id="1354b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1354b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1354b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1354b-123">Authorization</span></span>|<span data-ttu-id="1354b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1354b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1354b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1354b-125">Accept</span></span>|<span data-ttu-id="1354b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1354b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1354b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1354b-127">Request body</span></span>
<span data-ttu-id="1354b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1354b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1354b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1354b-129">Response</span></span>
<span data-ttu-id="1354b-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1354b-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1354b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1354b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1354b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1354b-132">Request</span></span>
<span data-ttu-id="1354b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1354b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="1354b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1354b-134">Response</span></span>
<span data-ttu-id="1354b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1354b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```




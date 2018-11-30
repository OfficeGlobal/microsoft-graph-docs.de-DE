---
title: Abrufen von „softwareUpdateStatusSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs softwareUpdateStatusSummary.
ms.openlocfilehash: f22c63235848bfe86f5ced684c66103a7203bedd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018340"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="bce94-103">Abrufen von „softwareUpdateStatusSummary“</span><span class="sxs-lookup"><span data-stu-id="bce94-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="bce94-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bce94-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bce94-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="bce94-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bce94-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bce94-106">Prerequisites</span></span>
<span data-ttu-id="bce94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bce94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bce94-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bce94-109">Permission type</span></span>|<span data-ttu-id="bce94-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bce94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bce94-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bce94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bce94-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bce94-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bce94-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bce94-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bce94-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bce94-114">Not supported.</span></span>|
|<span data-ttu-id="bce94-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bce94-115">Application</span></span>|<span data-ttu-id="bce94-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bce94-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bce94-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bce94-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bce94-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bce94-118">Optional query parameters</span></span>
<span data-ttu-id="bce94-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bce94-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bce94-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bce94-120">Request headers</span></span>
|<span data-ttu-id="bce94-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bce94-121">Header</span></span>|<span data-ttu-id="bce94-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bce94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bce94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bce94-123">Authorization</span></span>|<span data-ttu-id="bce94-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bce94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bce94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bce94-125">Accept</span></span>|<span data-ttu-id="bce94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bce94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bce94-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bce94-127">Request body</span></span>
<span data-ttu-id="bce94-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bce94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bce94-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bce94-129">Response</span></span>
<span data-ttu-id="bce94-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bce94-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bce94-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bce94-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bce94-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bce94-132">Request</span></span>
<span data-ttu-id="bce94-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bce94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="bce94-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bce94-134">Response</span></span>
<span data-ttu-id="bce94-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bce94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```




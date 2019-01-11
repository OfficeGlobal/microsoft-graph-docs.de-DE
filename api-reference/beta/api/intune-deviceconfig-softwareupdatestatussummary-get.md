---
title: Abrufen von „softwareUpdateStatusSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37b581963e31597869423ee8109f2aaa26bd0dcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847208"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="66ac2-103">Abrufen von „softwareUpdateStatusSummary“</span><span class="sxs-lookup"><span data-stu-id="66ac2-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="66ac2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66ac2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66ac2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66ac2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66ac2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66ac2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66ac2-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="66ac2-107">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66ac2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66ac2-108">Prerequisites</span></span>
<span data-ttu-id="66ac2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66ac2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66ac2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66ac2-111">Permission type</span></span>|<span data-ttu-id="66ac2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66ac2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66ac2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66ac2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66ac2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="66ac2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="66ac2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66ac2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66ac2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66ac2-116">Not supported.</span></span>|
|<span data-ttu-id="66ac2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66ac2-117">Application</span></span>|<span data-ttu-id="66ac2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66ac2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66ac2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66ac2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66ac2-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="66ac2-120">Optional query parameters</span></span>
<span data-ttu-id="66ac2-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66ac2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66ac2-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66ac2-122">Request headers</span></span>
|<span data-ttu-id="66ac2-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66ac2-123">Header</span></span>|<span data-ttu-id="66ac2-124">Wert</span><span class="sxs-lookup"><span data-stu-id="66ac2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66ac2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ac2-125">Authorization</span></span>|<span data-ttu-id="66ac2-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66ac2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66ac2-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66ac2-127">Accept</span></span>|<span data-ttu-id="66ac2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="66ac2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66ac2-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66ac2-129">Request body</span></span>
<span data-ttu-id="66ac2-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66ac2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66ac2-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="66ac2-131">Response</span></span>
<span data-ttu-id="66ac2-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="66ac2-132">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66ac2-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66ac2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="66ac2-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66ac2-134">Request</span></span>
<span data-ttu-id="66ac2-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66ac2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="66ac2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="66ac2-136">Response</span></span>
<span data-ttu-id="66ac2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66ac2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






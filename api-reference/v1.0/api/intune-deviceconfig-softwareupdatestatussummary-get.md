---
title: Abrufen von „softwareUpdateStatusSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 408fcf809d6fc42e0585ed2134c2024d6e0e4675
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967776"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="38905-103">Abrufen von „softwareUpdateStatusSummary“</span><span class="sxs-lookup"><span data-stu-id="38905-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="38905-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="38905-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38905-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="38905-105">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38905-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="38905-106">Prerequisites</span></span>
<span data-ttu-id="38905-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38905-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38905-109">Permission type</span></span>|<span data-ttu-id="38905-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38905-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38905-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38905-111">Delegated (work or school account)</span></span>|<span data-ttu-id="38905-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38905-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38905-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38905-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38905-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38905-114">Not supported.</span></span>|
|<span data-ttu-id="38905-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38905-115">Application</span></span>|<span data-ttu-id="38905-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38905-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38905-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38905-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38905-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="38905-118">Optional query parameters</span></span>
<span data-ttu-id="38905-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="38905-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38905-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38905-120">Request headers</span></span>
|<span data-ttu-id="38905-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="38905-121">Header</span></span>|<span data-ttu-id="38905-122">Wert</span><span class="sxs-lookup"><span data-stu-id="38905-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38905-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38905-123">Authorization</span></span>|<span data-ttu-id="38905-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="38905-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38905-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="38905-125">Accept</span></span>|<span data-ttu-id="38905-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38905-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38905-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38905-127">Request body</span></span>
<span data-ttu-id="38905-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38905-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38905-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="38905-129">Response</span></span>
<span data-ttu-id="38905-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="38905-130">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38905-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38905-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="38905-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38905-132">Request</span></span>
<span data-ttu-id="38905-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38905-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="38905-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="38905-134">Response</span></span>
<span data-ttu-id="38905-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




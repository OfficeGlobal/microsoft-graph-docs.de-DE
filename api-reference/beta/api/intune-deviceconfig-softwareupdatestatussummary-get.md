---
title: Abrufen von „softwareUpdateStatusSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs softwareUpdateStatusSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b189e300d106a472161d7f1df97c1019248527e4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977093"
---
# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="863dd-103">Abrufen von „softwareUpdateStatusSummary“</span><span class="sxs-lookup"><span data-stu-id="863dd-103">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="863dd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="863dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="863dd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="863dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="863dd-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="863dd-106">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="863dd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="863dd-107">Prerequisites</span></span>
<span data-ttu-id="863dd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="863dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="863dd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="863dd-110">Permission type</span></span>|<span data-ttu-id="863dd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="863dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="863dd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="863dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="863dd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="863dd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="863dd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="863dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="863dd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="863dd-115">Not supported.</span></span>|
|<span data-ttu-id="863dd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="863dd-116">Application</span></span>|<span data-ttu-id="863dd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="863dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="863dd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="863dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="863dd-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="863dd-119">Optional query parameters</span></span>
<span data-ttu-id="863dd-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="863dd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="863dd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="863dd-121">Request headers</span></span>
|<span data-ttu-id="863dd-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="863dd-122">Header</span></span>|<span data-ttu-id="863dd-123">Wert</span><span class="sxs-lookup"><span data-stu-id="863dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="863dd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="863dd-124">Authorization</span></span>|<span data-ttu-id="863dd-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="863dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="863dd-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="863dd-126">Accept</span></span>|<span data-ttu-id="863dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="863dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="863dd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="863dd-128">Request body</span></span>
<span data-ttu-id="863dd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="863dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="863dd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="863dd-130">Response</span></span>
<span data-ttu-id="863dd-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="863dd-131">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="863dd-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="863dd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="863dd-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="863dd-133">Request</span></span>
<span data-ttu-id="863dd-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="863dd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="863dd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="863dd-135">Response</span></span>
<span data-ttu-id="863dd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="863dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





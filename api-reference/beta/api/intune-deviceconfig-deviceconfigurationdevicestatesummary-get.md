---
title: Abrufen von „deviceConfigurationDeviceStateSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2baf921584f8cbcdba0ba734f4f512987e26c725
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989106"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="ff291-103">Abrufen von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="ff291-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="ff291-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff291-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff291-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ff291-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff291-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ff291-106">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff291-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff291-107">Prerequisites</span></span>
<span data-ttu-id="ff291-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff291-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff291-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff291-110">Permission type</span></span>|<span data-ttu-id="ff291-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff291-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff291-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff291-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff291-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff291-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff291-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff291-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff291-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff291-115">Not supported.</span></span>|
|<span data-ttu-id="ff291-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff291-116">Application</span></span>|<span data-ttu-id="ff291-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff291-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff291-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff291-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff291-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ff291-119">Optional query parameters</span></span>
<span data-ttu-id="ff291-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff291-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff291-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff291-121">Request headers</span></span>
|<span data-ttu-id="ff291-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff291-122">Header</span></span>|<span data-ttu-id="ff291-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ff291-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff291-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff291-124">Authorization</span></span>|<span data-ttu-id="ff291-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff291-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff291-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff291-126">Accept</span></span>|<span data-ttu-id="ff291-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ff291-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff291-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff291-128">Request body</span></span>
<span data-ttu-id="ff291-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff291-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff291-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff291-130">Response</span></span>
<span data-ttu-id="ff291-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff291-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff291-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff291-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff291-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff291-133">Request</span></span>
<span data-ttu-id="ff291-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff291-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="ff291-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff291-135">Response</span></span>
<span data-ttu-id="ff291-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff291-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





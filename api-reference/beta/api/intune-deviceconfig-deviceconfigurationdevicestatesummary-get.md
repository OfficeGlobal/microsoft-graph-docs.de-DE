---
title: Abrufen von „deviceConfigurationDeviceStateSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationDeviceStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17fd2e19b9a23d20ecbd5c4cb44c01add264009
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401257"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="cafdb-103">Abrufen von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="cafdb-103">Get deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="cafdb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cafdb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cafdb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cafdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cafdb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cafdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cafdb-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cafdb-107">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cafdb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cafdb-108">Prerequisites</span></span>
<span data-ttu-id="cafdb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cafdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cafdb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cafdb-111">Permission type</span></span>|<span data-ttu-id="cafdb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cafdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cafdb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cafdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cafdb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cafdb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cafdb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cafdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cafdb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cafdb-116">Not supported.</span></span>|
|<span data-ttu-id="cafdb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cafdb-117">Application</span></span>|<span data-ttu-id="cafdb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cafdb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cafdb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cafdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cafdb-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cafdb-120">Optional query parameters</span></span>
<span data-ttu-id="cafdb-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cafdb-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cafdb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cafdb-122">Request headers</span></span>
|<span data-ttu-id="cafdb-123">Header</span><span class="sxs-lookup"><span data-stu-id="cafdb-123">Header</span></span>|<span data-ttu-id="cafdb-124">Wert</span><span class="sxs-lookup"><span data-stu-id="cafdb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cafdb-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cafdb-125">Authorization</span></span>|<span data-ttu-id="cafdb-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cafdb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cafdb-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cafdb-127">Accept</span></span>|<span data-ttu-id="cafdb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cafdb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cafdb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cafdb-129">Request body</span></span>
<span data-ttu-id="cafdb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cafdb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cafdb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cafdb-131">Response</span></span>
<span data-ttu-id="cafdb-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cafdb-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafdb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cafdb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cafdb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cafdb-134">Request</span></span>
<span data-ttu-id="cafdb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cafdb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="cafdb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cafdb-136">Response</span></span>
<span data-ttu-id="cafdb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cafdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





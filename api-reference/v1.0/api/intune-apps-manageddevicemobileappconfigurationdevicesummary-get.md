---
title: Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee090d9a263a03e222da2fd338cfe44c9fead47
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974048"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="9c17c-103">Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="9c17c-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="9c17c-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9c17c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c17c-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9c17c-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c17c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c17c-106">Prerequisites</span></span>
<span data-ttu-id="9c17c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c17c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c17c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c17c-109">Permission type</span></span>|<span data-ttu-id="9c17c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c17c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c17c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c17c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c17c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c17c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9c17c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c17c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c17c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c17c-114">Not supported.</span></span>|
|<span data-ttu-id="9c17c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c17c-115">Application</span></span>|<span data-ttu-id="9c17c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c17c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c17c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c17c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c17c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9c17c-118">Optional query parameters</span></span>
<span data-ttu-id="9c17c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c17c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c17c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c17c-120">Request headers</span></span>
|<span data-ttu-id="9c17c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c17c-121">Header</span></span>|<span data-ttu-id="9c17c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9c17c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c17c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c17c-123">Authorization</span></span>|<span data-ttu-id="9c17c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c17c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c17c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c17c-125">Accept</span></span>|<span data-ttu-id="9c17c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c17c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c17c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c17c-127">Request body</span></span>
<span data-ttu-id="9c17c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c17c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c17c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c17c-129">Response</span></span>
<span data-ttu-id="9c17c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c17c-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c17c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c17c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c17c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c17c-132">Request</span></span>
<span data-ttu-id="9c17c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c17c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="9c17c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c17c-134">Response</span></span>
<span data-ttu-id="9c17c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c17c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




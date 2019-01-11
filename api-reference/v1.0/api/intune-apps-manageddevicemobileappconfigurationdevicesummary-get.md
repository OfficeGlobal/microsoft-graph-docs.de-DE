---
title: Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df5a9fbb686f4deaa324c8fdb4858e5b6686e6db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805985"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="70461-103">Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="70461-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="70461-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="70461-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70461-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="70461-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70461-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70461-106">Prerequisites</span></span>
<span data-ttu-id="70461-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70461-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70461-109">Permission type</span></span>|<span data-ttu-id="70461-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70461-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70461-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70461-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70461-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="70461-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="70461-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70461-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70461-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70461-114">Not supported.</span></span>|
|<span data-ttu-id="70461-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70461-115">Application</span></span>|<span data-ttu-id="70461-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70461-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70461-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70461-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70461-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="70461-118">Optional query parameters</span></span>
<span data-ttu-id="70461-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="70461-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70461-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70461-120">Request headers</span></span>
|<span data-ttu-id="70461-121">Header</span><span class="sxs-lookup"><span data-stu-id="70461-121">Header</span></span>|<span data-ttu-id="70461-122">Wert</span><span class="sxs-lookup"><span data-stu-id="70461-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70461-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70461-123">Authorization</span></span>|<span data-ttu-id="70461-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70461-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70461-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70461-125">Accept</span></span>|<span data-ttu-id="70461-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70461-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70461-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70461-127">Request body</span></span>
<span data-ttu-id="70461-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="70461-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70461-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="70461-129">Response</span></span>
<span data-ttu-id="70461-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="70461-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70461-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70461-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="70461-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70461-132">Request</span></span>
<span data-ttu-id="70461-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70461-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="70461-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="70461-134">Response</span></span>
<span data-ttu-id="70461-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70461-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




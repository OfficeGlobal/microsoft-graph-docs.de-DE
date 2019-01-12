---
title: Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a2488cc0a1820dac1cdc020c7d0db86423dfd2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925924"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="273cd-103">Abrufen von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="273cd-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="273cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="273cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="273cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="273cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="273cd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="273cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="273cd-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="273cd-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="273cd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="273cd-108">Prerequisites</span></span>
<span data-ttu-id="273cd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="273cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="273cd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="273cd-111">Permission type</span></span>|<span data-ttu-id="273cd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="273cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="273cd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="273cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="273cd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="273cd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="273cd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="273cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="273cd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="273cd-116">Not supported.</span></span>|
|<span data-ttu-id="273cd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="273cd-117">Application</span></span>|<span data-ttu-id="273cd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="273cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="273cd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="273cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="273cd-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="273cd-120">Optional query parameters</span></span>
<span data-ttu-id="273cd-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="273cd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="273cd-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="273cd-122">Request headers</span></span>
|<span data-ttu-id="273cd-123">Header</span><span class="sxs-lookup"><span data-stu-id="273cd-123">Header</span></span>|<span data-ttu-id="273cd-124">Wert</span><span class="sxs-lookup"><span data-stu-id="273cd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="273cd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="273cd-125">Authorization</span></span>|<span data-ttu-id="273cd-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="273cd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="273cd-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="273cd-127">Accept</span></span>|<span data-ttu-id="273cd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="273cd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="273cd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="273cd-129">Request body</span></span>
<span data-ttu-id="273cd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="273cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="273cd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="273cd-131">Response</span></span>
<span data-ttu-id="273cd-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="273cd-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="273cd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="273cd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="273cd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="273cd-134">Request</span></span>
<span data-ttu-id="273cd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="273cd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="273cd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="273cd-136">Response</span></span>
<span data-ttu-id="273cd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="273cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```






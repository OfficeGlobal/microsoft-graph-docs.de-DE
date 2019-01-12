---
title: deviceConfigurationUserOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0352818b7bb1e864eb42f1ab627c12dcf2634fa5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968155"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="30b49-103">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="30b49-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="30b49-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30b49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30b49-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="30b49-105">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30b49-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="30b49-106">Prerequisites</span></span>
<span data-ttu-id="30b49-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b49-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30b49-109">Permission type</span></span>|<span data-ttu-id="30b49-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30b49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b49-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30b49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30b49-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b49-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30b49-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30b49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b49-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30b49-114">Not supported.</span></span>|
|<span data-ttu-id="30b49-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30b49-115">Application</span></span>|<span data-ttu-id="30b49-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30b49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b49-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30b49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30b49-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="30b49-118">Optional query parameters</span></span>
<span data-ttu-id="30b49-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30b49-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="30b49-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30b49-120">Request headers</span></span>
|<span data-ttu-id="30b49-121">Header</span><span class="sxs-lookup"><span data-stu-id="30b49-121">Header</span></span>|<span data-ttu-id="30b49-122">Wert</span><span class="sxs-lookup"><span data-stu-id="30b49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30b49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30b49-123">Authorization</span></span>|<span data-ttu-id="30b49-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="30b49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30b49-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="30b49-125">Accept</span></span>|<span data-ttu-id="30b49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30b49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b49-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30b49-127">Request body</span></span>
<span data-ttu-id="30b49-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="30b49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30b49-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="30b49-129">Response</span></span>
<span data-ttu-id="30b49-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30b49-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b49-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30b49-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="30b49-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30b49-132">Request</span></span>
<span data-ttu-id="30b49-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30b49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="30b49-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="30b49-134">Response</span></span>
<span data-ttu-id="30b49-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30b49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 368

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
    "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
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




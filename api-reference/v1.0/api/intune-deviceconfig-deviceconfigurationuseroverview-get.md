---
title: deviceConfigurationUserOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserOverview-Objekts.
author: tfitzmac
ms.openlocfilehash: c70c1e188a35222a538db3162bc8272968f16fe5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302142"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="c9783-103">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="c9783-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="c9783-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9783-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9783-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9783-105">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9783-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9783-106">Prerequisites</span></span>
<span data-ttu-id="c9783-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9783-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9783-109">Permission type</span></span>|<span data-ttu-id="c9783-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9783-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9783-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9783-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9783-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9783-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9783-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9783-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9783-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9783-114">Not supported.</span></span>|
|<span data-ttu-id="c9783-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9783-115">Application</span></span>|<span data-ttu-id="c9783-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9783-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9783-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9783-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9783-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c9783-118">Optional query parameters</span></span>
<span data-ttu-id="c9783-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9783-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c9783-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9783-120">Request headers</span></span>
|<span data-ttu-id="c9783-121">Header</span><span class="sxs-lookup"><span data-stu-id="c9783-121">Header</span></span>|<span data-ttu-id="c9783-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c9783-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9783-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c9783-123">Authorization</span></span>|<span data-ttu-id="c9783-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9783-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9783-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9783-125">Accept</span></span>|<span data-ttu-id="c9783-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9783-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9783-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9783-127">Request body</span></span>
<span data-ttu-id="c9783-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9783-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9783-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9783-129">Response</span></span>
<span data-ttu-id="c9783-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9783-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9783-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9783-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9783-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9783-132">Request</span></span>
<span data-ttu-id="c9783-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9783-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="c9783-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9783-134">Response</span></span>
<span data-ttu-id="c9783-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9783-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: deviceConfigurationUserOverview abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserOverview-Objekts.
ms.openlocfilehash: 7aafa1b56b3bb7f308eac87ca95767837b443f81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018365"
---
# <a name="get-deviceconfigurationuseroverview"></a><span data-ttu-id="6814b-103">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="6814b-103">Get deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="6814b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6814b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6814b-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6814b-105">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6814b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6814b-106">Prerequisites</span></span>
<span data-ttu-id="6814b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6814b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6814b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6814b-109">Permission type</span></span>|<span data-ttu-id="6814b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6814b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6814b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6814b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6814b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6814b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6814b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6814b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6814b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6814b-114">Not supported.</span></span>|
|<span data-ttu-id="6814b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6814b-115">Application</span></span>|<span data-ttu-id="6814b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6814b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6814b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6814b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6814b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6814b-118">Optional query parameters</span></span>
<span data-ttu-id="6814b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6814b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6814b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6814b-120">Request headers</span></span>
|<span data-ttu-id="6814b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6814b-121">Header</span></span>|<span data-ttu-id="6814b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6814b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6814b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6814b-123">Authorization</span></span>|<span data-ttu-id="6814b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6814b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6814b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6814b-125">Accept</span></span>|<span data-ttu-id="6814b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6814b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6814b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6814b-127">Request body</span></span>
<span data-ttu-id="6814b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6814b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6814b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6814b-129">Response</span></span>
<span data-ttu-id="6814b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6814b-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6814b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6814b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6814b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6814b-132">Request</span></span>
<span data-ttu-id="6814b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6814b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="6814b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6814b-134">Response</span></span>
<span data-ttu-id="6814b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6814b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



---
title: deviceConfigurationDeviceStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationDeviceStatus-Objekts.
ms.openlocfilehash: 0778884d0d1933e53be6e1cac5fc96b0ba8d5697
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018855"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="f039e-103">deviceConfigurationDeviceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="f039e-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="f039e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f039e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f039e-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f039e-105">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f039e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f039e-106">Prerequisites</span></span>
<span data-ttu-id="f039e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f039e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f039e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f039e-109">Permission type</span></span>|<span data-ttu-id="f039e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f039e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f039e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f039e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f039e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f039e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f039e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f039e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f039e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f039e-114">Not supported.</span></span>|
|<span data-ttu-id="f039e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f039e-115">Application</span></span>|<span data-ttu-id="f039e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f039e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f039e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f039e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f039e-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f039e-118">Optional query parameters</span></span>
<span data-ttu-id="f039e-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f039e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f039e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f039e-120">Request headers</span></span>
|<span data-ttu-id="f039e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f039e-121">Header</span></span>|<span data-ttu-id="f039e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f039e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f039e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f039e-123">Authorization</span></span>|<span data-ttu-id="f039e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f039e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f039e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f039e-125">Accept</span></span>|<span data-ttu-id="f039e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f039e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f039e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f039e-127">Request body</span></span>
<span data-ttu-id="f039e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f039e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f039e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f039e-129">Response</span></span>
<span data-ttu-id="f039e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f039e-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f039e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f039e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f039e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f039e-132">Request</span></span>
<span data-ttu-id="f039e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f039e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="f039e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f039e-134">Response</span></span>
<span data-ttu-id="f039e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f039e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




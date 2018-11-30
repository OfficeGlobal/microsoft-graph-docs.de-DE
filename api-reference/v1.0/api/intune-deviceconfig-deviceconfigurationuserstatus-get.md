---
title: deviceConfigurationUserStatus abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceConfigurationUserStatus-Objekts.
ms.openlocfilehash: 053fa844bb09b9967c95b604fbb2d02d5d5896c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016292"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="d5cb5-103">deviceConfigurationUserStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="d5cb5-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="d5cb5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5cb5-105">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-105">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5cb5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5cb5-106">Prerequisites</span></span>
<span data-ttu-id="d5cb5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5cb5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5cb5-109">Permission type</span></span>|<span data-ttu-id="d5cb5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5cb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5cb5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5cb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5cb5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5cb5-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5cb5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5cb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5cb5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5cb5-114">Not supported.</span></span>|
|<span data-ttu-id="d5cb5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5cb5-115">Application</span></span>|<span data-ttu-id="d5cb5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5cb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5cb5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5cb5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5cb5-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d5cb5-118">Optional query parameters</span></span>
<span data-ttu-id="d5cb5-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d5cb5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5cb5-120">Request headers</span></span>
|<span data-ttu-id="d5cb5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5cb5-121">Header</span></span>|<span data-ttu-id="d5cb5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d5cb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5cb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5cb5-123">Authorization</span></span>|<span data-ttu-id="d5cb5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5cb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5cb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5cb5-125">Accept</span></span>|<span data-ttu-id="d5cb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5cb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5cb5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5cb5-127">Request body</span></span>
<span data-ttu-id="d5cb5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5cb5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5cb5-129">Response</span></span>
<span data-ttu-id="d5cb5-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5cb5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5cb5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5cb5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5cb5-132">Request</span></span>
<span data-ttu-id="d5cb5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="d5cb5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5cb5-134">Response</span></span>
<span data-ttu-id="d5cb5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5cb5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




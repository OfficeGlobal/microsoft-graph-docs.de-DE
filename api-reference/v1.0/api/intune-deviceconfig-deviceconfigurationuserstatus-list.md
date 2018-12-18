---
title: Auflisten von „deviceConfigurationUserStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationUserStatus auf.
author: tfitzmac
ms.openlocfilehash: e34fde4dda174927d7235d5ded4de918f142635d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316702"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="588d3-103">Auflisten von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="588d3-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="588d3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="588d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="588d3-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="588d3-105">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="588d3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="588d3-106">Prerequisites</span></span>
<span data-ttu-id="588d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588d3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="588d3-109">Permission type</span></span>|<span data-ttu-id="588d3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="588d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="588d3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="588d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="588d3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="588d3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="588d3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="588d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="588d3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="588d3-114">Not supported.</span></span>|
|<span data-ttu-id="588d3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="588d3-115">Application</span></span>|<span data-ttu-id="588d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="588d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="588d3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="588d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="588d3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="588d3-118">Request headers</span></span>
|<span data-ttu-id="588d3-119">Header</span><span class="sxs-lookup"><span data-stu-id="588d3-119">Header</span></span>|<span data-ttu-id="588d3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="588d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="588d3-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="588d3-121">Authorization</span></span>|<span data-ttu-id="588d3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="588d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="588d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="588d3-123">Accept</span></span>|<span data-ttu-id="588d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="588d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="588d3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="588d3-125">Request body</span></span>
<span data-ttu-id="588d3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="588d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588d3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="588d3-127">Response</span></span>
<span data-ttu-id="588d3-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="588d3-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588d3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="588d3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="588d3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="588d3-130">Request</span></span>
<span data-ttu-id="588d3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="588d3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="588d3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="588d3-132">Response</span></span>
<span data-ttu-id="588d3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="588d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




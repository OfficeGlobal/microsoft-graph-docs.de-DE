---
title: Auflisten von „deviceInstallState“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceInstallState auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9d85c822bfb4dbd7ee355ace90150a1ab418e242
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839823"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="dd852-103">Auflisten von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="dd852-103">List deviceInstallStates</span></span>

> <span data-ttu-id="dd852-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd852-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd852-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) auf.</span><span class="sxs-lookup"><span data-stu-id="dd852-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd852-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd852-106">Prerequisites</span></span>
<span data-ttu-id="dd852-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd852-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd852-109">Permission type</span></span>|<span data-ttu-id="dd852-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd852-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd852-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd852-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd852-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd852-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd852-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd852-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd852-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd852-114">Not supported.</span></span>|
|<span data-ttu-id="dd852-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd852-115">Application</span></span>|<span data-ttu-id="dd852-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd852-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd852-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd852-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="dd852-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd852-118">Request headers</span></span>
|<span data-ttu-id="dd852-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd852-119">Header</span></span>|<span data-ttu-id="dd852-120">Wert</span><span class="sxs-lookup"><span data-stu-id="dd852-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd852-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd852-121">Authorization</span></span>|<span data-ttu-id="dd852-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd852-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd852-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd852-123">Accept</span></span>|<span data-ttu-id="dd852-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd852-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd852-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd852-125">Request body</span></span>
<span data-ttu-id="dd852-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd852-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd852-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd852-127">Response</span></span>
<span data-ttu-id="dd852-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd852-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd852-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd852-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd852-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd852-130">Request</span></span>
<span data-ttu-id="dd852-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd852-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="dd852-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd852-132">Response</span></span>
<span data-ttu-id="dd852-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd852-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```




---
title: Abrufen von „deviceInstallState“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceInstallState.
ms.openlocfilehash: b2e111b477a4fb7122dd0addf18c167890b2639a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064043"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="39f88-103">Abrufen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="39f88-103">Get deviceInstallState</span></span>

> <span data-ttu-id="39f88-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="39f88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39f88-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39f88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39f88-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39f88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39f88-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="39f88-107">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39f88-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39f88-108">Prerequisites</span></span>
<span data-ttu-id="39f88-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f88-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39f88-111">Permission type</span></span>|<span data-ttu-id="39f88-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39f88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39f88-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39f88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39f88-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="39f88-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="39f88-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39f88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39f88-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f88-116">Not supported.</span></span>|
|<span data-ttu-id="39f88-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39f88-117">Application</span></span>|<span data-ttu-id="39f88-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f88-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39f88-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39f88-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="39f88-120">Optional query parameters</span></span>
<span data-ttu-id="39f88-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39f88-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="39f88-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39f88-122">Request headers</span></span>
|<span data-ttu-id="39f88-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="39f88-123">Header</span></span>|<span data-ttu-id="39f88-124">Wert</span><span class="sxs-lookup"><span data-stu-id="39f88-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39f88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f88-125">Authorization</span></span>|<span data-ttu-id="39f88-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39f88-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39f88-127">Accept</span><span class="sxs-lookup"><span data-stu-id="39f88-127">Accept</span></span>|<span data-ttu-id="39f88-128">application/json</span><span class="sxs-lookup"><span data-stu-id="39f88-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39f88-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39f88-129">Request body</span></span>
<span data-ttu-id="39f88-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39f88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39f88-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f88-131">Response</span></span>
<span data-ttu-id="39f88-132">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `200 OK` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="39f88-132">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f88-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39f88-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="39f88-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f88-134">Request</span></span>
<span data-ttu-id="39f88-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39f88-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="39f88-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f88-136">Response</span></span>
<span data-ttu-id="39f88-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39f88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": {
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
}
```






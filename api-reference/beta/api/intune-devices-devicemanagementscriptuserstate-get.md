---
title: Abrufen von deviceManagementScriptUserState
description: Lesen Sie Eigenschaften und Beziehungen des DeviceManagementScriptUserState-Objekts.
ms.openlocfilehash: d5175a6dc2b5562ac142d505a9a9025c94143bc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065090"
---
# <a name="get-devicemanagementscriptuserstate"></a><span data-ttu-id="9bb75-103">Abrufen von deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="9bb75-103">Get deviceManagementScriptUserState</span></span>

> <span data-ttu-id="9bb75-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bb75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bb75-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bb75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bb75-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9bb75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bb75-107">Lesen Sie Eigenschaften und Beziehungen des [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9bb75-107">Read properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bb75-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9bb75-108">Prerequisites</span></span>
<span data-ttu-id="9bb75-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bb75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bb75-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9bb75-111">Permission type</span></span>|<span data-ttu-id="9bb75-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9bb75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb75-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9bb75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bb75-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bb75-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9bb75-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9bb75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb75-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb75-116">Not supported.</span></span>|
|<span data-ttu-id="9bb75-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9bb75-117">Application</span></span>|<span data-ttu-id="9bb75-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9bb75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb75-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bb75-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9bb75-120">Optional query parameters</span></span>
<span data-ttu-id="9bb75-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9bb75-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9bb75-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9bb75-122">Request headers</span></span>
|<span data-ttu-id="9bb75-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9bb75-123">Header</span></span>|<span data-ttu-id="9bb75-124">Wert</span><span class="sxs-lookup"><span data-stu-id="9bb75-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb75-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb75-125">Authorization</span></span>|<span data-ttu-id="9bb75-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9bb75-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb75-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9bb75-127">Accept</span></span>|<span data-ttu-id="9bb75-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb75-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb75-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9bb75-129">Request body</span></span>
<span data-ttu-id="9bb75-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9bb75-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bb75-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb75-131">Response</span></span>
<span data-ttu-id="9bb75-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9bb75-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb75-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9bb75-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bb75-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9bb75-134">Request</span></span>
<span data-ttu-id="9bb75-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9bb75-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

### <a name="response"></a><span data-ttu-id="9bb75-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9bb75-136">Response</span></span>
<span data-ttu-id="9bb75-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9bb75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 258

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
    "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "userPrincipalName": "User Principal Name value"
  }
}
```






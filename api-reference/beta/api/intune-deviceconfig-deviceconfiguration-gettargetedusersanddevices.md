---
title: GetTargetedUsersAndDevices Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 95d3c93e15c3f52dc80dc55b6afe6e1dd11b9030
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058882"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="350cf-103">GetTargetedUsersAndDevices Aktion</span><span class="sxs-lookup"><span data-stu-id="350cf-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="350cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="350cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="350cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="350cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="350cf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="350cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="350cf-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="350cf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="350cf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="350cf-108">Prerequisites</span></span>
<span data-ttu-id="350cf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="350cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="350cf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="350cf-111">Permission type</span></span>|<span data-ttu-id="350cf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="350cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="350cf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="350cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="350cf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="350cf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="350cf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="350cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="350cf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="350cf-116">Not supported.</span></span>|
|<span data-ttu-id="350cf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="350cf-117">Application</span></span>|<span data-ttu-id="350cf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="350cf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="350cf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="350cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="350cf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="350cf-120">Request headers</span></span>
|<span data-ttu-id="350cf-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="350cf-121">Header</span></span>|<span data-ttu-id="350cf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="350cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="350cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="350cf-123">Authorization</span></span>|<span data-ttu-id="350cf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="350cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="350cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="350cf-125">Accept</span></span>|<span data-ttu-id="350cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="350cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="350cf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="350cf-127">Request body</span></span>
<span data-ttu-id="350cf-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="350cf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="350cf-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="350cf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="350cf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="350cf-130">Property</span></span>|<span data-ttu-id="350cf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="350cf-131">Type</span></span>|<span data-ttu-id="350cf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="350cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="350cf-133">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="350cf-133">deviceConfigurationIds</span></span>|<span data-ttu-id="350cf-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="350cf-134">String collection</span></span>|<span data-ttu-id="350cf-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="350cf-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="350cf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="350cf-136">Response</span></span>
<span data-ttu-id="350cf-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [DeviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="350cf-137">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="350cf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="350cf-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="350cf-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="350cf-139">Request</span></span>
<span data-ttu-id="350cf-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="350cf-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="350cf-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="350cf-141">Response</span></span>
<span data-ttu-id="350cf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="350cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```






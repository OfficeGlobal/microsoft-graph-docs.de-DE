---
title: getTargetedUsersAndDevices-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26aa7a56d3f7baec060f52c0c3bbb67fa011f83d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171162"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="7c7be-103">getTargetedUsersAndDevices-Aktion</span><span class="sxs-lookup"><span data-stu-id="7c7be-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="7c7be-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c7be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c7be-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7c7be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c7be-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7c7be-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c7be-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c7be-107">Prerequisites</span></span>
<span data-ttu-id="7c7be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c7be-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c7be-110">Permission type</span></span>|<span data-ttu-id="7c7be-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c7be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c7be-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c7be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c7be-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c7be-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c7be-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c7be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c7be-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c7be-115">Not supported.</span></span>|
|<span data-ttu-id="7c7be-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c7be-116">Application</span></span>|<span data-ttu-id="7c7be-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c7be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c7be-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c7be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="7c7be-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c7be-119">Request headers</span></span>
|<span data-ttu-id="7c7be-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c7be-120">Header</span></span>|<span data-ttu-id="7c7be-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7c7be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c7be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c7be-122">Authorization</span></span>|<span data-ttu-id="7c7be-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c7be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c7be-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c7be-124">Accept</span></span>|<span data-ttu-id="7c7be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c7be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c7be-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c7be-126">Request body</span></span>
<span data-ttu-id="7c7be-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="7c7be-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7c7be-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7c7be-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7c7be-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7c7be-129">Property</span></span>|<span data-ttu-id="7c7be-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7c7be-130">Type</span></span>|<span data-ttu-id="7c7be-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c7be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c7be-132">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="7c7be-132">deviceConfigurationIds</span></span>|<span data-ttu-id="7c7be-133">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7c7be-133">String collection</span></span>|<span data-ttu-id="7c7be-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="7c7be-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c7be-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c7be-135">Response</span></span>
<span data-ttu-id="7c7be-136">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c7be-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c7be-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c7be-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c7be-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c7be-138">Request</span></span>
<span data-ttu-id="7c7be-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c7be-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c7be-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c7be-140">Response</span></span>
<span data-ttu-id="7c7be-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c7be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





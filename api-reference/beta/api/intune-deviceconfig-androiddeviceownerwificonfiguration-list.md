---
title: Liste androidDeviceOwnerWiFiConfigurations
description: Listeneigenschaften und Beziehungen der AndroidDeviceOwnerWiFiConfiguration-Objekte.
author: tfitzmac
ms.openlocfilehash: 5fd46f7f2de0477c94d7e5afe042bf7a891dc4e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312796"
---
# <a name="list-androiddeviceownerwificonfigurations"></a><span data-ttu-id="edfdb-103">Liste androidDeviceOwnerWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="edfdb-103">List androidDeviceOwnerWiFiConfigurations</span></span>

> <span data-ttu-id="edfdb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="edfdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edfdb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="edfdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edfdb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="edfdb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edfdb-107">Listeneigenschaften und Beziehungen der [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="edfdb-107">List properties and relationships of the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edfdb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="edfdb-108">Prerequisites</span></span>
<span data-ttu-id="edfdb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edfdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edfdb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="edfdb-111">Permission type</span></span>|<span data-ttu-id="edfdb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="edfdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edfdb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="edfdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edfdb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="edfdb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="edfdb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="edfdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edfdb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="edfdb-116">Not supported.</span></span>|
|<span data-ttu-id="edfdb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="edfdb-117">Application</span></span>|<span data-ttu-id="edfdb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="edfdb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edfdb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="edfdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="edfdb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="edfdb-120">Request headers</span></span>
|<span data-ttu-id="edfdb-121">Header</span><span class="sxs-lookup"><span data-stu-id="edfdb-121">Header</span></span>|<span data-ttu-id="edfdb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="edfdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edfdb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="edfdb-123">Authorization</span></span>|<span data-ttu-id="edfdb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="edfdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edfdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="edfdb-125">Accept</span></span>|<span data-ttu-id="edfdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edfdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edfdb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="edfdb-127">Request body</span></span>
<span data-ttu-id="edfdb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="edfdb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edfdb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="edfdb-129">Response</span></span>
<span data-ttu-id="edfdb-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="edfdb-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edfdb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="edfdb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="edfdb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="edfdb-132">Request</span></span>
<span data-ttu-id="edfdb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="edfdb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="edfdb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="edfdb-134">Response</span></span>
<span data-ttu-id="edfdb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="edfdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
      "id": "8d25beba-beba-8d25-babe-258dbabe258d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wep",
      "preSharedKey": "Pre Shared Key value",
      "preSharedKeyIsSet": true
    }
  ]
}
```






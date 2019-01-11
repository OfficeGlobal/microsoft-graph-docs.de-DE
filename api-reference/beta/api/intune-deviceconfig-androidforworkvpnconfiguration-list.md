---
title: Liste androidForWorkVpnConfigurations
description: Listeneigenschaften und Beziehungen der AndroidForWorkVpnConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81816923c27d604b9002c49e88ed573a4e126713
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817500"
---
# <a name="list-androidforworkvpnconfigurations"></a><span data-ttu-id="33c96-103">Liste androidForWorkVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="33c96-103">List androidForWorkVpnConfigurations</span></span>

> <span data-ttu-id="33c96-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33c96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33c96-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33c96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33c96-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33c96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33c96-107">Listeneigenschaften und Beziehungen der [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="33c96-107">List properties and relationships of the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33c96-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33c96-108">Prerequisites</span></span>
<span data-ttu-id="33c96-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33c96-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33c96-111">Permission type</span></span>|<span data-ttu-id="33c96-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33c96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33c96-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33c96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33c96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33c96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33c96-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33c96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33c96-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33c96-116">Not supported.</span></span>|
|<span data-ttu-id="33c96-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33c96-117">Application</span></span>|<span data-ttu-id="33c96-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33c96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33c96-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33c96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33c96-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33c96-120">Request headers</span></span>
|<span data-ttu-id="33c96-121">Header</span><span class="sxs-lookup"><span data-stu-id="33c96-121">Header</span></span>|<span data-ttu-id="33c96-122">Wert</span><span class="sxs-lookup"><span data-stu-id="33c96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33c96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33c96-123">Authorization</span></span>|<span data-ttu-id="33c96-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33c96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33c96-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33c96-125">Accept</span></span>|<span data-ttu-id="33c96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33c96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33c96-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33c96-127">Request body</span></span>
<span data-ttu-id="33c96-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="33c96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33c96-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="33c96-129">Response</span></span>
<span data-ttu-id="33c96-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="33c96-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33c96-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33c96-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="33c96-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33c96-132">Request</span></span>
<span data-ttu-id="33c96-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33c96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="33c96-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="33c96-134">Response</span></span>
<span data-ttu-id="33c96-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33c96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1346

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
      "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "role": "Role value",
      "realm": "Realm value",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "fingerprint": "Fingerprint value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "authenticationMethod": "usernameAndPassword"
    }
  ]
}
```






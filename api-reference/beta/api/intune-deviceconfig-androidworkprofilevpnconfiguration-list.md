---
title: AndroidWorkProfileVpnConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidWorkProfileVpnConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 700739c0d20706519217586ab466c388d274f1f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171953"
---
# <a name="list-androidworkprofilevpnconfigurations"></a><span data-ttu-id="699f6-103">AndroidWorkProfileVpnConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="699f6-103">List androidWorkProfileVpnConfigurations</span></span>

> <span data-ttu-id="699f6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="699f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="699f6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="699f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="699f6-106">AufListen von Eigenschaften und Beziehungen der [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="699f6-106">List properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="699f6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="699f6-107">Prerequisites</span></span>
<span data-ttu-id="699f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="699f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="699f6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="699f6-110">Permission type</span></span>|<span data-ttu-id="699f6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="699f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="699f6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="699f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="699f6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="699f6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="699f6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="699f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="699f6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="699f6-115">Not supported.</span></span>|
|<span data-ttu-id="699f6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="699f6-116">Application</span></span>|<span data-ttu-id="699f6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="699f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="699f6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="699f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="699f6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="699f6-119">Request headers</span></span>
|<span data-ttu-id="699f6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="699f6-120">Header</span></span>|<span data-ttu-id="699f6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="699f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="699f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="699f6-122">Authorization</span></span>|<span data-ttu-id="699f6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="699f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="699f6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="699f6-124">Accept</span></span>|<span data-ttu-id="699f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="699f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="699f6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="699f6-126">Request body</span></span>
<span data-ttu-id="699f6-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="699f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="699f6-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="699f6-128">Response</span></span>
<span data-ttu-id="699f6-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="699f6-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="699f6-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="699f6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="699f6-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="699f6-131">Request</span></span>
<span data-ttu-id="699f6-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="699f6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="699f6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="699f6-133">Response</span></span>
<span data-ttu-id="699f6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="699f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1350

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
      "id": "32910378-0378-3291-7803-913278039132",
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





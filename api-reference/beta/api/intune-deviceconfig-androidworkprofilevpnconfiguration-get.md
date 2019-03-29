---
title: AndroidWorkProfileVpnConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des androidWorkProfileVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ac2945b519d108044c4d6f74e1f587d077fdd1d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972725"
---
# <a name="get-androidworkprofilevpnconfiguration"></a><span data-ttu-id="5fef0-103">AndroidWorkProfileVpnConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="5fef0-103">Get androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="5fef0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5fef0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fef0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5fef0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fef0-106">Lesen von Eigenschaften und Beziehungen des [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5fef0-106">Read properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fef0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5fef0-107">Prerequisites</span></span>
<span data-ttu-id="5fef0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fef0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fef0-110">Permission type</span></span>|<span data-ttu-id="5fef0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fef0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fef0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fef0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fef0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fef0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5fef0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fef0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fef0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fef0-115">Not supported.</span></span>|
|<span data-ttu-id="5fef0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fef0-116">Application</span></span>|<span data-ttu-id="5fef0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fef0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fef0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fef0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fef0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5fef0-119">Optional query parameters</span></span>
<span data-ttu-id="5fef0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5fef0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fef0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fef0-121">Request headers</span></span>
|<span data-ttu-id="5fef0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5fef0-122">Header</span></span>|<span data-ttu-id="5fef0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5fef0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fef0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fef0-124">Authorization</span></span>|<span data-ttu-id="5fef0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5fef0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fef0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5fef0-126">Accept</span></span>|<span data-ttu-id="5fef0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5fef0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fef0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fef0-128">Request body</span></span>
<span data-ttu-id="5fef0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5fef0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fef0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fef0-130">Response</span></span>
<span data-ttu-id="5fef0-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5fef0-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fef0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fef0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fef0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fef0-133">Request</span></span>
<span data-ttu-id="5fef0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fef0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5fef0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fef0-135">Response</span></span>
<span data-ttu-id="5fef0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fef0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1258

{
  "value": {
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
}
```





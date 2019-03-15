---
title: IosLobAppProvisioningConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosLobAppProvisioningConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 667ea00d6cf689f45196bd4fbefb9438c2ff9590
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571858"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="e3eee-103">IosLobAppProvisioningConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="e3eee-103">Get iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="e3eee-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3eee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3eee-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3eee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3eee-106">Lesen von Eigenschaften und Beziehungen des [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3eee-106">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3eee-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3eee-107">Prerequisites</span></span>
<span data-ttu-id="e3eee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3eee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3eee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3eee-110">Permission type</span></span>|<span data-ttu-id="e3eee-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3eee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3eee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3eee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3eee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3eee-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3eee-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3eee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3eee-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3eee-115">Not supported.</span></span>|
|<span data-ttu-id="e3eee-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3eee-116">Application</span></span>|<span data-ttu-id="e3eee-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3eee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3eee-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3eee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3eee-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e3eee-119">Optional query parameters</span></span>
<span data-ttu-id="e3eee-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3eee-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3eee-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3eee-121">Request headers</span></span>
|<span data-ttu-id="e3eee-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3eee-122">Header</span></span>|<span data-ttu-id="e3eee-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e3eee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3eee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3eee-124">Authorization</span></span>|<span data-ttu-id="e3eee-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3eee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3eee-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3eee-126">Accept</span></span>|<span data-ttu-id="e3eee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e3eee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3eee-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3eee-128">Request body</span></span>
<span data-ttu-id="e3eee-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3eee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3eee-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3eee-130">Response</span></span>
<span data-ttu-id="e3eee-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3eee-131">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3eee-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3eee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3eee-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3eee-133">Request</span></span>
<span data-ttu-id="e3eee-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3eee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e3eee-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3eee-135">Response</span></span>
<span data-ttu-id="e3eee-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3eee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
    "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA==",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```





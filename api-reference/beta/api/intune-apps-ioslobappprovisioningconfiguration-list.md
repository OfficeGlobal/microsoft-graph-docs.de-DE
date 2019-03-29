---
title: IosLobAppProvisioningConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der iosLobAppProvisioningConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3e9a82886a8d16634572d1f64172d7cee5fff9e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984940"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="0a64a-103">IosLobAppProvisioningConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="0a64a-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="0a64a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a64a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a64a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0a64a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a64a-106">AufListen von Eigenschaften und Beziehungen der [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0a64a-106">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a64a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0a64a-107">Prerequisites</span></span>
<span data-ttu-id="0a64a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a64a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a64a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a64a-110">Permission type</span></span>|<span data-ttu-id="0a64a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a64a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a64a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a64a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a64a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a64a-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a64a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a64a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a64a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a64a-115">Not supported.</span></span>|
|<span data-ttu-id="0a64a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a64a-116">Application</span></span>|<span data-ttu-id="0a64a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a64a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a64a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a64a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a64a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a64a-119">Request headers</span></span>
|<span data-ttu-id="0a64a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0a64a-120">Header</span></span>|<span data-ttu-id="0a64a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0a64a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a64a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a64a-122">Authorization</span></span>|<span data-ttu-id="0a64a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a64a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a64a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0a64a-124">Accept</span></span>|<span data-ttu-id="0a64a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a64a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a64a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a64a-126">Request body</span></span>
<span data-ttu-id="0a64a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0a64a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a64a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a64a-128">Response</span></span>
<span data-ttu-id="0a64a-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0a64a-129">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a64a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a64a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a64a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a64a-131">Request</span></span>
<span data-ttu-id="0a64a-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a64a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="0a64a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a64a-133">Response</span></span>
<span data-ttu-id="0a64a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a64a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 632

{
  "value": [
    {
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
  ]
}
```





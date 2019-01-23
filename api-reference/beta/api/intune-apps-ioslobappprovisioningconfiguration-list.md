---
title: Liste iosLobAppProvisioningConfigurations
description: Listeneigenschaften und Beziehungen der IosLobAppProvisioningConfiguration-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f26b0a5c0bd2161693a29be5c5ed5e1409f8bbc6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397799"
---
# <a name="list-ioslobappprovisioningconfigurations"></a><span data-ttu-id="0f937-103">Liste iosLobAppProvisioningConfigurations</span><span class="sxs-lookup"><span data-stu-id="0f937-103">List iosLobAppProvisioningConfigurations</span></span>

> <span data-ttu-id="0f937-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f937-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f937-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f937-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f937-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f937-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f937-107">Listeneigenschaften und Beziehungen der [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0f937-107">List properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f937-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f937-108">Prerequisites</span></span>
<span data-ttu-id="0f937-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f937-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f937-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f937-111">Permission type</span></span>|<span data-ttu-id="0f937-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f937-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f937-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f937-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f937-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f937-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0f937-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f937-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f937-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f937-116">Not supported.</span></span>|
|<span data-ttu-id="0f937-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f937-117">Application</span></span>|<span data-ttu-id="0f937-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f937-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f937-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f937-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0f937-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f937-120">Request headers</span></span>
|<span data-ttu-id="0f937-121">Header</span><span class="sxs-lookup"><span data-stu-id="0f937-121">Header</span></span>|<span data-ttu-id="0f937-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0f937-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f937-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0f937-123">Authorization</span></span>|<span data-ttu-id="0f937-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f937-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f937-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f937-125">Accept</span></span>|<span data-ttu-id="0f937-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f937-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f937-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f937-127">Request body</span></span>
<span data-ttu-id="0f937-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f937-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f937-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f937-129">Response</span></span>
<span data-ttu-id="0f937-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0f937-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f937-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f937-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f937-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f937-132">Request</span></span>
<span data-ttu-id="0f937-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f937-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
```

### <a name="response"></a><span data-ttu-id="0f937-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f937-134">Response</span></span>
<span data-ttu-id="0f937-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f937-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
      "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA==",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```





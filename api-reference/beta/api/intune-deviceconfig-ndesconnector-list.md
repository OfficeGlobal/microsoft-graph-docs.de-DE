---
title: NdesConnectors aufListen
description: AufListen von Eigenschaften und Beziehungen der ndesConnector-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ec5bf0a02f3b4ceb58dc0a27ecfecea14d8f7e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160382"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="d240c-103">NdesConnectors aufListen</span><span class="sxs-lookup"><span data-stu-id="d240c-103">List ndesConnectors</span></span>

> <span data-ttu-id="d240c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d240c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d240c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d240c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d240c-106">AufListen von Eigenschaften und Beziehungen der [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d240c-106">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d240c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d240c-107">Prerequisites</span></span>
<span data-ttu-id="d240c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d240c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d240c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d240c-110">Permission type</span></span>|<span data-ttu-id="d240c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d240c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d240c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d240c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d240c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d240c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d240c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d240c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d240c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d240c-115">Not supported.</span></span>|
|<span data-ttu-id="d240c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d240c-116">Application</span></span>|<span data-ttu-id="d240c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d240c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d240c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d240c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d240c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d240c-119">Request headers</span></span>
|<span data-ttu-id="d240c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d240c-120">Header</span></span>|<span data-ttu-id="d240c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d240c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d240c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d240c-122">Authorization</span></span>|<span data-ttu-id="d240c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d240c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d240c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d240c-124">Accept</span></span>|<span data-ttu-id="d240c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d240c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d240c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d240c-126">Request body</span></span>
<span data-ttu-id="d240c-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d240c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d240c-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d240c-128">Response</span></span>
<span data-ttu-id="d240c-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d240c-129">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d240c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d240c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d240c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d240c-131">Request</span></span>
<span data-ttu-id="d240c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d240c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="d240c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d240c-133">Response</span></span>
<span data-ttu-id="d240c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d240c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```





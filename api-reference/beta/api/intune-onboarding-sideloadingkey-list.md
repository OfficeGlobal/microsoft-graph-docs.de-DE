---
title: SideLoadingKeies aufListen
description: AufListen von Eigenschaften und Beziehungen der sideLoadingKey-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3bf543c678815e563dd9607b56483084183a99a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143232"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="915ac-103">SideLoadingKeies aufListen</span><span class="sxs-lookup"><span data-stu-id="915ac-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="915ac-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="915ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="915ac-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="915ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="915ac-106">AufListen von Eigenschaften und Beziehungen der [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="915ac-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="915ac-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="915ac-107">Prerequisites</span></span>
<span data-ttu-id="915ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="915ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="915ac-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="915ac-110">Permission type</span></span>|<span data-ttu-id="915ac-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="915ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="915ac-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="915ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="915ac-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="915ac-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="915ac-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="915ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="915ac-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="915ac-115">Not supported.</span></span>|
|<span data-ttu-id="915ac-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="915ac-116">Application</span></span>|<span data-ttu-id="915ac-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="915ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="915ac-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="915ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="915ac-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="915ac-119">Request headers</span></span>
|<span data-ttu-id="915ac-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="915ac-120">Header</span></span>|<span data-ttu-id="915ac-121">Wert</span><span class="sxs-lookup"><span data-stu-id="915ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="915ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="915ac-122">Authorization</span></span>|<span data-ttu-id="915ac-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="915ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="915ac-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="915ac-124">Accept</span></span>|<span data-ttu-id="915ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="915ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="915ac-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="915ac-126">Request body</span></span>
<span data-ttu-id="915ac-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="915ac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="915ac-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="915ac-128">Response</span></span>
<span data-ttu-id="915ac-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="915ac-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="915ac-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="915ac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="915ac-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="915ac-131">Request</span></span>
<span data-ttu-id="915ac-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="915ac-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="915ac-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="915ac-133">Response</span></span>
<span data-ttu-id="915ac-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="915ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```





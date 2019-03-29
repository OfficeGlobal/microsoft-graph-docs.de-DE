---
title: EmbeddedSIMActivationCodePoolAssignments aufListen
description: AufListen von Eigenschaften und Beziehungen der embeddedSIMActivationCodePoolAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2595adcfd070a0e48819bde8e9a3747dcdbf901f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958214"
---
# <a name="list-embeddedsimactivationcodepoolassignments"></a><span data-ttu-id="2c243-103">EmbeddedSIMActivationCodePoolAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="2c243-103">List embeddedSIMActivationCodePoolAssignments</span></span>

> <span data-ttu-id="2c243-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c243-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2c243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c243-106">AufListen von Eigenschaften und Beziehungen der [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2c243-106">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c243-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2c243-107">Prerequisites</span></span>
<span data-ttu-id="2c243-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c243-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c243-110">Permission type</span></span>|<span data-ttu-id="2c243-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c243-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c243-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c243-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c243-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c243-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2c243-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c243-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c243-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c243-115">Not supported.</span></span>|
|<span data-ttu-id="2c243-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c243-116">Application</span></span>|<span data-ttu-id="2c243-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c243-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c243-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c243-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2c243-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c243-119">Request headers</span></span>
|<span data-ttu-id="2c243-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2c243-120">Header</span></span>|<span data-ttu-id="2c243-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2c243-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c243-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c243-122">Authorization</span></span>|<span data-ttu-id="2c243-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2c243-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c243-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2c243-124">Accept</span></span>|<span data-ttu-id="2c243-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c243-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c243-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c243-126">Request body</span></span>
<span data-ttu-id="2c243-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2c243-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c243-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c243-128">Response</span></span>
<span data-ttu-id="2c243-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2c243-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c243-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c243-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c243-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c243-131">Request</span></span>
<span data-ttu-id="2c243-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c243-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

### <a name="response"></a><span data-ttu-id="2c243-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c243-133">Response</span></span>
<span data-ttu-id="2c243-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c243-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
      "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





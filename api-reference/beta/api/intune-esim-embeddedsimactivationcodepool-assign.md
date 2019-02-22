---
title: Aktion zuweisen
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eef7f430df82c41f506078564e38dc7efad39e0c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145577"
---
# <a name="assign-action"></a><span data-ttu-id="1d4d7-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="1d4d7-103">assign action</span></span>

> <span data-ttu-id="1d4d7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d4d7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d4d7-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1d4d7-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d4d7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d4d7-107">Prerequisites</span></span>
<span data-ttu-id="1d4d7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d4d7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d4d7-110">Permission type</span></span>|<span data-ttu-id="1d4d7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d4d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4d7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d4d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d4d7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d4d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4d7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d4d7-115">Not supported.</span></span>|
|<span data-ttu-id="1d4d7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d4d7-116">Application</span></span>|<span data-ttu-id="1d4d7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d4d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4d7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d4d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1d4d7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d4d7-119">Request headers</span></span>
|<span data-ttu-id="1d4d7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1d4d7-120">Header</span></span>|<span data-ttu-id="1d4d7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1d4d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d4d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4d7-122">Authorization</span></span>|<span data-ttu-id="1d4d7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d4d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d4d7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1d4d7-124">Accept</span></span>|<span data-ttu-id="1d4d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d4d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4d7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d4d7-126">Request body</span></span>
<span data-ttu-id="1d4d7-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1d4d7-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1d4d7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d4d7-129">Property</span></span>|<span data-ttu-id="1d4d7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1d4d7-130">Type</span></span>|<span data-ttu-id="1d4d7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d4d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4d7-132">assignments</span><span class="sxs-lookup"><span data-stu-id="1d4d7-132">assignments</span></span>|<span data-ttu-id="1d4d7-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="1d4d7-133">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="1d4d7-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1d4d7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d4d7-135">Response</span></span>
<span data-ttu-id="1d4d7-136">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-136">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4d7-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d4d7-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d4d7-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d4d7-138">Request</span></span>
<span data-ttu-id="1d4d7-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign

Content-type: application/json
Content-length: 287

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="1d4d7-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d4d7-140">Response</span></span>
<span data-ttu-id="1d4d7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d4d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





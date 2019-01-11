---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 54a4689c5317ae4df1044cf2d8ca262189a357c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848930"
---
# <a name="assign-action"></a><span data-ttu-id="7b4d4-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="7b4d4-103">assign action</span></span>

> <span data-ttu-id="7b4d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b4d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b4d4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b4d4-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7b4d4-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b4d4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b4d4-108">Prerequisites</span></span>
<span data-ttu-id="7b4d4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b4d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b4d4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b4d4-111">Permission type</span></span>|<span data-ttu-id="7b4d4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b4d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b4d4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b4d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b4d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b4d4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b4d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b4d4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b4d4-116">Not supported.</span></span>|
|<span data-ttu-id="7b4d4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b4d4-117">Application</span></span>|<span data-ttu-id="7b4d4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b4d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b4d4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b4d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7b4d4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b4d4-120">Request headers</span></span>
|<span data-ttu-id="7b4d4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b4d4-121">Header</span></span>|<span data-ttu-id="7b4d4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7b4d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b4d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b4d4-123">Authorization</span></span>|<span data-ttu-id="7b4d4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b4d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b4d4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b4d4-125">Accept</span></span>|<span data-ttu-id="7b4d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b4d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b4d4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b4d4-127">Request body</span></span>
<span data-ttu-id="7b4d4-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7b4d4-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7b4d4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b4d4-130">Property</span></span>|<span data-ttu-id="7b4d4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7b4d4-131">Type</span></span>|<span data-ttu-id="7b4d4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b4d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b4d4-133">assignments</span><span class="sxs-lookup"><span data-stu-id="7b4d4-133">assignments</span></span>|<span data-ttu-id="7b4d4-134">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7b4d4-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="7b4d4-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7b4d4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7b4d4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b4d4-136">Response</span></span>
<span data-ttu-id="7b4d4-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b4d4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b4d4-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b4d4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b4d4-139">Request</span></span>
<span data-ttu-id="7b4d4-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b4d4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b4d4-141">Response</span></span>
<span data-ttu-id="7b4d4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b4d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






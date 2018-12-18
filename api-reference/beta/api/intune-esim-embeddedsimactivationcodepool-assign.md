---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 88b6b7eef26e0187bacf2ee647c95452a1642cba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316107"
---
# <a name="assign-action"></a><span data-ttu-id="c0244-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="c0244-103">assign action</span></span>

> <span data-ttu-id="c0244-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0244-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0244-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0244-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0244-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0244-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0244-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c0244-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0244-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0244-108">Prerequisites</span></span>
<span data-ttu-id="c0244-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0244-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0244-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0244-111">Permission type</span></span>|<span data-ttu-id="c0244-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0244-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0244-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0244-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0244-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0244-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0244-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0244-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0244-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0244-116">Not supported.</span></span>|
|<span data-ttu-id="c0244-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0244-117">Application</span></span>|<span data-ttu-id="c0244-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0244-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0244-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0244-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c0244-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0244-120">Request headers</span></span>
|<span data-ttu-id="c0244-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0244-121">Header</span></span>|<span data-ttu-id="c0244-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0244-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0244-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c0244-123">Authorization</span></span>|<span data-ttu-id="c0244-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0244-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0244-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0244-125">Accept</span></span>|<span data-ttu-id="c0244-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0244-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0244-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0244-127">Request body</span></span>
<span data-ttu-id="c0244-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="c0244-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c0244-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c0244-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c0244-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c0244-130">Property</span></span>|<span data-ttu-id="c0244-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c0244-131">Type</span></span>|<span data-ttu-id="c0244-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0244-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0244-133">assignments</span><span class="sxs-lookup"><span data-stu-id="c0244-133">assignments</span></span>|<span data-ttu-id="c0244-134">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c0244-134">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="c0244-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c0244-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c0244-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0244-136">Response</span></span>
<span data-ttu-id="c0244-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c0244-137">If successful, this action returns a `200 OK` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0244-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0244-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0244-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0244-139">Request</span></span>
<span data-ttu-id="c0244-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0244-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0244-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0244-141">Response</span></span>
<span data-ttu-id="c0244-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0244-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






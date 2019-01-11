---
title: Aktion „assign“
description: Ersetzen Sie alle Gruppen für eine Richtlinie.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b41ce4ec1c6e304168aebb4c53b4512b0a11f4b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858667"
---
# <a name="assign-action"></a><span data-ttu-id="0af85-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="0af85-103">assign action</span></span>

> <span data-ttu-id="0af85-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0af85-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0af85-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0af85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0af85-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0af85-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0af85-107">Ersetzen Sie alle Gruppen für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="0af85-107">Replace all targeted groups for a policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0af85-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0af85-108">Prerequisites</span></span>
<span data-ttu-id="0af85-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af85-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0af85-111">Permission type</span></span>|<span data-ttu-id="0af85-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0af85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0af85-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0af85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0af85-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af85-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0af85-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0af85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0af85-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0af85-116">Not supported.</span></span>|
|<span data-ttu-id="0af85-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0af85-117">Application</span></span>|<span data-ttu-id="0af85-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0af85-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0af85-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0af85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0af85-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0af85-120">Request headers</span></span>
|<span data-ttu-id="0af85-121">Header</span><span class="sxs-lookup"><span data-stu-id="0af85-121">Header</span></span>|<span data-ttu-id="0af85-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0af85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0af85-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af85-123">Authorization</span></span>|<span data-ttu-id="0af85-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0af85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0af85-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0af85-125">Accept</span></span>|<span data-ttu-id="0af85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0af85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af85-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0af85-127">Request body</span></span>
<span data-ttu-id="0af85-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="0af85-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0af85-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="0af85-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0af85-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0af85-130">Property</span></span>|<span data-ttu-id="0af85-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0af85-131">Type</span></span>|<span data-ttu-id="0af85-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0af85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af85-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="0af85-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="0af85-134">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0af85-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0af85-135">Liste der Zuordnungen für Office-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="0af85-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="0af85-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0af85-136">Response</span></span>
<span data-ttu-id="0af85-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0af85-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af85-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0af85-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="0af85-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0af85-139">Request</span></span>
<span data-ttu-id="0af85-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0af85-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign

Content-type: application/json
Content-length: 299

{
  "officeConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0af85-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="0af85-141">Response</span></span>
<span data-ttu-id="0af85-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0af85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```




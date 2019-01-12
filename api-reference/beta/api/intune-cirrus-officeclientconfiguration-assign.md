---
title: Aktion „assign“
description: Ersetzen Sie alle Gruppen für eine Richtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0dc9a3fb0ed7b941d8ebc8d37c9a69e605f0804b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964004"
---
# <a name="assign-action"></a><span data-ttu-id="4bccf-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="4bccf-103">assign action</span></span>

> <span data-ttu-id="4bccf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4bccf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bccf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4bccf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bccf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4bccf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bccf-107">Ersetzen Sie alle Gruppen für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="4bccf-107">Replace all targeted groups for a policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bccf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4bccf-108">Prerequisites</span></span>
<span data-ttu-id="4bccf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bccf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bccf-111">Permission type</span></span>|<span data-ttu-id="4bccf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bccf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bccf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bccf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bccf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bccf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bccf-116">Not supported.</span></span>|
|<span data-ttu-id="4bccf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bccf-117">Application</span></span>|<span data-ttu-id="4bccf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bccf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bccf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4bccf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bccf-120">Request headers</span></span>
|<span data-ttu-id="4bccf-121">Header</span><span class="sxs-lookup"><span data-stu-id="4bccf-121">Header</span></span>|<span data-ttu-id="4bccf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4bccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bccf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bccf-123">Authorization</span></span>|<span data-ttu-id="4bccf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4bccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bccf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4bccf-125">Accept</span></span>|<span data-ttu-id="4bccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bccf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bccf-127">Request body</span></span>
<span data-ttu-id="4bccf-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4bccf-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4bccf-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4bccf-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4bccf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4bccf-130">Property</span></span>|<span data-ttu-id="4bccf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4bccf-131">Type</span></span>|<span data-ttu-id="4bccf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bccf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bccf-133">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="4bccf-133">officeConfigurationAssignments</span></span>|<span data-ttu-id="4bccf-134">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4bccf-134">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4bccf-135">Liste der Zuordnungen für Office-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="4bccf-135">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="4bccf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bccf-136">Response</span></span>
<span data-ttu-id="4bccf-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4bccf-137">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bccf-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bccf-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bccf-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bccf-139">Request</span></span>
<span data-ttu-id="4bccf-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4bccf-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4bccf-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bccf-141">Response</span></span>
<span data-ttu-id="4bccf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bccf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




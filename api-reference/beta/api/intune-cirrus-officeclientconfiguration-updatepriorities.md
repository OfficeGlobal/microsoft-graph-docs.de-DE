---
title: UpdatePriorities Aktion
description: Aktualisieren Sie die Richtlinie Prioritäten.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 15c57de2077842ff2115770859fc34357e0f6a22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940477"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="26e8b-103">UpdatePriorities Aktion</span><span class="sxs-lookup"><span data-stu-id="26e8b-103">updatePriorities action</span></span>

> <span data-ttu-id="26e8b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="26e8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e8b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26e8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26e8b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="26e8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26e8b-107">Aktualisieren Sie die Richtlinie Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="26e8b-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26e8b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="26e8b-108">Prerequisites</span></span>
<span data-ttu-id="26e8b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e8b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="26e8b-111">Permission type</span></span>|<span data-ttu-id="26e8b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="26e8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e8b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="26e8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e8b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e8b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26e8b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="26e8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e8b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26e8b-116">Not supported.</span></span>|
|<span data-ttu-id="26e8b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="26e8b-117">Application</span></span>|<span data-ttu-id="26e8b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="26e8b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e8b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="26e8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="26e8b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="26e8b-120">Request headers</span></span>
|<span data-ttu-id="26e8b-121">Header</span><span class="sxs-lookup"><span data-stu-id="26e8b-121">Header</span></span>|<span data-ttu-id="26e8b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="26e8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26e8b-123">Authorization</span></span>|<span data-ttu-id="26e8b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="26e8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e8b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="26e8b-125">Accept</span></span>|<span data-ttu-id="26e8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e8b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="26e8b-127">Request body</span></span>
<span data-ttu-id="26e8b-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="26e8b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="26e8b-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="26e8b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26e8b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26e8b-130">Property</span></span>|<span data-ttu-id="26e8b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="26e8b-131">Type</span></span>|<span data-ttu-id="26e8b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26e8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e8b-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="26e8b-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="26e8b-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="26e8b-134">String collection</span></span>|<span data-ttu-id="26e8b-135">Liste der Office-Konfiguration Richtlinie-ids</span><span class="sxs-lookup"><span data-stu-id="26e8b-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="26e8b-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="26e8b-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="26e8b-137">Int32-Auflistung</span><span class="sxs-lookup"><span data-stu-id="26e8b-137">Int32 collection</span></span>|<span data-ttu-id="26e8b-138">Liste der Prioritäten für Office-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="26e8b-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="26e8b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="26e8b-139">Response</span></span>
<span data-ttu-id="26e8b-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="26e8b-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26e8b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="26e8b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="26e8b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="26e8b-142">Request</span></span>
<span data-ttu-id="26e8b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="26e8b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities

Content-type: application/json
Content-length: 143

{
  "officeConfigurationPolicyIds": [
    "Office Configuration Policy Ids value"
  ],
  "officeConfigurationPriorities": [
    13
  ]
}
```

### <a name="response"></a><span data-ttu-id="26e8b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="26e8b-144">Response</span></span>
<span data-ttu-id="26e8b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="26e8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




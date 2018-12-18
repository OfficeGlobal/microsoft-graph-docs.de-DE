---
title: UpdatePriorities Aktion
description: Aktualisieren Sie die Richtlinie Prioritäten.
author: tfitzmac
ms.openlocfilehash: d8c493200d5ed1c0e6eb2228a1e74337237e73e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302590"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="68715-103">UpdatePriorities Aktion</span><span class="sxs-lookup"><span data-stu-id="68715-103">updatePriorities action</span></span>

> <span data-ttu-id="68715-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="68715-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68715-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68715-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68715-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="68715-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68715-107">Aktualisieren Sie die Richtlinie Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="68715-107">Update policy priorities.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68715-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="68715-108">Prerequisites</span></span>
<span data-ttu-id="68715-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68715-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68715-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68715-111">Permission type</span></span>|<span data-ttu-id="68715-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68715-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68715-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68715-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68715-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68715-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68715-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68715-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68715-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68715-116">Not supported.</span></span>|
|<span data-ttu-id="68715-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68715-117">Application</span></span>|<span data-ttu-id="68715-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68715-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68715-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68715-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="68715-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68715-120">Request headers</span></span>
|<span data-ttu-id="68715-121">Header</span><span class="sxs-lookup"><span data-stu-id="68715-121">Header</span></span>|<span data-ttu-id="68715-122">Wert</span><span class="sxs-lookup"><span data-stu-id="68715-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68715-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="68715-123">Authorization</span></span>|<span data-ttu-id="68715-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="68715-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68715-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68715-125">Accept</span></span>|<span data-ttu-id="68715-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68715-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68715-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68715-127">Request body</span></span>
<span data-ttu-id="68715-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="68715-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="68715-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="68715-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="68715-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68715-130">Property</span></span>|<span data-ttu-id="68715-131">Typ</span><span class="sxs-lookup"><span data-stu-id="68715-131">Type</span></span>|<span data-ttu-id="68715-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68715-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68715-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="68715-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="68715-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="68715-134">String collection</span></span>|<span data-ttu-id="68715-135">Liste der Office-Konfiguration Richtlinie-ids</span><span class="sxs-lookup"><span data-stu-id="68715-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="68715-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="68715-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="68715-137">Int32-Auflistung</span><span class="sxs-lookup"><span data-stu-id="68715-137">Int32 collection</span></span>|<span data-ttu-id="68715-138">Liste der Prioritäten für Office-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="68715-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="68715-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="68715-139">Response</span></span>
<span data-ttu-id="68715-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="68715-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68715-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68715-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="68715-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68715-142">Request</span></span>
<span data-ttu-id="68715-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68715-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68715-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="68715-144">Response</span></span>
<span data-ttu-id="68715-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68715-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




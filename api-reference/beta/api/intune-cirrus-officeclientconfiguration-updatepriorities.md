---
title: updatePriorities-Aktion
description: Aktualisieren der Richtlinien Prioritäten.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6422cd3f40270f6502a58551e6c5c1b739219e00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154992"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="5b344-103">updatePriorities-Aktion</span><span class="sxs-lookup"><span data-stu-id="5b344-103">updatePriorities action</span></span>

> <span data-ttu-id="5b344-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b344-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b344-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5b344-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b344-106">Aktualisieren der Richtlinien Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="5b344-106">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b344-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b344-107">Prerequisites</span></span>
<span data-ttu-id="5b344-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b344-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b344-110">Permission type</span></span>|<span data-ttu-id="5b344-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b344-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b344-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b344-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b344-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b344-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b344-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b344-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b344-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b344-115">Not supported.</span></span>|
|<span data-ttu-id="5b344-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b344-116">Application</span></span>|<span data-ttu-id="5b344-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b344-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b344-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b344-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="5b344-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b344-119">Request headers</span></span>
|<span data-ttu-id="5b344-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b344-120">Header</span></span>|<span data-ttu-id="5b344-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5b344-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b344-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b344-122">Authorization</span></span>|<span data-ttu-id="5b344-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b344-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b344-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b344-124">Accept</span></span>|<span data-ttu-id="5b344-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b344-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b344-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b344-126">Request body</span></span>
<span data-ttu-id="5b344-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="5b344-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5b344-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5b344-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5b344-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b344-129">Property</span></span>|<span data-ttu-id="5b344-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5b344-130">Type</span></span>|<span data-ttu-id="5b344-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b344-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b344-132">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="5b344-132">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="5b344-133">String collection</span><span class="sxs-lookup"><span data-stu-id="5b344-133">String collection</span></span>|<span data-ttu-id="5b344-134">Liste der Office-Konfigurationsrichtlinien-IDs</span><span class="sxs-lookup"><span data-stu-id="5b344-134">List of office configuration policy ids</span></span>|
|<span data-ttu-id="5b344-135">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="5b344-135">officeConfigurationPriorities</span></span>|<span data-ttu-id="5b344-136">Int32-Auflistung</span><span class="sxs-lookup"><span data-stu-id="5b344-136">Int32 collection</span></span>|<span data-ttu-id="5b344-137">Liste der Office-Konfigurations Prioritäten</span><span class="sxs-lookup"><span data-stu-id="5b344-137">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="5b344-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b344-138">Response</span></span>
<span data-ttu-id="5b344-139">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="5b344-139">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5b344-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b344-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b344-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b344-141">Request</span></span>
<span data-ttu-id="5b344-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b344-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b344-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b344-143">Response</span></span>
<span data-ttu-id="5b344-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b344-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




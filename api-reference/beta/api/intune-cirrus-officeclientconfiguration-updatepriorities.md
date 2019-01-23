---
title: UpdatePriorities Aktion
description: Aktualisieren Sie die Richtlinie Prioritäten.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a78ec2801522354709643dfdd88da0e6dd9756c8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412975"
---
# <a name="updatepriorities-action"></a><span data-ttu-id="c5117-103">UpdatePriorities Aktion</span><span class="sxs-lookup"><span data-stu-id="c5117-103">updatePriorities action</span></span>

> <span data-ttu-id="c5117-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c5117-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5117-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5117-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5117-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5117-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5117-107">Aktualisieren Sie die Richtlinie Prioritäten.</span><span class="sxs-lookup"><span data-stu-id="c5117-107">Update policy priorities.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5117-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5117-108">Prerequisites</span></span>
<span data-ttu-id="c5117-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5117-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5117-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5117-111">Permission type</span></span>|<span data-ttu-id="c5117-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5117-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5117-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5117-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5117-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5117-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5117-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5117-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5117-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5117-116">Not supported.</span></span>|
|<span data-ttu-id="c5117-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5117-117">Application</span></span>|<span data-ttu-id="c5117-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5117-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5117-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5117-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/microsoft.management.services.api.updatePriorities
```

## <a name="request-headers"></a><span data-ttu-id="c5117-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5117-120">Request headers</span></span>
|<span data-ttu-id="c5117-121">Header</span><span class="sxs-lookup"><span data-stu-id="c5117-121">Header</span></span>|<span data-ttu-id="c5117-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c5117-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5117-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c5117-123">Authorization</span></span>|<span data-ttu-id="c5117-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5117-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5117-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5117-125">Accept</span></span>|<span data-ttu-id="c5117-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5117-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5117-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5117-127">Request body</span></span>
<span data-ttu-id="c5117-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="c5117-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c5117-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c5117-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c5117-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5117-130">Property</span></span>|<span data-ttu-id="c5117-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c5117-131">Type</span></span>|<span data-ttu-id="c5117-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5117-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5117-133">officeConfigurationPolicyIds</span><span class="sxs-lookup"><span data-stu-id="c5117-133">officeConfigurationPolicyIds</span></span>|<span data-ttu-id="c5117-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c5117-134">String collection</span></span>|<span data-ttu-id="c5117-135">Liste der Office-Konfiguration Richtlinie-ids</span><span class="sxs-lookup"><span data-stu-id="c5117-135">List of office configuration policy ids</span></span>|
|<span data-ttu-id="c5117-136">officeConfigurationPriorities</span><span class="sxs-lookup"><span data-stu-id="c5117-136">officeConfigurationPriorities</span></span>|<span data-ttu-id="c5117-137">Int32-Auflistung</span><span class="sxs-lookup"><span data-stu-id="c5117-137">Int32 collection</span></span>|<span data-ttu-id="c5117-138">Liste der Prioritäten für Office-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="c5117-138">List of office configuration priorities</span></span>|



## <a name="response"></a><span data-ttu-id="c5117-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5117-139">Response</span></span>
<span data-ttu-id="c5117-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` zurück.</span><span class="sxs-lookup"><span data-stu-id="c5117-140">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5117-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5117-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5117-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5117-142">Request</span></span>
<span data-ttu-id="c5117-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5117-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5117-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5117-144">Response</span></span>
<span data-ttu-id="c5117-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5117-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




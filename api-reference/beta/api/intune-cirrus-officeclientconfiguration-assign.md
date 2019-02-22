---
title: Aktion zuweisen
description: Ersetzen Sie alle Zielgruppen für eine Richtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b6dfde86fe1163ea7cb9f86720a979c79e99671c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145661"
---
# <a name="assign-action"></a><span data-ttu-id="36d7e-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="36d7e-103">assign action</span></span>

> <span data-ttu-id="36d7e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36d7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36d7e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="36d7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d7e-106">Ersetzen Sie alle Zielgruppen für eine Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="36d7e-106">Replace all targeted groups for a policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36d7e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36d7e-107">Prerequisites</span></span>
<span data-ttu-id="36d7e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36d7e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36d7e-110">Permission type</span></span>|<span data-ttu-id="36d7e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36d7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36d7e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36d7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36d7e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36d7e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36d7e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36d7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36d7e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36d7e-115">Not supported.</span></span>|
|<span data-ttu-id="36d7e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36d7e-116">Application</span></span>|<span data-ttu-id="36d7e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36d7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36d7e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36d7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="36d7e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36d7e-119">Request headers</span></span>
|<span data-ttu-id="36d7e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="36d7e-120">Header</span></span>|<span data-ttu-id="36d7e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="36d7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36d7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36d7e-122">Authorization</span></span>|<span data-ttu-id="36d7e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36d7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36d7e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36d7e-124">Accept</span></span>|<span data-ttu-id="36d7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36d7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d7e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36d7e-126">Request body</span></span>
<span data-ttu-id="36d7e-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="36d7e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="36d7e-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="36d7e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="36d7e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36d7e-129">Property</span></span>|<span data-ttu-id="36d7e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="36d7e-130">Type</span></span>|<span data-ttu-id="36d7e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36d7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36d7e-132">officeConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="36d7e-132">officeConfigurationAssignments</span></span>|<span data-ttu-id="36d7e-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="36d7e-133">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="36d7e-134">Liste der Office-Konfigurations Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="36d7e-134">List of office configuration assignments</span></span>|



## <a name="response"></a><span data-ttu-id="36d7e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="36d7e-135">Response</span></span>
<span data-ttu-id="36d7e-136">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="36d7e-136">If successful, this action returns a `200 OK` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d7e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36d7e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="36d7e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36d7e-138">Request</span></span>
<span data-ttu-id="36d7e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36d7e-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36d7e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="36d7e-140">Response</span></span>
<span data-ttu-id="36d7e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36d7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




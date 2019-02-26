---
title: Aktion zuweisen
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4cf7440dd856731a0079ce7781b4c9c05d932d9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151653"
---
# <a name="assign-action"></a><span data-ttu-id="de142-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="de142-103">assign action</span></span>

> <span data-ttu-id="de142-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="de142-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de142-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="de142-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de142-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="de142-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de142-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de142-107">Prerequisites</span></span>
<span data-ttu-id="de142-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="de142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="de142-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de142-110">Permission type</span></span>|<span data-ttu-id="de142-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de142-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de142-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de142-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de142-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de142-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de142-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de142-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de142-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de142-115">Not supported.</span></span>|
|<span data-ttu-id="de142-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de142-116">Application</span></span>|<span data-ttu-id="de142-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de142-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de142-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de142-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="de142-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de142-119">Request headers</span></span>
|<span data-ttu-id="de142-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de142-120">Header</span></span>|<span data-ttu-id="de142-121">Wert</span><span class="sxs-lookup"><span data-stu-id="de142-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de142-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de142-122">Authorization</span></span>|<span data-ttu-id="de142-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de142-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de142-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de142-124">Accept</span></span>|<span data-ttu-id="de142-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de142-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de142-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de142-126">Request body</span></span>
<span data-ttu-id="de142-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="de142-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="de142-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="de142-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="de142-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de142-129">Property</span></span>|<span data-ttu-id="de142-130">Typ</span><span class="sxs-lookup"><span data-stu-id="de142-130">Type</span></span>|<span data-ttu-id="de142-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de142-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de142-132">assignments</span><span class="sxs-lookup"><span data-stu-id="de142-132">assignments</span></span>|<span data-ttu-id="de142-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="de142-133">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="de142-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="de142-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de142-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="de142-135">Response</span></span>
<span data-ttu-id="de142-136">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="de142-136">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de142-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de142-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="de142-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de142-138">Request</span></span>
<span data-ttu-id="de142-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de142-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="de142-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="de142-140">Response</span></span>
<span data-ttu-id="de142-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de142-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





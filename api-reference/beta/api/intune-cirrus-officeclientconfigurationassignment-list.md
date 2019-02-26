---
title: OfficeClientConfigurationAssignments aufListen
description: AufListen von Eigenschaften und Beziehungen der officeClientConfigurationAssignment-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc0e458e9912b5da7a00c1dfc8814c48457a9b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157582"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="47dae-103">OfficeClientConfigurationAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="47dae-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="47dae-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47dae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47dae-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="47dae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47dae-106">AufListen von Eigenschaften und Beziehungen der [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="47dae-106">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47dae-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47dae-107">Prerequisites</span></span>
<span data-ttu-id="47dae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47dae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47dae-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47dae-110">Permission type</span></span>|<span data-ttu-id="47dae-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47dae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47dae-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47dae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47dae-113">\* \* TODO: Bestimmen von Bereichen \* \*</span><span class="sxs-lookup"><span data-stu-id="47dae-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="47dae-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47dae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47dae-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47dae-115">Not supported.</span></span>|
|<span data-ttu-id="47dae-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47dae-116">Application</span></span>|<span data-ttu-id="47dae-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47dae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47dae-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47dae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="47dae-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47dae-119">Request headers</span></span>
|<span data-ttu-id="47dae-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47dae-120">Header</span></span>|<span data-ttu-id="47dae-121">Wert</span><span class="sxs-lookup"><span data-stu-id="47dae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47dae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47dae-122">Authorization</span></span>|<span data-ttu-id="47dae-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47dae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47dae-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47dae-124">Accept</span></span>|<span data-ttu-id="47dae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47dae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47dae-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47dae-126">Request body</span></span>
<span data-ttu-id="47dae-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47dae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47dae-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="47dae-128">Response</span></span>
<span data-ttu-id="47dae-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47dae-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47dae-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47dae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="47dae-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47dae-131">Request</span></span>
<span data-ttu-id="47dae-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47dae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="47dae-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="47dae-133">Response</span></span>
<span data-ttu-id="47dae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47dae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




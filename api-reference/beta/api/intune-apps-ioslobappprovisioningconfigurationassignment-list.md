---
title: IosLobAppProvisioningConfigurationAssignments aufListen
description: AufListen von Eigenschaften und Beziehungen der iosLobAppProvisioningConfigurationAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cf3755a54d3ad7c3a09c2342640a783a4a131ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170539"
---
# <a name="list-ioslobappprovisioningconfigurationassignments"></a><span data-ttu-id="9f033-103">IosLobAppProvisioningConfigurationAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="9f033-103">List iosLobAppProvisioningConfigurationAssignments</span></span>

> <span data-ttu-id="9f033-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f033-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f033-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9f033-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f033-106">AufListen von Eigenschaften und Beziehungen der [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9f033-106">List properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f033-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f033-107">Prerequisites</span></span>
<span data-ttu-id="9f033-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f033-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f033-110">Permission type</span></span>|<span data-ttu-id="9f033-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f033-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f033-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f033-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f033-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f033-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f033-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f033-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f033-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f033-115">Not supported.</span></span>|
|<span data-ttu-id="9f033-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f033-116">Application</span></span>|<span data-ttu-id="9f033-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f033-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f033-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f033-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9f033-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f033-119">Request headers</span></span>
|<span data-ttu-id="9f033-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f033-120">Header</span></span>|<span data-ttu-id="9f033-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9f033-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f033-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f033-122">Authorization</span></span>|<span data-ttu-id="9f033-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f033-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f033-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f033-124">Accept</span></span>|<span data-ttu-id="9f033-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f033-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f033-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f033-126">Request body</span></span>
<span data-ttu-id="9f033-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f033-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f033-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f033-128">Response</span></span>
<span data-ttu-id="9f033-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9f033-129">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f033-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f033-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f033-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f033-131">Request</span></span>
<span data-ttu-id="9f033-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f033-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="9f033-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f033-133">Response</span></span>
<span data-ttu-id="9f033-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f033-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





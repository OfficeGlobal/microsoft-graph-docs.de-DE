---
title: Liste iosLobAppProvisioningConfigurationAssignments
description: Listeneigenschaften und Beziehungen der IosLobAppProvisioningConfigurationAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41230396c73ac1682b639488da733a497381e017
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823877"
---
# <a name="list-ioslobappprovisioningconfigurationassignments"></a><span data-ttu-id="58816-103">Liste iosLobAppProvisioningConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="58816-103">List iosLobAppProvisioningConfigurationAssignments</span></span>

> <span data-ttu-id="58816-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="58816-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58816-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58816-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58816-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="58816-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58816-107">Listeneigenschaften und Beziehungen der [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="58816-107">List properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58816-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58816-108">Prerequisites</span></span>
<span data-ttu-id="58816-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58816-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58816-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58816-111">Permission type</span></span>|<span data-ttu-id="58816-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58816-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58816-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58816-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58816-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58816-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58816-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58816-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58816-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58816-116">Not supported.</span></span>|
|<span data-ttu-id="58816-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58816-117">Application</span></span>|<span data-ttu-id="58816-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58816-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58816-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58816-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="58816-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58816-120">Request headers</span></span>
|<span data-ttu-id="58816-121">Header</span><span class="sxs-lookup"><span data-stu-id="58816-121">Header</span></span>|<span data-ttu-id="58816-122">Wert</span><span class="sxs-lookup"><span data-stu-id="58816-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58816-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58816-123">Authorization</span></span>|<span data-ttu-id="58816-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58816-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58816-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58816-125">Accept</span></span>|<span data-ttu-id="58816-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58816-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58816-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58816-127">Request body</span></span>
<span data-ttu-id="58816-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="58816-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58816-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="58816-129">Response</span></span>
<span data-ttu-id="58816-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="58816-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58816-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58816-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="58816-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58816-132">Request</span></span>
<span data-ttu-id="58816-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58816-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="58816-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="58816-134">Response</span></span>
<span data-ttu-id="58816-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58816-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






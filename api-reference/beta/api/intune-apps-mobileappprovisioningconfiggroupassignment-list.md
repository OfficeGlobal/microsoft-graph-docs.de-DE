---
title: Liste mobileAppProvisioningConfigGroupAssignments
description: Listeneigenschaften und Beziehungen der MobileAppProvisioningConfigGroupAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d34b005a246ae5f896f80800cf176047bce4954c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854558"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="342bc-103">Liste mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="342bc-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="342bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="342bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="342bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="342bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="342bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="342bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="342bc-107">Listeneigenschaften und Beziehungen der [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="342bc-107">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="342bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="342bc-108">Prerequisites</span></span>
<span data-ttu-id="342bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="342bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="342bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="342bc-111">Permission type</span></span>|<span data-ttu-id="342bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="342bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="342bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="342bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="342bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="342bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="342bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="342bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="342bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="342bc-116">Not supported.</span></span>|
|<span data-ttu-id="342bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="342bc-117">Application</span></span>|<span data-ttu-id="342bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="342bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="342bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="342bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="342bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="342bc-120">Request headers</span></span>
|<span data-ttu-id="342bc-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="342bc-121">Header</span></span>|<span data-ttu-id="342bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="342bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="342bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="342bc-123">Authorization</span></span>|<span data-ttu-id="342bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="342bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="342bc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="342bc-125">Accept</span></span>|<span data-ttu-id="342bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="342bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="342bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="342bc-127">Request body</span></span>
<span data-ttu-id="342bc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="342bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="342bc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="342bc-129">Response</span></span>
<span data-ttu-id="342bc-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="342bc-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="342bc-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="342bc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="342bc-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="342bc-132">Request</span></span>
<span data-ttu-id="342bc-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="342bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="342bc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="342bc-134">Response</span></span>
<span data-ttu-id="342bc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="342bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```






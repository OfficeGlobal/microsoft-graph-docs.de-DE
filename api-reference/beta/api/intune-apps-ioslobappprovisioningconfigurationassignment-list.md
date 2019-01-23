---
title: Liste iosLobAppProvisioningConfigurationAssignments
description: Listeneigenschaften und Beziehungen der IosLobAppProvisioningConfigurationAssignment-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c177e97d0d55cd728cb5909acbaedf889078642
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409531"
---
# <a name="list-ioslobappprovisioningconfigurationassignments"></a><span data-ttu-id="efbc7-103">Liste iosLobAppProvisioningConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="efbc7-103">List iosLobAppProvisioningConfigurationAssignments</span></span>

> <span data-ttu-id="efbc7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="efbc7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="efbc7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efbc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efbc7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="efbc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efbc7-107">Listeneigenschaften und Beziehungen der [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="efbc7-107">List properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efbc7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="efbc7-108">Prerequisites</span></span>
<span data-ttu-id="efbc7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="efbc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="efbc7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efbc7-111">Permission type</span></span>|<span data-ttu-id="efbc7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efbc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efbc7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efbc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efbc7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="efbc7-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="efbc7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efbc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efbc7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efbc7-116">Not supported.</span></span>|
|<span data-ttu-id="efbc7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efbc7-117">Application</span></span>|<span data-ttu-id="efbc7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efbc7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efbc7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efbc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="efbc7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="efbc7-120">Request headers</span></span>
|<span data-ttu-id="efbc7-121">Header</span><span class="sxs-lookup"><span data-stu-id="efbc7-121">Header</span></span>|<span data-ttu-id="efbc7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="efbc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efbc7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="efbc7-123">Authorization</span></span>|<span data-ttu-id="efbc7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="efbc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efbc7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="efbc7-125">Accept</span></span>|<span data-ttu-id="efbc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efbc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efbc7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="efbc7-127">Request body</span></span>
<span data-ttu-id="efbc7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="efbc7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efbc7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="efbc7-129">Response</span></span>
<span data-ttu-id="efbc7-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="efbc7-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efbc7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efbc7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="efbc7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efbc7-132">Request</span></span>
<span data-ttu-id="efbc7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="efbc7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="efbc7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="efbc7-134">Response</span></span>
<span data-ttu-id="efbc7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efbc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





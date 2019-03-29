---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30ac71a5cd3d1b8f53608e924f9c964012f28493
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963485"
---
# <a name="assign-action"></a><span data-ttu-id="73e79-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="73e79-103">assign action</span></span>

> <span data-ttu-id="73e79-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73e79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73e79-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="73e79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73e79-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="73e79-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73e79-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73e79-107">Prerequisites</span></span>
<span data-ttu-id="73e79-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e79-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73e79-110">Permission type</span></span>|<span data-ttu-id="73e79-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73e79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73e79-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73e79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73e79-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73e79-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73e79-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73e79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73e79-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73e79-115">Not supported.</span></span>|
|<span data-ttu-id="73e79-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73e79-116">Application</span></span>|<span data-ttu-id="73e79-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73e79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73e79-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73e79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="73e79-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73e79-119">Request headers</span></span>
|<span data-ttu-id="73e79-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73e79-120">Header</span></span>|<span data-ttu-id="73e79-121">Wert</span><span class="sxs-lookup"><span data-stu-id="73e79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73e79-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73e79-122">Authorization</span></span>|<span data-ttu-id="73e79-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73e79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73e79-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73e79-124">Accept</span></span>|<span data-ttu-id="73e79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73e79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73e79-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73e79-126">Request body</span></span>
<span data-ttu-id="73e79-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="73e79-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="73e79-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="73e79-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="73e79-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73e79-129">Property</span></span>|<span data-ttu-id="73e79-130">Typ</span><span class="sxs-lookup"><span data-stu-id="73e79-130">Type</span></span>|<span data-ttu-id="73e79-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73e79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73e79-132">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="73e79-132">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="73e79-133">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="73e79-133">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="73e79-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="73e79-134">Not yet documented</span></span>|
|<span data-ttu-id="73e79-135">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="73e79-135">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="73e79-136">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="73e79-136">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="73e79-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="73e79-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="73e79-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="73e79-138">Response</span></span>
<span data-ttu-id="73e79-139">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73e79-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73e79-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73e79-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="73e79-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73e79-141">Request</span></span>
<span data-ttu-id="73e79-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73e79-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign

Content-type: application/json
Content-length: 578

{
  "appProvisioningConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ],
  "iOSLobAppProvisioningConfigAssignments": [
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

### <a name="response"></a><span data-ttu-id="73e79-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="73e79-143">Response</span></span>
<span data-ttu-id="73e79-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73e79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





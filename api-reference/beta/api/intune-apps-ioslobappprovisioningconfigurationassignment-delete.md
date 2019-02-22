---
title: IosLobAppProvisioningConfigurationAssignment löschen
description: Löscht eine iosLobAppProvisioningConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c390b5c2baa9fc395e6cd0dd8a1501add10ea1db
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153109"
---
# <a name="delete-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="5cf59-103">IosLobAppProvisioningConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="5cf59-103">Delete iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="5cf59-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5cf59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cf59-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5cf59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cf59-106">Löscht eine [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5cf59-106">Deletes a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cf59-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5cf59-107">Prerequisites</span></span>
<span data-ttu-id="5cf59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5cf59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cf59-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5cf59-110">Permission type</span></span>|<span data-ttu-id="5cf59-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5cf59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cf59-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5cf59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5cf59-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cf59-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cf59-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5cf59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cf59-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cf59-115">Not supported.</span></span>|
|<span data-ttu-id="5cf59-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5cf59-116">Application</span></span>|<span data-ttu-id="5cf59-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cf59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cf59-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cf59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5cf59-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5cf59-119">Request headers</span></span>
|<span data-ttu-id="5cf59-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5cf59-120">Header</span></span>|<span data-ttu-id="5cf59-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5cf59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cf59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cf59-122">Authorization</span></span>|<span data-ttu-id="5cf59-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5cf59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cf59-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5cf59-124">Accept</span></span>|<span data-ttu-id="5cf59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5cf59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cf59-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5cf59-126">Request body</span></span>
<span data-ttu-id="5cf59-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5cf59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cf59-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cf59-128">Response</span></span>
<span data-ttu-id="5cf59-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cf59-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5cf59-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5cf59-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cf59-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cf59-131">Request</span></span>
<span data-ttu-id="5cf59-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5cf59-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5cf59-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cf59-133">Response</span></span>
<span data-ttu-id="5cf59-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cf59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





---
title: IosLobAppProvisioningConfigurationAssignment löschen
description: Löscht eine IosLobAppProvisioningConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af38c172150224df8738a716537ac2bdda9126eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828777"
---
# <a name="delete-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="36503-103">IosLobAppProvisioningConfigurationAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="36503-103">Delete iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="36503-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="36503-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36503-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36503-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36503-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36503-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36503-107">Löscht eine [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="36503-107">Deletes a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36503-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36503-108">Prerequisites</span></span>
<span data-ttu-id="36503-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36503-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36503-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36503-111">Permission type</span></span>|<span data-ttu-id="36503-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36503-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36503-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36503-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36503-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36503-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36503-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36503-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36503-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36503-116">Not supported.</span></span>|
|<span data-ttu-id="36503-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36503-117">Application</span></span>|<span data-ttu-id="36503-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36503-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36503-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36503-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="36503-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36503-120">Request headers</span></span>
|<span data-ttu-id="36503-121">Header</span><span class="sxs-lookup"><span data-stu-id="36503-121">Header</span></span>|<span data-ttu-id="36503-122">Wert</span><span class="sxs-lookup"><span data-stu-id="36503-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36503-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36503-123">Authorization</span></span>|<span data-ttu-id="36503-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36503-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36503-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36503-125">Accept</span></span>|<span data-ttu-id="36503-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36503-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36503-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36503-127">Request body</span></span>
<span data-ttu-id="36503-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36503-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36503-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="36503-129">Response</span></span>
<span data-ttu-id="36503-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36503-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36503-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36503-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36503-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36503-132">Request</span></span>
<span data-ttu-id="36503-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36503-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="36503-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="36503-134">Response</span></span>
<span data-ttu-id="36503-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36503-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






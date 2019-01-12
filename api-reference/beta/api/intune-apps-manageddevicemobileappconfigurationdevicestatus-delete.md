---
title: ManagedDeviceMobileAppConfigurationDeviceStatus löschen
description: Löscht eine ManagedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d376e546f5de314571fcc4faaa9ff04346b9f52f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934429"
---
# <a name="delete-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="c0225-103">ManagedDeviceMobileAppConfigurationDeviceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="c0225-103">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="c0225-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0225-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0225-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0225-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0225-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0225-107">Löscht eine [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c0225-107">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0225-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c0225-108">Prerequisites</span></span>
<span data-ttu-id="c0225-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0225-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0225-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0225-111">Permission type</span></span>|<span data-ttu-id="c0225-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0225-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0225-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0225-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0225-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0225-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c0225-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0225-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0225-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0225-116">Not supported.</span></span>|
|<span data-ttu-id="c0225-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0225-117">Application</span></span>|<span data-ttu-id="c0225-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c0225-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0225-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0225-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c0225-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0225-120">Request headers</span></span>
|<span data-ttu-id="c0225-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0225-121">Header</span></span>|<span data-ttu-id="c0225-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0225-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0225-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0225-123">Authorization</span></span>|<span data-ttu-id="c0225-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c0225-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0225-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c0225-125">Accept</span></span>|<span data-ttu-id="c0225-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0225-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0225-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0225-127">Request body</span></span>
<span data-ttu-id="c0225-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c0225-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0225-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0225-129">Response</span></span>
<span data-ttu-id="c0225-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0225-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0225-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0225-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0225-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0225-132">Request</span></span>
<span data-ttu-id="c0225-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0225-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="c0225-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0225-134">Response</span></span>
<span data-ttu-id="c0225-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0225-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






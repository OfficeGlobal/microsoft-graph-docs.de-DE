---
title: ManagedDeviceMobileAppConfigurationDeviceStatus löschen
description: Löscht eine ManagedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9053b3f86b8809f4920b7d10c157e40fe58ba4f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867319"
---
# <a name="delete-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="c517e-103">ManagedDeviceMobileAppConfigurationDeviceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="c517e-103">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="c517e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c517e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c517e-105">Löscht eine [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c517e-105">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c517e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c517e-106">Prerequisites</span></span>
<span data-ttu-id="c517e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c517e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c517e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c517e-109">Permission type</span></span>|<span data-ttu-id="c517e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c517e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c517e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c517e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c517e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c517e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c517e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c517e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c517e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c517e-114">Not supported.</span></span>|
|<span data-ttu-id="c517e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c517e-115">Application</span></span>|<span data-ttu-id="c517e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c517e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c517e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c517e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c517e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c517e-118">Request headers</span></span>
|<span data-ttu-id="c517e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c517e-119">Header</span></span>|<span data-ttu-id="c517e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c517e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c517e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c517e-121">Authorization</span></span>|<span data-ttu-id="c517e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c517e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c517e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c517e-123">Accept</span></span>|<span data-ttu-id="c517e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c517e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c517e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c517e-125">Request body</span></span>
<span data-ttu-id="c517e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c517e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c517e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c517e-127">Response</span></span>
<span data-ttu-id="c517e-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c517e-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c517e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c517e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c517e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c517e-130">Request</span></span>
<span data-ttu-id="c517e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c517e-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="c517e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c517e-132">Response</span></span>
<span data-ttu-id="c517e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c517e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




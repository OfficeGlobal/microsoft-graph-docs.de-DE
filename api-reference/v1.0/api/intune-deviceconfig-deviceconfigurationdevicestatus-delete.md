---
title: deviceConfigurationDeviceStatus löschen
description: Löscht ein deviceConfigurationDeviceStatus-Objekt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 38d777bc1f2b9c0bcbc23271d634294cddf9be02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810605"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="37f21-103">deviceConfigurationDeviceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="37f21-103">Delete deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="37f21-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="37f21-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37f21-105">Löscht ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="37f21-105">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37f21-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37f21-106">Prerequisites</span></span>
<span data-ttu-id="37f21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f21-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37f21-109">Permission type</span></span>|<span data-ttu-id="37f21-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37f21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f21-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37f21-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37f21-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f21-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37f21-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37f21-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f21-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37f21-114">Not supported.</span></span>|
|<span data-ttu-id="37f21-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37f21-115">Application</span></span>|<span data-ttu-id="37f21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37f21-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f21-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37f21-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="37f21-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37f21-118">Request headers</span></span>
|<span data-ttu-id="37f21-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="37f21-119">Header</span></span>|<span data-ttu-id="37f21-120">Wert</span><span class="sxs-lookup"><span data-stu-id="37f21-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37f21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f21-121">Authorization</span></span>|<span data-ttu-id="37f21-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37f21-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37f21-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="37f21-123">Accept</span></span>|<span data-ttu-id="37f21-124">application/json</span><span class="sxs-lookup"><span data-stu-id="37f21-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f21-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37f21-125">Request body</span></span>
<span data-ttu-id="37f21-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="37f21-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37f21-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="37f21-127">Response</span></span>
<span data-ttu-id="37f21-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37f21-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="37f21-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37f21-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="37f21-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37f21-130">Request</span></span>
<span data-ttu-id="37f21-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37f21-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="37f21-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="37f21-132">Response</span></span>
<span data-ttu-id="37f21-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37f21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




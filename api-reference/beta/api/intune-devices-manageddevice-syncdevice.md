---
title: syncDevice-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8f3a435eef337aca83c98c1ecb70d56bccbc8df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953224"
---
# <a name="syncdevice-action"></a><span data-ttu-id="a012e-103">syncDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="a012e-103">syncDevice action</span></span>

> <span data-ttu-id="a012e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a012e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a012e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a012e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a012e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a012e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a012e-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a012e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a012e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a012e-108">Prerequisites</span></span>
<span data-ttu-id="a012e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a012e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a012e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a012e-111">Permission type</span></span>|<span data-ttu-id="a012e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a012e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a012e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a012e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a012e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a012e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a012e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a012e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a012e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a012e-116">Not supported.</span></span>|
|<span data-ttu-id="a012e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a012e-117">Application</span></span>|<span data-ttu-id="a012e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a012e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a012e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a012e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="a012e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a012e-120">Request headers</span></span>
|<span data-ttu-id="a012e-121">Header</span><span class="sxs-lookup"><span data-stu-id="a012e-121">Header</span></span>|<span data-ttu-id="a012e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a012e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a012e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a012e-123">Authorization</span></span>|<span data-ttu-id="a012e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a012e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a012e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a012e-125">Accept</span></span>|<span data-ttu-id="a012e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a012e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a012e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a012e-127">Request body</span></span>
<span data-ttu-id="a012e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a012e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a012e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a012e-129">Response</span></span>
<span data-ttu-id="a012e-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="a012e-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a012e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a012e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a012e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a012e-132">Request</span></span>
<span data-ttu-id="a012e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a012e-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="a012e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a012e-134">Response</span></span>
<span data-ttu-id="a012e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a012e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






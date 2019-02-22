---
title: rebootNow-Aktion
description: Gerät neu starten
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcfb45c52331454c56a15efb25d573f7b6f14d39
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147901"
---
# <a name="rebootnow-action"></a><span data-ttu-id="31d14-103">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="31d14-103">rebootNow action</span></span>

> <span data-ttu-id="31d14-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31d14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31d14-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="31d14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31d14-106">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="31d14-106">Reboot device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31d14-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31d14-107">Prerequisites</span></span>
<span data-ttu-id="31d14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="31d14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31d14-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31d14-110">Permission type</span></span>|<span data-ttu-id="31d14-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31d14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d14-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31d14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31d14-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="31d14-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="31d14-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31d14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d14-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31d14-115">Not supported.</span></span>|
|<span data-ttu-id="31d14-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31d14-116">Application</span></span>|<span data-ttu-id="31d14-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31d14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d14-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31d14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rebootNow
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rebootNow
```

## <a name="request-headers"></a><span data-ttu-id="31d14-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31d14-119">Request headers</span></span>
|<span data-ttu-id="31d14-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31d14-120">Header</span></span>|<span data-ttu-id="31d14-121">Wert</span><span class="sxs-lookup"><span data-stu-id="31d14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31d14-122">Authorization</span></span>|<span data-ttu-id="31d14-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31d14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d14-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31d14-124">Accept</span></span>|<span data-ttu-id="31d14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31d14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d14-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31d14-126">Request body</span></span>
<span data-ttu-id="31d14-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31d14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31d14-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="31d14-128">Response</span></span>
<span data-ttu-id="31d14-129">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="31d14-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="31d14-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31d14-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="31d14-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31d14-131">Request</span></span>
<span data-ttu-id="31d14-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31d14-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/rebootNow
```

### <a name="response"></a><span data-ttu-id="31d14-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="31d14-133">Response</span></span>
<span data-ttu-id="31d14-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31d14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





---
title: remoteLock-Aktion
description: Remotesperre
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35787fe0776774d1f2550b7a3a19d662b42cae0d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973628"
---
# <a name="remotelock-action"></a><span data-ttu-id="d5b03-103">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="d5b03-103">remoteLock action</span></span>

> <span data-ttu-id="d5b03-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5b03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b03-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d5b03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b03-106">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="d5b03-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5b03-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5b03-107">Prerequisites</span></span>
<span data-ttu-id="d5b03-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5b03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b03-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5b03-110">Permission type</span></span>|<span data-ttu-id="d5b03-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5b03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5b03-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5b03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5b03-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d5b03-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d5b03-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5b03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5b03-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5b03-115">Not supported.</span></span>|
|<span data-ttu-id="d5b03-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5b03-116">Application</span></span>|<span data-ttu-id="d5b03-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5b03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5b03-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5b03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="d5b03-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5b03-119">Request headers</span></span>
|<span data-ttu-id="d5b03-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5b03-120">Header</span></span>|<span data-ttu-id="d5b03-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d5b03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5b03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5b03-122">Authorization</span></span>|<span data-ttu-id="d5b03-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5b03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5b03-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d5b03-124">Accept</span></span>|<span data-ttu-id="d5b03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5b03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5b03-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5b03-126">Request body</span></span>
<span data-ttu-id="d5b03-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d5b03-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5b03-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5b03-128">Response</span></span>
<span data-ttu-id="d5b03-129">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5b03-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5b03-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5b03-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5b03-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5b03-131">Request</span></span>
<span data-ttu-id="d5b03-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5b03-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="d5b03-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5b03-133">Response</span></span>
<span data-ttu-id="d5b03-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5b03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





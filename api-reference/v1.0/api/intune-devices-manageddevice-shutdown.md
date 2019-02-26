---
title: shutDown-Aktion
description: Gerät abschalten
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f47dd5beeacf9e55597957765518d16af50036cb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257274"
---
# <a name="shutdown-action"></a><span data-ttu-id="e7d35-103">shutDown-Aktion</span><span class="sxs-lookup"><span data-stu-id="e7d35-103">shutDown action</span></span>

> <span data-ttu-id="e7d35-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e7d35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d35-105">Gerät abschalten</span><span class="sxs-lookup"><span data-stu-id="e7d35-105">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7d35-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e7d35-106">Prerequisites</span></span>
<span data-ttu-id="e7d35-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7d35-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7d35-109">Permission type</span></span>|<span data-ttu-id="e7d35-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7d35-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d35-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7d35-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d35-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e7d35-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e7d35-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7d35-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d35-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7d35-114">Not supported.</span></span>|
|<span data-ttu-id="e7d35-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7d35-115">Application</span></span>|<span data-ttu-id="e7d35-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7d35-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d35-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7d35-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="e7d35-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7d35-118">Request headers</span></span>
|<span data-ttu-id="e7d35-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e7d35-119">Header</span></span>|<span data-ttu-id="e7d35-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e7d35-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d35-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7d35-121">Authorization</span></span>|<span data-ttu-id="e7d35-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e7d35-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d35-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e7d35-123">Accept</span></span>|<span data-ttu-id="e7d35-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d35-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d35-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7d35-125">Request body</span></span>
<span data-ttu-id="e7d35-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7d35-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d35-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7d35-127">Response</span></span>
<span data-ttu-id="e7d35-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e7d35-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7d35-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7d35-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7d35-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7d35-130">Request</span></span>
<span data-ttu-id="e7d35-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7d35-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="e7d35-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7d35-132">Response</span></span>
<span data-ttu-id="e7d35-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7d35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




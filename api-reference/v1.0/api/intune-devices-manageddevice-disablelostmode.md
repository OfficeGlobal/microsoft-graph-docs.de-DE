---
title: disableLostMode-Aktion
description: Modus für verlorene Geräte deaktivieren
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a377869d236f06921bd2a3d7fe5d5dea8659c81a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956821"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="7b5af-103">disableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="7b5af-103">disableLostMode action</span></span>

> <span data-ttu-id="7b5af-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b5af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b5af-105">Modus für verlorene Geräte deaktivieren</span><span class="sxs-lookup"><span data-stu-id="7b5af-105">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b5af-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b5af-106">Prerequisites</span></span>
<span data-ttu-id="7b5af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b5af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b5af-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b5af-109">Permission type</span></span>|<span data-ttu-id="7b5af-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b5af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b5af-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b5af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b5af-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7b5af-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7b5af-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b5af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b5af-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b5af-114">Not supported.</span></span>|
|<span data-ttu-id="7b5af-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b5af-115">Application</span></span>|<span data-ttu-id="7b5af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b5af-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b5af-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b5af-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="7b5af-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b5af-118">Request headers</span></span>
|<span data-ttu-id="7b5af-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b5af-119">Header</span></span>|<span data-ttu-id="7b5af-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7b5af-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b5af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b5af-121">Authorization</span></span>|<span data-ttu-id="7b5af-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b5af-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b5af-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b5af-123">Accept</span></span>|<span data-ttu-id="7b5af-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b5af-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b5af-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b5af-125">Request body</span></span>
<span data-ttu-id="7b5af-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b5af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b5af-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b5af-127">Response</span></span>
<span data-ttu-id="7b5af-128">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b5af-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7b5af-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b5af-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b5af-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b5af-130">Request</span></span>
<span data-ttu-id="7b5af-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b5af-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="7b5af-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b5af-132">Response</span></span>
<span data-ttu-id="7b5af-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b5af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




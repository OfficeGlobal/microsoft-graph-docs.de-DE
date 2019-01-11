---
title: windowsDefenderUpdateSignatures-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 93869feea6163636ca19fb681740293e76c72d98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885554"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="1e8eb-103">windowsDefenderUpdateSignatures-Aktion</span><span class="sxs-lookup"><span data-stu-id="1e8eb-103">windowsDefenderUpdateSignatures action</span></span>

> <span data-ttu-id="1e8eb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1e8eb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e8eb-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1e8eb-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e8eb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e8eb-106">Prerequisites</span></span>
<span data-ttu-id="1e8eb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e8eb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e8eb-109">Permission type</span></span>|<span data-ttu-id="1e8eb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e8eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e8eb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e8eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e8eb-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1e8eb-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1e8eb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e8eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e8eb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e8eb-114">Not supported.</span></span>|
|<span data-ttu-id="1e8eb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e8eb-115">Application</span></span>|<span data-ttu-id="1e8eb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e8eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e8eb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e8eb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="1e8eb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e8eb-118">Request headers</span></span>
|<span data-ttu-id="1e8eb-119">Header</span><span class="sxs-lookup"><span data-stu-id="1e8eb-119">Header</span></span>|<span data-ttu-id="1e8eb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1e8eb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e8eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e8eb-121">Authorization</span></span>|<span data-ttu-id="1e8eb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e8eb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e8eb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e8eb-123">Accept</span></span>|<span data-ttu-id="1e8eb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e8eb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e8eb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e8eb-125">Request body</span></span>
<span data-ttu-id="1e8eb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e8eb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e8eb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e8eb-127">Response</span></span>
<span data-ttu-id="1e8eb-128">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="1e8eb-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1e8eb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e8eb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e8eb-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e8eb-130">Request</span></span>
<span data-ttu-id="1e8eb-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e8eb-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="1e8eb-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e8eb-132">Response</span></span>
<span data-ttu-id="1e8eb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e8eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




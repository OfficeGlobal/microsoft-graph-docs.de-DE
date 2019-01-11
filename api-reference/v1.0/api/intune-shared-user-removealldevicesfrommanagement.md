---
title: removeAllDevicesFromManagement-Aktion
description: Die Verwaltung aller Geräte für diesen Benutzer einstellen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3f43d941775f726c73981b387ef60fd9e26cc955
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849644"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="224e7-103">removeAllDevicesFromManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="224e7-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="224e7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="224e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="224e7-105">Die Verwaltung aller Geräte für diesen Benutzer einstellen.</span><span class="sxs-lookup"><span data-stu-id="224e7-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="224e7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="224e7-106">Prerequisites</span></span>
<span data-ttu-id="224e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="224e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="224e7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="224e7-109">Permission type</span></span>|<span data-ttu-id="224e7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="224e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="224e7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="224e7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="224e7-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="224e7-112">_varies by context_</span></span> |
| <span data-ttu-id="224e7-113">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="224e7-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="224e7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="224e7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="224e7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="224e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="224e7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="224e7-116">Not supported.</span></span>|
|<span data-ttu-id="224e7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="224e7-117">Application</span></span>|<span data-ttu-id="224e7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="224e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="224e7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="224e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="224e7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="224e7-120">Request headers</span></span>
|<span data-ttu-id="224e7-121">Header</span><span class="sxs-lookup"><span data-stu-id="224e7-121">Header</span></span>|<span data-ttu-id="224e7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="224e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="224e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="224e7-123">Authorization</span></span>|<span data-ttu-id="224e7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="224e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="224e7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="224e7-125">Accept</span></span>|<span data-ttu-id="224e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="224e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="224e7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="224e7-127">Request body</span></span>
<span data-ttu-id="224e7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="224e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="224e7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="224e7-129">Response</span></span>
<span data-ttu-id="224e7-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="224e7-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="224e7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="224e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="224e7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="224e7-132">Request</span></span>
<span data-ttu-id="224e7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="224e7-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="224e7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="224e7-134">Response</span></span>
<span data-ttu-id="224e7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="224e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




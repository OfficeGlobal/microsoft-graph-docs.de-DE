---
title: removeAllDevicesFromManagement-Aktion
description: Die Verwaltung aller Geräte für diesen Benutzer einstellen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40baa470968c10bbe26af1d8397306f5b9e3f736
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252798"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="6fbe1-103">removeAllDevicesFromManagement-Aktion</span><span class="sxs-lookup"><span data-stu-id="6fbe1-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="6fbe1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbe1-105">Die Verwaltung aller Geräte für diesen Benutzer einstellen.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fbe1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fbe1-106">Prerequisites</span></span>
<span data-ttu-id="6fbe1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fbe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fbe1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fbe1-109">Permission type</span></span>|<span data-ttu-id="6fbe1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fbe1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fbe1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fbe1-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6fbe1-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="6fbe1-112">_varies by context_</span></span> |
| <span data-ttu-id="6fbe1-113">&nbsp;&nbsp; Geräteverwaltung</span><span class="sxs-lookup"><span data-stu-id="6fbe1-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6fbe1-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6fbe1-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="6fbe1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fbe1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fbe1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fbe1-116">Not supported.</span></span>|
|<span data-ttu-id="6fbe1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fbe1-117">Application</span></span>|<span data-ttu-id="6fbe1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fbe1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fbe1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fbe1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="6fbe1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fbe1-120">Request headers</span></span>
|<span data-ttu-id="6fbe1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6fbe1-121">Header</span></span>|<span data-ttu-id="6fbe1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6fbe1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fbe1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fbe1-123">Authorization</span></span>|<span data-ttu-id="6fbe1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fbe1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fbe1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6fbe1-125">Accept</span></span>|<span data-ttu-id="6fbe1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fbe1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fbe1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fbe1-127">Request body</span></span>
<span data-ttu-id="6fbe1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fbe1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fbe1-129">Response</span></span>
<span data-ttu-id="6fbe1-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6fbe1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fbe1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fbe1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fbe1-132">Request</span></span>
<span data-ttu-id="6fbe1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="6fbe1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fbe1-134">Response</span></span>
<span data-ttu-id="6fbe1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fbe1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




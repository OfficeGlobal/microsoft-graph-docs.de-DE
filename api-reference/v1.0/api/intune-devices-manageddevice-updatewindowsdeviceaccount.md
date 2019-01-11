---
title: updateWindowsDeviceAccount-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b189793dfb9351de9015b3052a88ac53e31fa85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829624"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="6671b-103">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="6671b-103">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="6671b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6671b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6671b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6671b-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6671b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6671b-106">Prerequisites</span></span>
<span data-ttu-id="6671b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6671b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6671b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6671b-109">Permission type</span></span>|<span data-ttu-id="6671b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6671b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6671b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6671b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6671b-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6671b-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6671b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6671b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6671b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6671b-114">Not supported.</span></span>|
|<span data-ttu-id="6671b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6671b-115">Application</span></span>|<span data-ttu-id="6671b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6671b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6671b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6671b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="6671b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6671b-118">Request headers</span></span>
|<span data-ttu-id="6671b-119">Header</span><span class="sxs-lookup"><span data-stu-id="6671b-119">Header</span></span>|<span data-ttu-id="6671b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6671b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6671b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6671b-121">Authorization</span></span>|<span data-ttu-id="6671b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6671b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6671b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6671b-123">Accept</span></span>|<span data-ttu-id="6671b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6671b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6671b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6671b-125">Request body</span></span>
<span data-ttu-id="6671b-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="6671b-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6671b-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6671b-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6671b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6671b-128">Property</span></span>|<span data-ttu-id="6671b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6671b-129">Type</span></span>|<span data-ttu-id="6671b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6671b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6671b-131">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="6671b-131">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="6671b-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="6671b-132">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="6671b-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="6671b-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6671b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6671b-134">Response</span></span>
<span data-ttu-id="6671b-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="6671b-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6671b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6671b-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="6671b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6671b-137">Request</span></span>
<span data-ttu-id="6671b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6671b-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6671b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6671b-139">Response</span></span>
<span data-ttu-id="6671b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6671b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




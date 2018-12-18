---
title: Benutzer löschen
description: Löscht einen user.
author: tfitzmac
ms.openlocfilehash: 8ed00b2967fa04fd23351c7dbc369b25d97cba39
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337317"
---
# <a name="delete-user"></a><span data-ttu-id="2616d-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="2616d-103">Delete user</span></span>

> <span data-ttu-id="2616d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2616d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2616d-105">Löscht ein [user](../resources/intune-shared-user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2616d-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2616d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2616d-106">Prerequisites</span></span>
<span data-ttu-id="2616d-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="2616d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2616d-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2616d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="2616d-109">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="2616d-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="2616d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2616d-110">Permission type</span></span>|<span data-ttu-id="2616d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2616d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2616d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2616d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2616d-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="2616d-113">_varies by context_</span></span>|
| <span data-ttu-id="2616d-114">&nbsp;&nbsp; Geräte</span><span class="sxs-lookup"><span data-stu-id="2616d-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="2616d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2616d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="2616d-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="2616d-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="2616d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2616d-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="2616d-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="2616d-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="2616d-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2616d-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="2616d-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="2616d-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="2616d-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2616d-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="2616d-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2616d-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2616d-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2616d-123">Not supported.</span></span>|
|<span data-ttu-id="2616d-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2616d-124">Application</span></span>|<span data-ttu-id="2616d-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2616d-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2616d-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2616d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="2616d-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2616d-127">Request headers</span></span>
|<span data-ttu-id="2616d-128">Header</span><span class="sxs-lookup"><span data-stu-id="2616d-128">Header</span></span>|<span data-ttu-id="2616d-129">Wert</span><span class="sxs-lookup"><span data-stu-id="2616d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2616d-130">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2616d-130">Authorization</span></span>|<span data-ttu-id="2616d-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2616d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2616d-132">Accept</span><span class="sxs-lookup"><span data-stu-id="2616d-132">Accept</span></span>|<span data-ttu-id="2616d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="2616d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2616d-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2616d-134">Request body</span></span>
<span data-ttu-id="2616d-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2616d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2616d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2616d-136">Response</span></span>
<span data-ttu-id="2616d-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2616d-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2616d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2616d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2616d-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2616d-139">Request</span></span>
<span data-ttu-id="2616d-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2616d-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="2616d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2616d-141">Response</span></span>
<span data-ttu-id="2616d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2616d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




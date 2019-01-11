---
title: Benutzer löschen
description: Löscht einen user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1979284cada76f76a98acc8956271b7224aa53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837835"
---
# <a name="delete-user"></a><span data-ttu-id="c66eb-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="c66eb-103">Delete user</span></span>

> <span data-ttu-id="c66eb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c66eb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c66eb-105">Löscht ein [user](../resources/intune-shared-user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c66eb-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c66eb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c66eb-106">Prerequisites</span></span>
<span data-ttu-id="c66eb-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="c66eb-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c66eb-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c66eb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c66eb-109">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="c66eb-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="c66eb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c66eb-110">Permission type</span></span>|<span data-ttu-id="c66eb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c66eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c66eb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c66eb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c66eb-113">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="c66eb-113">_varies by context_</span></span>|
| <span data-ttu-id="c66eb-114">&nbsp;&nbsp; Geräte</span><span class="sxs-lookup"><span data-stu-id="c66eb-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="c66eb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66eb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c66eb-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="c66eb-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c66eb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66eb-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c66eb-118">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="c66eb-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="c66eb-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66eb-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c66eb-120">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="c66eb-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="c66eb-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66eb-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="c66eb-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c66eb-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c66eb-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c66eb-123">Not supported.</span></span>|
|<span data-ttu-id="c66eb-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c66eb-124">Application</span></span>|<span data-ttu-id="c66eb-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c66eb-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c66eb-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c66eb-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c66eb-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c66eb-127">Request headers</span></span>
|<span data-ttu-id="c66eb-128">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c66eb-128">Header</span></span>|<span data-ttu-id="c66eb-129">Wert</span><span class="sxs-lookup"><span data-stu-id="c66eb-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c66eb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c66eb-130">Authorization</span></span>|<span data-ttu-id="c66eb-131">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c66eb-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c66eb-132">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c66eb-132">Accept</span></span>|<span data-ttu-id="c66eb-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c66eb-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c66eb-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c66eb-134">Request body</span></span>
<span data-ttu-id="c66eb-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c66eb-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c66eb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c66eb-136">Response</span></span>
<span data-ttu-id="c66eb-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c66eb-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c66eb-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c66eb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c66eb-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c66eb-139">Request</span></span>
<span data-ttu-id="c66eb-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c66eb-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c66eb-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c66eb-141">Response</span></span>
<span data-ttu-id="c66eb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c66eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




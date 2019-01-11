---
title: Benutzer löschen
description: Löscht einen user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6adc1e40e522746a9bfa687366f2492717ac83ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827272"
---
# <a name="delete-user"></a><span data-ttu-id="efe4b-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="efe4b-103">Delete user</span></span>

> <span data-ttu-id="efe4b-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="efe4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efe4b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efe4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efe4b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="efe4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efe4b-107">Löscht ein [user](../resources/intune-shared-user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="efe4b-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efe4b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="efe4b-108">Prerequisites</span></span>
<span data-ttu-id="efe4b-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="efe4b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="efe4b-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efe4b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="efe4b-111">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="efe4b-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="efe4b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="efe4b-112">Permission type</span></span>|<span data-ttu-id="efe4b-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="efe4b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe4b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="efe4b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="efe4b-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="efe4b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="efe4b-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe4b-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="efe4b-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="efe4b-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="efe4b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe4b-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="efe4b-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="efe4b-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="efe4b-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe4b-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="efe4b-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="efe4b-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="efe4b-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe4b-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="efe4b-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="efe4b-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe4b-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efe4b-124">Not supported.</span></span>|
|<span data-ttu-id="efe4b-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="efe4b-125">Application</span></span>|<span data-ttu-id="efe4b-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="efe4b-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe4b-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efe4b-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="efe4b-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="efe4b-128">Request headers</span></span>

|<span data-ttu-id="efe4b-129">Header</span><span class="sxs-lookup"><span data-stu-id="efe4b-129">Header</span></span>|<span data-ttu-id="efe4b-130">Wert</span><span class="sxs-lookup"><span data-stu-id="efe4b-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efe4b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="efe4b-131">Authorization</span></span>|<span data-ttu-id="efe4b-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="efe4b-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efe4b-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="efe4b-133">Accept</span></span>|<span data-ttu-id="efe4b-134">application/json</span><span class="sxs-lookup"><span data-stu-id="efe4b-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe4b-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="efe4b-135">Request body</span></span>

<span data-ttu-id="efe4b-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="efe4b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efe4b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="efe4b-137">Response</span></span>

<span data-ttu-id="efe4b-138">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efe4b-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efe4b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efe4b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="efe4b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efe4b-140">Request</span></span>

<span data-ttu-id="efe4b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="efe4b-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="efe4b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="efe4b-142">Response</span></span>

<span data-ttu-id="efe4b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efe4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




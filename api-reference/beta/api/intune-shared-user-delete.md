---
title: Benutzer löschen
description: Löscht einen user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6d0afb6c816241acf15319c3fb4082d3cc7935dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165492"
---
# <a name="delete-user"></a><span data-ttu-id="cb3db-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="cb3db-103">Delete user</span></span>

> <span data-ttu-id="cb3db-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="cb3db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb3db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb3db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb3db-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cb3db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb3db-107">Löscht ein [user](../resources/intune-shared-user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="cb3db-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb3db-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb3db-108">Prerequisites</span></span>
<span data-ttu-id="cb3db-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="cb3db-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cb3db-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3db-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="cb3db-111">Die erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="cb3db-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="cb3db-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb3db-112">Permission type</span></span>|<span data-ttu-id="cb3db-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb3db-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3db-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb3db-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cb3db-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="cb3db-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="cb3db-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3db-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="cb3db-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="cb3db-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="cb3db-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3db-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="cb3db-119">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="cb3db-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="cb3db-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3db-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="cb3db-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="cb3db-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="cb3db-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3db-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb3db-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb3db-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3db-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb3db-124">Not supported.</span></span>|
|<span data-ttu-id="cb3db-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb3db-125">Application</span></span>|<span data-ttu-id="cb3db-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb3db-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3db-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb3db-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="cb3db-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb3db-128">Request headers</span></span>

|<span data-ttu-id="cb3db-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cb3db-129">Header</span></span>|<span data-ttu-id="cb3db-130">Wert</span><span class="sxs-lookup"><span data-stu-id="cb3db-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3db-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3db-131">Authorization</span></span>|<span data-ttu-id="cb3db-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb3db-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3db-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cb3db-133">Accept</span></span>|<span data-ttu-id="cb3db-134">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3db-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3db-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb3db-135">Request body</span></span>

<span data-ttu-id="cb3db-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb3db-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb3db-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb3db-137">Response</span></span>

<span data-ttu-id="cb3db-138">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb3db-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cb3db-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb3db-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb3db-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb3db-140">Request</span></span>

<span data-ttu-id="cb3db-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb3db-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="cb3db-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb3db-142">Response</span></span>

<span data-ttu-id="cb3db-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb3db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




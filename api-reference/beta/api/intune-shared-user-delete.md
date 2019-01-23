---
title: Benutzer löschen
description: Löscht einen user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecf07bf080a76e6f1fce515d41090be214e7a514
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407151"
---
# <a name="delete-user"></a><span data-ttu-id="f3fec-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="f3fec-103">Delete user</span></span>

> <span data-ttu-id="f3fec-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f3fec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f3fec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3fec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3fec-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f3fec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3fec-107">Löscht ein [user](../resources/intune-shared-user.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f3fec-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3fec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3fec-108">Prerequisites</span></span>
<span data-ttu-id="f3fec-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="f3fec-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f3fec-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3fec-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f3fec-111">Die spezifische erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="f3fec-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="f3fec-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3fec-112">Permission type</span></span>|<span data-ttu-id="f3fec-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3fec-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3fec-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3fec-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f3fec-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="f3fec-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f3fec-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f3fec-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f3fec-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f3fec-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f3fec-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f3fec-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f3fec-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="f3fec-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="f3fec-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f3fec-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fec-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3fec-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3fec-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3fec-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3fec-124">Not supported.</span></span>|
|<span data-ttu-id="f3fec-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3fec-125">Application</span></span>|<span data-ttu-id="f3fec-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3fec-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3fec-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3fec-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="f3fec-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3fec-128">Request headers</span></span>

|<span data-ttu-id="f3fec-129">Header</span><span class="sxs-lookup"><span data-stu-id="f3fec-129">Header</span></span>|<span data-ttu-id="f3fec-130">Wert</span><span class="sxs-lookup"><span data-stu-id="f3fec-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3fec-131">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f3fec-131">Authorization</span></span>|<span data-ttu-id="f3fec-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3fec-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3fec-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f3fec-133">Accept</span></span>|<span data-ttu-id="f3fec-134">application/json</span><span class="sxs-lookup"><span data-stu-id="f3fec-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3fec-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3fec-135">Request body</span></span>

<span data-ttu-id="f3fec-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3fec-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3fec-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3fec-137">Response</span></span>

<span data-ttu-id="f3fec-138">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3fec-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3fec-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3fec-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3fec-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3fec-140">Request</span></span>

<span data-ttu-id="f3fec-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3fec-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="f3fec-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3fec-142">Response</span></span>

<span data-ttu-id="f3fec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3fec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




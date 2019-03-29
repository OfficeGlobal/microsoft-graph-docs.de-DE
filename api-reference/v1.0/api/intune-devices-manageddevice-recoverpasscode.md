---
title: recoverPasscode-Aktion
description: Kennung wiederherstellen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fed5fa3e910ccc74808f63728d6c3253bb879e0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976302"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="bf115-103">recoverPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="bf115-103">recoverPasscode action</span></span>

> <span data-ttu-id="bf115-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bf115-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf115-105">Kennung wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="bf115-105">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf115-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bf115-106">Prerequisites</span></span>
<span data-ttu-id="bf115-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf115-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf115-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf115-109">Permission type</span></span>|<span data-ttu-id="bf115-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf115-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf115-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf115-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf115-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="bf115-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="bf115-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf115-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf115-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf115-114">Not supported.</span></span>|
|<span data-ttu-id="bf115-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf115-115">Application</span></span>|<span data-ttu-id="bf115-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf115-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf115-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf115-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="bf115-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf115-118">Request headers</span></span>
|<span data-ttu-id="bf115-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bf115-119">Header</span></span>|<span data-ttu-id="bf115-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bf115-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf115-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf115-121">Authorization</span></span>|<span data-ttu-id="bf115-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bf115-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf115-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bf115-123">Accept</span></span>|<span data-ttu-id="bf115-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf115-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf115-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf115-125">Request body</span></span>
<span data-ttu-id="bf115-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bf115-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf115-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf115-127">Response</span></span>
<span data-ttu-id="bf115-128">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf115-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf115-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf115-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf115-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf115-130">Request</span></span>
<span data-ttu-id="bf115-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf115-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="bf115-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf115-132">Response</span></span>
<span data-ttu-id="bf115-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf115-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




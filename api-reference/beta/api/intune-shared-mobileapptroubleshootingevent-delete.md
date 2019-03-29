---
title: MobileAppTroubleshootingEvent löschen
description: Beschreibt die Delete-mobileAppTroubleshootingEvent-Methode der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41c9383524e29ff897ea255555ab663476c36659
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979879"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="088e3-103">MobileAppTroubleshootingEvent löschen</span><span class="sxs-lookup"><span data-stu-id="088e3-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="088e3-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="088e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="088e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="088e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="088e3-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="088e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="088e3-107">Löscht eine [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="088e3-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="088e3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="088e3-108">Prerequisites</span></span>
<span data-ttu-id="088e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088e3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="088e3-111">Permission type</span></span>|<span data-ttu-id="088e3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="088e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="088e3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="088e3-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="088e3-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="088e3-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="088e3-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088e3-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="088e3-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="088e3-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="088e3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088e3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="088e3-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="088e3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="088e3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="088e3-119">Not supported.</span></span>|
|<span data-ttu-id="088e3-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="088e3-120">Application</span></span>|<span data-ttu-id="088e3-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="088e3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="088e3-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="088e3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="088e3-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="088e3-123">Request headers</span></span>
|<span data-ttu-id="088e3-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="088e3-124">Header</span></span>|<span data-ttu-id="088e3-125">Wert</span><span class="sxs-lookup"><span data-stu-id="088e3-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="088e3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="088e3-126">Authorization</span></span>|<span data-ttu-id="088e3-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="088e3-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="088e3-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="088e3-128">Accept</span></span>|<span data-ttu-id="088e3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="088e3-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="088e3-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="088e3-130">Request body</span></span>
<span data-ttu-id="088e3-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="088e3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="088e3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="088e3-132">Response</span></span>
<span data-ttu-id="088e3-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="088e3-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="088e3-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="088e3-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="088e3-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="088e3-135">Request</span></span>
<span data-ttu-id="088e3-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="088e3-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="088e3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="088e3-137">Response</span></span>
<span data-ttu-id="088e3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="088e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





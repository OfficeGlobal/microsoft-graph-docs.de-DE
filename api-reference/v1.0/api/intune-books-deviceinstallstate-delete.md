---
title: deviceInstallState löschen
description: Löscht ein deviceInstallState-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d19c1e9052e231cfd6f6ebcdec6bdf7255806d28
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970128"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="ec7ec-103">deviceInstallState löschen</span><span class="sxs-lookup"><span data-stu-id="ec7ec-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="ec7ec-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec7ec-105">Löscht ein [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-105">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec7ec-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec7ec-106">Prerequisites</span></span>
<span data-ttu-id="ec7ec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec7ec-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec7ec-109">Permission type</span></span>|<span data-ttu-id="ec7ec-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec7ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec7ec-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec7ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec7ec-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec7ec-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec7ec-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec7ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec7ec-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec7ec-114">Not supported.</span></span>|
|<span data-ttu-id="ec7ec-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec7ec-115">Application</span></span>|<span data-ttu-id="ec7ec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec7ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec7ec-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec7ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ec7ec-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec7ec-118">Request headers</span></span>
|<span data-ttu-id="ec7ec-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec7ec-119">Header</span></span>|<span data-ttu-id="ec7ec-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ec7ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec7ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec7ec-121">Authorization</span></span>|<span data-ttu-id="ec7ec-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec7ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec7ec-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ec7ec-123">Accept</span></span>|<span data-ttu-id="ec7ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec7ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec7ec-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec7ec-125">Request body</span></span>
<span data-ttu-id="ec7ec-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec7ec-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec7ec-127">Response</span></span>
<span data-ttu-id="ec7ec-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ec7ec-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec7ec-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec7ec-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec7ec-130">Request</span></span>
<span data-ttu-id="ec7ec-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="ec7ec-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec7ec-132">Response</span></span>
<span data-ttu-id="ec7ec-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec7ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




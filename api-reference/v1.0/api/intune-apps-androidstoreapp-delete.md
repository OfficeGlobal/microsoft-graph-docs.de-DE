---
title: androidStoreApp löschen
description: Löscht eine androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f3eadc141163507b8ef8af5bf80ce50dd1c800c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985347"
---
# <a name="delete-androidstoreapp"></a><span data-ttu-id="50204-103">androidStoreApp löschen</span><span class="sxs-lookup"><span data-stu-id="50204-103">Delete androidStoreApp</span></span>

> <span data-ttu-id="50204-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="50204-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50204-105">Löscht eine [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="50204-105">Deletes a [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50204-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50204-106">Prerequisites</span></span>
<span data-ttu-id="50204-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50204-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50204-109">Permission type</span></span>|<span data-ttu-id="50204-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50204-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50204-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50204-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50204-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50204-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50204-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50204-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50204-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50204-114">Not supported.</span></span>|
|<span data-ttu-id="50204-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50204-115">Application</span></span>|<span data-ttu-id="50204-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50204-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50204-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50204-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="50204-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50204-118">Request headers</span></span>
|<span data-ttu-id="50204-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="50204-119">Header</span></span>|<span data-ttu-id="50204-120">Wert</span><span class="sxs-lookup"><span data-stu-id="50204-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50204-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50204-121">Authorization</span></span>|<span data-ttu-id="50204-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50204-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50204-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50204-123">Accept</span></span>|<span data-ttu-id="50204-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50204-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50204-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50204-125">Request body</span></span>
<span data-ttu-id="50204-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50204-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50204-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="50204-127">Response</span></span>
<span data-ttu-id="50204-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50204-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50204-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50204-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="50204-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50204-130">Request</span></span>
<span data-ttu-id="50204-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50204-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="50204-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="50204-132">Response</span></span>
<span data-ttu-id="50204-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50204-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




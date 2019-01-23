---
title: Win32LobApp löschen
description: Löscht eine win32LobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bd00a13f039e86c550e4ae28ce7ca4748aa360a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417623"
---
# <a name="delete-win32lobapp"></a><span data-ttu-id="7a5ba-103">Win32LobApp löschen</span><span class="sxs-lookup"><span data-stu-id="7a5ba-103">Delete win32LobApp</span></span>

> <span data-ttu-id="7a5ba-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a5ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a5ba-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a5ba-107">Löscht eine [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a5ba-107">Deletes a [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a5ba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7a5ba-108">Prerequisites</span></span>
<span data-ttu-id="7a5ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a5ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a5ba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a5ba-111">Permission type</span></span>|<span data-ttu-id="7a5ba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a5ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a5ba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a5ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a5ba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a5ba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a5ba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a5ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a5ba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a5ba-116">Not supported.</span></span>|
|<span data-ttu-id="7a5ba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a5ba-117">Application</span></span>|<span data-ttu-id="7a5ba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a5ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a5ba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7a5ba-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a5ba-120">Request headers</span></span>
|<span data-ttu-id="7a5ba-121">Header</span><span class="sxs-lookup"><span data-stu-id="7a5ba-121">Header</span></span>|<span data-ttu-id="7a5ba-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7a5ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a5ba-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7a5ba-123">Authorization</span></span>|<span data-ttu-id="7a5ba-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7a5ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a5ba-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7a5ba-125">Accept</span></span>|<span data-ttu-id="7a5ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a5ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a5ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a5ba-127">Request body</span></span>
<span data-ttu-id="7a5ba-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a5ba-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5ba-129">Response</span></span>
<span data-ttu-id="7a5ba-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7a5ba-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a5ba-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a5ba-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5ba-132">Request</span></span>
<span data-ttu-id="7a5ba-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7a5ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5ba-134">Response</span></span>
<span data-ttu-id="7a5ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a5ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





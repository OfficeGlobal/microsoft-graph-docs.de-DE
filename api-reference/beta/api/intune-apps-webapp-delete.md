---
title: webApp löschen
description: Löscht eine webApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53d14ed6f54719b5846e668a2a60f200f55da5b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837247"
---
# <a name="delete-webapp"></a><span data-ttu-id="08394-103">webApp löschen</span><span class="sxs-lookup"><span data-stu-id="08394-103">Delete webApp</span></span>

> <span data-ttu-id="08394-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08394-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08394-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08394-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08394-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="08394-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08394-107">Löscht eine [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="08394-107">Deletes a [webApp](../resources/intune-apps-webapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08394-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08394-108">Prerequisites</span></span>
<span data-ttu-id="08394-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08394-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08394-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08394-111">Permission type</span></span>|<span data-ttu-id="08394-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08394-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08394-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08394-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08394-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08394-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08394-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08394-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08394-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08394-116">Not supported.</span></span>|
|<span data-ttu-id="08394-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08394-117">Application</span></span>|<span data-ttu-id="08394-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08394-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08394-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08394-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="08394-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08394-120">Request headers</span></span>
|<span data-ttu-id="08394-121">Header</span><span class="sxs-lookup"><span data-stu-id="08394-121">Header</span></span>|<span data-ttu-id="08394-122">Wert</span><span class="sxs-lookup"><span data-stu-id="08394-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08394-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08394-123">Authorization</span></span>|<span data-ttu-id="08394-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08394-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08394-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08394-125">Accept</span></span>|<span data-ttu-id="08394-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08394-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08394-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08394-127">Request body</span></span>
<span data-ttu-id="08394-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="08394-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08394-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="08394-129">Response</span></span>
<span data-ttu-id="08394-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08394-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08394-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08394-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="08394-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08394-132">Request</span></span>
<span data-ttu-id="08394-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08394-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="08394-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="08394-134">Response</span></span>
<span data-ttu-id="08394-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08394-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






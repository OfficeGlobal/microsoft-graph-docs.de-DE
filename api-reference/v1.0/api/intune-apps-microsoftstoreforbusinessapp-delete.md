---
title: microsoftStoreForBusinessApp löschen
description: Löscht ein microsoftStoreForBusinessApp-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee02c0081d8a1167b17185cd00f01567daec0d61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972726"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="d4c74-103">microsoftStoreForBusinessApp löschen</span><span class="sxs-lookup"><span data-stu-id="d4c74-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="d4c74-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4c74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4c74-105">Löscht ein [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d4c74-105">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4c74-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4c74-106">Prerequisites</span></span>
<span data-ttu-id="d4c74-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c74-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4c74-109">Permission type</span></span>|<span data-ttu-id="d4c74-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4c74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c74-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4c74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c74-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c74-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c74-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4c74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c74-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4c74-114">Not supported.</span></span>|
|<span data-ttu-id="d4c74-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4c74-115">Application</span></span>|<span data-ttu-id="d4c74-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4c74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c74-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4c74-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d4c74-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4c74-118">Request headers</span></span>
|<span data-ttu-id="d4c74-119">Header</span><span class="sxs-lookup"><span data-stu-id="d4c74-119">Header</span></span>|<span data-ttu-id="d4c74-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d4c74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c74-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4c74-121">Authorization</span></span>|<span data-ttu-id="d4c74-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4c74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c74-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4c74-123">Accept</span></span>|<span data-ttu-id="d4c74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c74-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4c74-125">Request body</span></span>
<span data-ttu-id="d4c74-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d4c74-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c74-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4c74-127">Response</span></span>
<span data-ttu-id="d4c74-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4c74-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d4c74-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4c74-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4c74-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4c74-130">Request</span></span>
<span data-ttu-id="d4c74-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4c74-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d4c74-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4c74-132">Response</span></span>
<span data-ttu-id="d4c74-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4c74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




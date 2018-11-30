---
title: managedIOSLobApp löschen
description: Löscht eine managedIOSLobApp.
ms.openlocfilehash: eba72f6c030f0530274630eac819b7dda88518d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019744"
---
# <a name="delete-managedioslobapp"></a><span data-ttu-id="0846f-103">managedIOSLobApp löschen</span><span class="sxs-lookup"><span data-stu-id="0846f-103">Delete managedIOSLobApp</span></span>

> <span data-ttu-id="0846f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0846f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0846f-105">Löscht eine [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0846f-105">Deletes a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0846f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0846f-106">Prerequisites</span></span>
<span data-ttu-id="0846f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0846f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0846f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0846f-109">Permission type</span></span>|<span data-ttu-id="0846f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0846f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0846f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0846f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0846f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0846f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0846f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0846f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0846f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0846f-114">Not supported.</span></span>|
|<span data-ttu-id="0846f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0846f-115">Application</span></span>|<span data-ttu-id="0846f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0846f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0846f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0846f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0846f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0846f-118">Request headers</span></span>
|<span data-ttu-id="0846f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0846f-119">Header</span></span>|<span data-ttu-id="0846f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0846f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0846f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0846f-121">Authorization</span></span>|<span data-ttu-id="0846f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0846f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0846f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0846f-123">Accept</span></span>|<span data-ttu-id="0846f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0846f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0846f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0846f-125">Request body</span></span>
<span data-ttu-id="0846f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0846f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0846f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0846f-127">Response</span></span>
<span data-ttu-id="0846f-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0846f-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0846f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0846f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0846f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0846f-130">Request</span></span>
<span data-ttu-id="0846f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0846f-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="0846f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0846f-132">Response</span></span>
<span data-ttu-id="0846f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0846f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




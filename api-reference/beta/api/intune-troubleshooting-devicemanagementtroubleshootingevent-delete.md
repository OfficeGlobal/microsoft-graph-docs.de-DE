---
title: deviceManagementTroubleshootingEvent löschen
description: Löscht ein deviceManagementTroubleshootingEvent-Objekt.
ms.openlocfilehash: a8bea05b6a3f755253b397fcb846119e851d2b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065662"
---
# <a name="delete-devicemanagementtroubleshootingevent"></a><span data-ttu-id="f1e59-103">deviceManagementTroubleshootingEvent löschen</span><span class="sxs-lookup"><span data-stu-id="f1e59-103">Delete deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="f1e59-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1e59-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1e59-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1e59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1e59-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1e59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1e59-107">Löscht ein [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="f1e59-107">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1e59-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1e59-108">Prerequisites</span></span>
<span data-ttu-id="f1e59-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e59-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1e59-111">Permission type</span></span>|<span data-ttu-id="f1e59-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1e59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e59-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1e59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e59-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e59-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1e59-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1e59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e59-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e59-116">Not supported.</span></span>|
|<span data-ttu-id="f1e59-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1e59-117">Application</span></span>|<span data-ttu-id="f1e59-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1e59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e59-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="f1e59-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1e59-120">Request headers</span></span>
|<span data-ttu-id="f1e59-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1e59-121">Header</span></span>|<span data-ttu-id="f1e59-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f1e59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e59-123">Authorization</span></span>|<span data-ttu-id="f1e59-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1e59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1e59-125">Accept</span></span>|<span data-ttu-id="f1e59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e59-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1e59-127">Request body</span></span>
<span data-ttu-id="f1e59-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1e59-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1e59-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e59-129">Response</span></span>
<span data-ttu-id="f1e59-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1e59-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1e59-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1e59-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1e59-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1e59-132">Request</span></span>
<span data-ttu-id="f1e59-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1e59-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="f1e59-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1e59-134">Response</span></span>
<span data-ttu-id="f1e59-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1e59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






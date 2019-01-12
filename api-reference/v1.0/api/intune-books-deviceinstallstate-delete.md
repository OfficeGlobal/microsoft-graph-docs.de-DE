---
title: deviceInstallState löschen
description: Löscht ein deviceInstallState-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4a7aea434b80b25307e5488abee6b80bdeacb8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911889"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="911dc-103">deviceInstallState löschen</span><span class="sxs-lookup"><span data-stu-id="911dc-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="911dc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="911dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="911dc-105">Löscht ein [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="911dc-105">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="911dc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="911dc-106">Prerequisites</span></span>
<span data-ttu-id="911dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="911dc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="911dc-109">Permission type</span></span>|<span data-ttu-id="911dc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="911dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="911dc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="911dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="911dc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911dc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="911dc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="911dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="911dc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="911dc-114">Not supported.</span></span>|
|<span data-ttu-id="911dc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="911dc-115">Application</span></span>|<span data-ttu-id="911dc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="911dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="911dc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="911dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="911dc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="911dc-118">Request headers</span></span>
|<span data-ttu-id="911dc-119">Header</span><span class="sxs-lookup"><span data-stu-id="911dc-119">Header</span></span>|<span data-ttu-id="911dc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="911dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="911dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="911dc-121">Authorization</span></span>|<span data-ttu-id="911dc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="911dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="911dc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="911dc-123">Accept</span></span>|<span data-ttu-id="911dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="911dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="911dc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="911dc-125">Request body</span></span>
<span data-ttu-id="911dc-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="911dc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="911dc-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="911dc-127">Response</span></span>
<span data-ttu-id="911dc-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="911dc-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="911dc-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="911dc-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="911dc-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="911dc-130">Request</span></span>
<span data-ttu-id="911dc-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="911dc-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="911dc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="911dc-132">Response</span></span>
<span data-ttu-id="911dc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="911dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




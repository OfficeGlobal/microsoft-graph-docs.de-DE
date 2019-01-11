---
title: deviceInstallState löschen
description: Löscht ein deviceInstallState-Objekt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f415b478ff7453a6a1ac7abcdd496ca80f6e4502
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874151"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="c19cd-103">deviceInstallState löschen</span><span class="sxs-lookup"><span data-stu-id="c19cd-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="c19cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c19cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c19cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c19cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c19cd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c19cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c19cd-107">Löscht ein [deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c19cd-107">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c19cd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c19cd-108">Prerequisites</span></span>
<span data-ttu-id="c19cd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19cd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c19cd-111">Permission type</span></span>|<span data-ttu-id="c19cd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c19cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c19cd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c19cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c19cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c19cd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c19cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c19cd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c19cd-116">Not supported.</span></span>|
|<span data-ttu-id="c19cd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c19cd-117">Application</span></span>|<span data-ttu-id="c19cd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c19cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c19cd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c19cd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c19cd-120">Request headers</span></span>
|<span data-ttu-id="c19cd-121">Header</span><span class="sxs-lookup"><span data-stu-id="c19cd-121">Header</span></span>|<span data-ttu-id="c19cd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c19cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c19cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19cd-123">Authorization</span></span>|<span data-ttu-id="c19cd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c19cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c19cd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c19cd-125">Accept</span></span>|<span data-ttu-id="c19cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c19cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c19cd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c19cd-127">Request body</span></span>
<span data-ttu-id="c19cd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c19cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c19cd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19cd-129">Response</span></span>
<span data-ttu-id="c19cd-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c19cd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c19cd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c19cd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c19cd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19cd-132">Request</span></span>
<span data-ttu-id="c19cd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c19cd-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="c19cd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19cd-134">Response</span></span>
<span data-ttu-id="c19cd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c19cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






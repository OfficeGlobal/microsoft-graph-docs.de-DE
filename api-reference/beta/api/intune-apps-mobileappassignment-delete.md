---
title: mobileAppAssignment löschen
description: Löscht eine mobileAppAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 743588cf2cd04f176b23f8c6282c599b5aafb0fe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420507"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="f6397-103">mobileAppAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="f6397-103">Delete mobileAppAssignment</span></span>

> <span data-ttu-id="f6397-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f6397-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6397-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6397-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6397-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6397-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6397-107">Löscht eine [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f6397-107">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6397-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6397-108">Prerequisites</span></span>
<span data-ttu-id="f6397-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f6397-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6397-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6397-111">Permission type</span></span>|<span data-ttu-id="f6397-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6397-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6397-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6397-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6397-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6397-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6397-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6397-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6397-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6397-116">Not supported.</span></span>|
|<span data-ttu-id="f6397-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6397-117">Application</span></span>|<span data-ttu-id="f6397-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6397-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6397-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6397-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f6397-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6397-120">Request headers</span></span>
|<span data-ttu-id="f6397-121">Header</span><span class="sxs-lookup"><span data-stu-id="f6397-121">Header</span></span>|<span data-ttu-id="f6397-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f6397-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6397-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f6397-123">Authorization</span></span>|<span data-ttu-id="f6397-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6397-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6397-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6397-125">Accept</span></span>|<span data-ttu-id="f6397-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6397-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6397-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6397-127">Request body</span></span>
<span data-ttu-id="f6397-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6397-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6397-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6397-129">Response</span></span>
<span data-ttu-id="f6397-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6397-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6397-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6397-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6397-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6397-132">Request</span></span>
<span data-ttu-id="f6397-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6397-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f6397-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6397-134">Response</span></span>
<span data-ttu-id="f6397-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6397-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





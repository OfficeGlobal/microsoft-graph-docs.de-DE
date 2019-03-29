---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5a1177d5d6e8a7df83623d4efacd109947b220e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964122"
---
# <a name="assign-action"></a><span data-ttu-id="eecf2-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="eecf2-103">assign action</span></span>

> <span data-ttu-id="eecf2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eecf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eecf2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="eecf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eecf2-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eecf2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eecf2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eecf2-107">Prerequisites</span></span>
<span data-ttu-id="eecf2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eecf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecf2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eecf2-110">Permission type</span></span>|<span data-ttu-id="eecf2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eecf2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eecf2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eecf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eecf2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eecf2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eecf2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eecf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eecf2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eecf2-115">Not supported.</span></span>|
|<span data-ttu-id="eecf2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eecf2-116">Application</span></span>|<span data-ttu-id="eecf2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eecf2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eecf2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eecf2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="eecf2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eecf2-119">Request headers</span></span>
|<span data-ttu-id="eecf2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eecf2-120">Header</span></span>|<span data-ttu-id="eecf2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="eecf2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eecf2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eecf2-122">Authorization</span></span>|<span data-ttu-id="eecf2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eecf2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eecf2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eecf2-124">Accept</span></span>|<span data-ttu-id="eecf2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eecf2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eecf2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eecf2-126">Request body</span></span>
<span data-ttu-id="eecf2-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="eecf2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eecf2-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="eecf2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eecf2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eecf2-129">Property</span></span>|<span data-ttu-id="eecf2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="eecf2-130">Type</span></span>|<span data-ttu-id="eecf2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eecf2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eecf2-132">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="eecf2-132">mobileAppAssignments</span></span>|<span data-ttu-id="eecf2-133">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="eecf2-133">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="eecf2-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="eecf2-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eecf2-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="eecf2-135">Response</span></span>
<span data-ttu-id="eecf2-136">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eecf2-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eecf2-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eecf2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="eecf2-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eecf2-138">Request</span></span>
<span data-ttu-id="eecf2-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eecf2-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="eecf2-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="eecf2-140">Response</span></span>
<span data-ttu-id="eecf2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eecf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





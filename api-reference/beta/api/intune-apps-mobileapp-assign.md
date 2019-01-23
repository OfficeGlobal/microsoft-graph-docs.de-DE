---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 008d16fa6af0adff90606b1b88c3e98097b43b60
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420948"
---
# <a name="assign-action"></a><span data-ttu-id="05033-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="05033-103">assign action</span></span>

> <span data-ttu-id="05033-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="05033-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05033-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="05033-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05033-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="05033-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05033-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="05033-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05033-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="05033-108">Prerequisites</span></span>
<span data-ttu-id="05033-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="05033-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05033-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="05033-111">Permission type</span></span>|<span data-ttu-id="05033-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="05033-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05033-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="05033-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05033-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05033-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05033-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="05033-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05033-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05033-116">Not supported.</span></span>|
|<span data-ttu-id="05033-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="05033-117">Application</span></span>|<span data-ttu-id="05033-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="05033-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05033-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="05033-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/assign
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/assign
```

## <a name="request-headers"></a><span data-ttu-id="05033-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="05033-120">Request headers</span></span>
|<span data-ttu-id="05033-121">Header</span><span class="sxs-lookup"><span data-stu-id="05033-121">Header</span></span>|<span data-ttu-id="05033-122">Wert</span><span class="sxs-lookup"><span data-stu-id="05033-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05033-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="05033-123">Authorization</span></span>|<span data-ttu-id="05033-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="05033-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05033-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="05033-125">Accept</span></span>|<span data-ttu-id="05033-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05033-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05033-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="05033-127">Request body</span></span>
<span data-ttu-id="05033-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="05033-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05033-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="05033-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05033-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05033-130">Property</span></span>|<span data-ttu-id="05033-131">Typ</span><span class="sxs-lookup"><span data-stu-id="05033-131">Type</span></span>|<span data-ttu-id="05033-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05033-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05033-133">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="05033-133">mobileAppAssignments</span></span>|<span data-ttu-id="05033-134">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="05033-134">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="05033-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="05033-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05033-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="05033-136">Response</span></span>
<span data-ttu-id="05033-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="05033-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05033-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="05033-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="05033-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="05033-139">Request</span></span>
<span data-ttu-id="05033-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="05033-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05033-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="05033-141">Response</span></span>
<span data-ttu-id="05033-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="05033-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





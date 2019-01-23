---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ec08c34c6580643f47b4e09eb191031f6b29ef3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428891"
---
# <a name="assign-action"></a><span data-ttu-id="63ec7-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="63ec7-103">assign action</span></span>

> <span data-ttu-id="63ec7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="63ec7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63ec7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63ec7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63ec7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63ec7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63ec7-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="63ec7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63ec7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="63ec7-108">Prerequisites</span></span>
<span data-ttu-id="63ec7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="63ec7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63ec7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63ec7-111">Permission type</span></span>|<span data-ttu-id="63ec7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63ec7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63ec7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63ec7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63ec7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63ec7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63ec7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63ec7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63ec7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63ec7-116">Not supported.</span></span>|
|<span data-ttu-id="63ec7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63ec7-117">Application</span></span>|<span data-ttu-id="63ec7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63ec7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63ec7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63ec7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="63ec7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63ec7-120">Request headers</span></span>
|<span data-ttu-id="63ec7-121">Header</span><span class="sxs-lookup"><span data-stu-id="63ec7-121">Header</span></span>|<span data-ttu-id="63ec7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="63ec7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63ec7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="63ec7-123">Authorization</span></span>|<span data-ttu-id="63ec7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="63ec7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63ec7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="63ec7-125">Accept</span></span>|<span data-ttu-id="63ec7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63ec7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ec7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63ec7-127">Request body</span></span>
<span data-ttu-id="63ec7-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="63ec7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="63ec7-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="63ec7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="63ec7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="63ec7-130">Property</span></span>|<span data-ttu-id="63ec7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="63ec7-131">Type</span></span>|<span data-ttu-id="63ec7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63ec7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63ec7-133">assignments</span><span class="sxs-lookup"><span data-stu-id="63ec7-133">assignments</span></span>|<span data-ttu-id="63ec7-134">[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="63ec7-134">[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection</span></span>|<span data-ttu-id="63ec7-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="63ec7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="63ec7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="63ec7-136">Response</span></span>
<span data-ttu-id="63ec7-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="63ec7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63ec7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63ec7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="63ec7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63ec7-139">Request</span></span>
<span data-ttu-id="63ec7-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63ec7-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assign

Content-type: application/json
Content-length: 279

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="63ec7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="63ec7-141">Response</span></span>
<span data-ttu-id="63ec7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63ec7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





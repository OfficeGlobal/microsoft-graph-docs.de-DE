---
title: Liste intuneBrandingProfileAssignments
description: Listeneigenschaften und Beziehungen der IntuneBrandingProfileAssignment-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0ccb5ea075c0009dff5cad8b3ec265f24a2c052c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429966"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="6ed78-103">Liste intuneBrandingProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="6ed78-103">List intuneBrandingProfileAssignments</span></span>

> <span data-ttu-id="6ed78-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6ed78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ed78-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ed78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ed78-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ed78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ed78-107">Listeneigenschaften und Beziehungen der [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6ed78-107">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ed78-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6ed78-108">Prerequisites</span></span>
<span data-ttu-id="6ed78-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ed78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6ed78-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ed78-111">Permission type</span></span>|<span data-ttu-id="6ed78-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ed78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ed78-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ed78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ed78-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ed78-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6ed78-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ed78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ed78-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ed78-116">Not supported.</span></span>|
|<span data-ttu-id="6ed78-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ed78-117">Application</span></span>|<span data-ttu-id="6ed78-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ed78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ed78-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ed78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6ed78-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ed78-120">Request headers</span></span>
|<span data-ttu-id="6ed78-121">Header</span><span class="sxs-lookup"><span data-stu-id="6ed78-121">Header</span></span>|<span data-ttu-id="6ed78-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6ed78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ed78-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6ed78-123">Authorization</span></span>|<span data-ttu-id="6ed78-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6ed78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ed78-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6ed78-125">Accept</span></span>|<span data-ttu-id="6ed78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ed78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ed78-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ed78-127">Request body</span></span>
<span data-ttu-id="6ed78-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6ed78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ed78-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ed78-129">Response</span></span>
<span data-ttu-id="6ed78-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6ed78-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed78-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ed78-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ed78-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ed78-132">Request</span></span>
<span data-ttu-id="6ed78-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ed78-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="6ed78-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ed78-134">Response</span></span>
<span data-ttu-id="6ed78-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ed78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
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




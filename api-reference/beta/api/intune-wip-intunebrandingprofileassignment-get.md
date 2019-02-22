---
title: IntuneBrandingProfileAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des intuneBrandingProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7310c69494befa12ee45a440f0adbafcb824664c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154054"
---
# <a name="get-intunebrandingprofileassignment"></a><span data-ttu-id="6b77d-103">IntuneBrandingProfileAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="6b77d-103">Get intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="6b77d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b77d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b77d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6b77d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b77d-106">Lesen von Eigenschaften und Beziehungen des [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b77d-106">Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b77d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6b77d-107">Prerequisites</span></span>
<span data-ttu-id="6b77d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b77d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b77d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b77d-110">Permission type</span></span>|<span data-ttu-id="6b77d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b77d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b77d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b77d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b77d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b77d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b77d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b77d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b77d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b77d-115">Not supported.</span></span>|
|<span data-ttu-id="6b77d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b77d-116">Application</span></span>|<span data-ttu-id="6b77d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b77d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b77d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b77d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b77d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6b77d-119">Optional query parameters</span></span>
<span data-ttu-id="6b77d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b77d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b77d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b77d-121">Request headers</span></span>
|<span data-ttu-id="6b77d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6b77d-122">Header</span></span>|<span data-ttu-id="6b77d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6b77d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b77d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b77d-124">Authorization</span></span>|<span data-ttu-id="6b77d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6b77d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b77d-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6b77d-126">Accept</span></span>|<span data-ttu-id="6b77d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6b77d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b77d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b77d-128">Request body</span></span>
<span data-ttu-id="6b77d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b77d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b77d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b77d-130">Response</span></span>
<span data-ttu-id="6b77d-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6b77d-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b77d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b77d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b77d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b77d-133">Request</span></span>
<span data-ttu-id="6b77d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b77d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6b77d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b77d-135">Response</span></span>
<span data-ttu-id="6b77d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b77d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
    "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





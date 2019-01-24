---
title: IntuneBrandingProfileAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IntuneBrandingProfileAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7bfdba766221fc27dde6a8b71212620b744c4fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429967"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="c7ef0-103">IntuneBrandingProfileAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c7ef0-103">Update intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="c7ef0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7ef0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7ef0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ef0-107">Aktualisieren Sie die Eigenschaften eines [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7ef0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7ef0-108">Prerequisites</span></span>
<span data-ttu-id="c7ef0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7ef0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7ef0-111">Permission type</span></span>|<span data-ttu-id="c7ef0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7ef0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ef0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7ef0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ef0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ef0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7ef0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7ef0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ef0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7ef0-116">Not supported.</span></span>|
|<span data-ttu-id="c7ef0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7ef0-117">Application</span></span>|<span data-ttu-id="c7ef0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7ef0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ef0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7ef0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c7ef0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7ef0-120">Request headers</span></span>
|<span data-ttu-id="c7ef0-121">Header</span><span class="sxs-lookup"><span data-stu-id="c7ef0-121">Header</span></span>|<span data-ttu-id="c7ef0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c7ef0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7ef0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c7ef0-123">Authorization</span></span>|<span data-ttu-id="c7ef0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7ef0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7ef0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c7ef0-125">Accept</span></span>|<span data-ttu-id="c7ef0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7ef0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ef0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7ef0-127">Request body</span></span>
<span data-ttu-id="c7ef0-128">Geben Sie im Textkörper Anforderung für das Objekt [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="c7ef0-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="c7ef0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7ef0-130">Property</span></span>|<span data-ttu-id="c7ef0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c7ef0-131">Type</span></span>|<span data-ttu-id="c7ef0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7ef0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ef0-133">id</span><span class="sxs-lookup"><span data-stu-id="c7ef0-133">id</span></span>|<span data-ttu-id="c7ef0-134">String</span><span class="sxs-lookup"><span data-stu-id="c7ef0-134">String</span></span>|<span data-ttu-id="c7ef0-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="c7ef0-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c7ef0-136">target</span><span class="sxs-lookup"><span data-stu-id="c7ef0-136">target</span></span>|[<span data-ttu-id="c7ef0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c7ef0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c7ef0-138">Zuordnungsfeld Ziel an, die das branding Profil zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c7ef0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7ef0-139">Response</span></span>
<span data-ttu-id="c7ef0-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7ef0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7ef0-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7ef0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7ef0-142">Request</span></span>
<span data-ttu-id="c7ef0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c7ef0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7ef0-144">Response</span></span>
<span data-ttu-id="c7ef0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7ef0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




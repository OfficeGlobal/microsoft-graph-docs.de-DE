---
title: IntuneBrandingProfileAssignment erstellen
description: Erstellen eines neuen intuneBrandingProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97e8743b93ab0ce89f43d7714c7bf9aa12d81b06
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960552"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="ea35f-103">IntuneBrandingProfileAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="ea35f-103">Create intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="ea35f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea35f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea35f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea35f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea35f-106">Erstellen eines neuen [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea35f-106">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea35f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea35f-107">Prerequisites</span></span>
<span data-ttu-id="ea35f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea35f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea35f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea35f-110">Permission type</span></span>|<span data-ttu-id="ea35f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea35f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea35f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea35f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea35f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea35f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea35f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea35f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea35f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea35f-115">Not supported.</span></span>|
|<span data-ttu-id="ea35f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea35f-116">Application</span></span>|<span data-ttu-id="ea35f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea35f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea35f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea35f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ea35f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea35f-119">Request headers</span></span>
|<span data-ttu-id="ea35f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ea35f-120">Header</span></span>|<span data-ttu-id="ea35f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ea35f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea35f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea35f-122">Authorization</span></span>|<span data-ttu-id="ea35f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea35f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea35f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea35f-124">Accept</span></span>|<span data-ttu-id="ea35f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea35f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea35f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea35f-126">Request body</span></span>
<span data-ttu-id="ea35f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das intuneBrandingProfileAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ea35f-127">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="ea35f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der intuneBrandingProfileAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ea35f-128">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="ea35f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea35f-129">Property</span></span>|<span data-ttu-id="ea35f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ea35f-130">Type</span></span>|<span data-ttu-id="ea35f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea35f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea35f-132">id</span><span class="sxs-lookup"><span data-stu-id="ea35f-132">id</span></span>|<span data-ttu-id="ea35f-133">String</span><span class="sxs-lookup"><span data-stu-id="ea35f-133">String</span></span>|<span data-ttu-id="ea35f-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="ea35f-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ea35f-135">target</span><span class="sxs-lookup"><span data-stu-id="ea35f-135">target</span></span>|[<span data-ttu-id="ea35f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ea35f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ea35f-137">Zuordnungsziel, dem das Branding-Profil zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ea35f-137">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="ea35f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea35f-138">Response</span></span>
<span data-ttu-id="ea35f-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ea35f-139">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea35f-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea35f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea35f-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea35f-141">Request</span></span>
<span data-ttu-id="ea35f-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea35f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ea35f-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea35f-143">Response</span></span>
<span data-ttu-id="ea35f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea35f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





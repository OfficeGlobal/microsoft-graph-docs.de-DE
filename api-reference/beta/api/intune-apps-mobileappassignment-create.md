---
title: Erstellen von „mobileAppAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ceae2f0bacac3d83532a6aa9b338c32573d6332
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874655"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="393ec-103">Erstellen von „mobileAppAssignment“</span><span class="sxs-lookup"><span data-stu-id="393ec-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="393ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="393ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="393ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="393ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="393ec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="393ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="393ec-107">Diese Methode erstellt ein neues Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="393ec-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="393ec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="393ec-108">Prerequisites</span></span>
<span data-ttu-id="393ec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="393ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="393ec-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="393ec-111">Permission type</span></span>|<span data-ttu-id="393ec-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="393ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="393ec-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="393ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="393ec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="393ec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="393ec-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="393ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="393ec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="393ec-116">Not supported.</span></span>|
|<span data-ttu-id="393ec-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="393ec-117">Application</span></span>|<span data-ttu-id="393ec-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="393ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="393ec-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="393ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="393ec-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="393ec-120">Request headers</span></span>
|<span data-ttu-id="393ec-121">Header</span><span class="sxs-lookup"><span data-stu-id="393ec-121">Header</span></span>|<span data-ttu-id="393ec-122">Wert</span><span class="sxs-lookup"><span data-stu-id="393ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="393ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="393ec-123">Authorization</span></span>|<span data-ttu-id="393ec-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="393ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="393ec-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="393ec-125">Accept</span></span>|<span data-ttu-id="393ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="393ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="393ec-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="393ec-127">Request body</span></span>
<span data-ttu-id="393ec-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „mobileAppAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="393ec-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="393ec-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „mobileAppAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="393ec-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="393ec-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="393ec-130">Property</span></span>|<span data-ttu-id="393ec-131">Typ</span><span class="sxs-lookup"><span data-stu-id="393ec-131">Type</span></span>|<span data-ttu-id="393ec-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="393ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393ec-133">id</span><span class="sxs-lookup"><span data-stu-id="393ec-133">id</span></span>|<span data-ttu-id="393ec-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="393ec-134">String</span></span>|<span data-ttu-id="393ec-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="393ec-135">Key of the entity.</span></span>|
|<span data-ttu-id="393ec-136">intent</span><span class="sxs-lookup"><span data-stu-id="393ec-136">intent</span></span>|[<span data-ttu-id="393ec-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="393ec-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="393ec-138">Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="393ec-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="393ec-139">target</span><span class="sxs-lookup"><span data-stu-id="393ec-139">target</span></span>|[<span data-ttu-id="393ec-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="393ec-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="393ec-141">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="393ec-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="393ec-142">settings</span><span class="sxs-lookup"><span data-stu-id="393ec-142">settings</span></span>|[<span data-ttu-id="393ec-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="393ec-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="393ec-144">Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="393ec-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="393ec-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="393ec-145">Response</span></span>
<span data-ttu-id="393ec-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="393ec-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="393ec-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="393ec-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="393ec-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="393ec-148">Request</span></span>
<span data-ttu-id="393ec-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="393ec-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="393ec-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="393ec-150">Response</span></span>
<span data-ttu-id="393ec-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="393ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

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
```






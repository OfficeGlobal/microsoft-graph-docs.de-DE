---
title: EmbeddedSIMActivationCodePoolAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EmbeddedSIMActivationCodePoolAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b893ac21367ba96f66c4a2ba9ee20240225fcea1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824452"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="bb376-103">EmbeddedSIMActivationCodePoolAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bb376-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="bb376-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb376-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb376-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb376-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb376-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bb376-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb376-107">Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb376-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb376-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bb376-108">Prerequisites</span></span>
<span data-ttu-id="bb376-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb376-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb376-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb376-111">Permission type</span></span>|<span data-ttu-id="bb376-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb376-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb376-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb376-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb376-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb376-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb376-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb376-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb376-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb376-116">Not supported.</span></span>|
|<span data-ttu-id="bb376-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb376-117">Application</span></span>|<span data-ttu-id="bb376-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb376-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb376-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb376-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bb376-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb376-120">Request headers</span></span>
|<span data-ttu-id="bb376-121">Header</span><span class="sxs-lookup"><span data-stu-id="bb376-121">Header</span></span>|<span data-ttu-id="bb376-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bb376-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb376-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb376-123">Authorization</span></span>|<span data-ttu-id="bb376-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bb376-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb376-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bb376-125">Accept</span></span>|<span data-ttu-id="bb376-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb376-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb376-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb376-127">Request body</span></span>
<span data-ttu-id="bb376-128">Geben Sie im Textkörper Anforderung für das Objekt [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bb376-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="bb376-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb376-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="bb376-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb376-130">Property</span></span>|<span data-ttu-id="bb376-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bb376-131">Type</span></span>|<span data-ttu-id="bb376-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb376-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb376-133">id</span><span class="sxs-lookup"><span data-stu-id="bb376-133">id</span></span>|<span data-ttu-id="bb376-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb376-134">String</span></span>|<span data-ttu-id="bb376-135">Eindeutiger Bezeichner für die eingebettete SIM Aktivierung Code Pool Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="bb376-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="bb376-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="bb376-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="bb376-137">target</span><span class="sxs-lookup"><span data-stu-id="bb376-137">target</span></span>|[<span data-ttu-id="bb376-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb376-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bb376-139">Der Typ der Zielgruppen vom eingebetteten SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="bb376-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="bb376-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb376-140">Response</span></span>
<span data-ttu-id="bb376-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bb376-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb376-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb376-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb376-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb376-143">Request</span></span>
<span data-ttu-id="bb376-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb376-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="bb376-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb376-145">Response</span></span>
<span data-ttu-id="bb376-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb376-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






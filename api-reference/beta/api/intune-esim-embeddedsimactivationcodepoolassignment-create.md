---
title: Erstellen von embeddedSIMActivationCodePoolAssignment
description: Erstellen eines neuen EmbeddedSIMActivationCodePoolAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e020dafec47fe1a669251825ba0dff75f41f382c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865933"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="0c70b-103">Erstellen von embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="0c70b-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="0c70b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0c70b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c70b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c70b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c70b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0c70b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c70b-107">Erstellen eines neuen [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c70b-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c70b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c70b-108">Prerequisites</span></span>
<span data-ttu-id="0c70b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c70b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c70b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c70b-111">Permission type</span></span>|<span data-ttu-id="0c70b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c70b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c70b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c70b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c70b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c70b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c70b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c70b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c70b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c70b-116">Not supported.</span></span>|
|<span data-ttu-id="0c70b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c70b-117">Application</span></span>|<span data-ttu-id="0c70b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c70b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c70b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c70b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0c70b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c70b-120">Request headers</span></span>
|<span data-ttu-id="0c70b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0c70b-121">Header</span></span>|<span data-ttu-id="0c70b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0c70b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c70b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c70b-123">Authorization</span></span>|<span data-ttu-id="0c70b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c70b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c70b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c70b-125">Accept</span></span>|<span data-ttu-id="0c70b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c70b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c70b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c70b-127">Request body</span></span>
<span data-ttu-id="0c70b-128">Geben Sie im Textkörper Anforderung für das Objekt EmbeddedSIMActivationCodePoolAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0c70b-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="0c70b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die EmbeddedSIMActivationCodePoolAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="0c70b-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="0c70b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c70b-130">Property</span></span>|<span data-ttu-id="0c70b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0c70b-131">Type</span></span>|<span data-ttu-id="0c70b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c70b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c70b-133">id</span><span class="sxs-lookup"><span data-stu-id="0c70b-133">id</span></span>|<span data-ttu-id="0c70b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c70b-134">String</span></span>|<span data-ttu-id="0c70b-135">Eindeutiger Bezeichner für die eingebettete SIM Aktivierung Code Pool Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="0c70b-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="0c70b-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="0c70b-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0c70b-137">target</span><span class="sxs-lookup"><span data-stu-id="0c70b-137">target</span></span>|[<span data-ttu-id="0c70b-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0c70b-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0c70b-139">Der Typ der Zielgruppen vom eingebetteten SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="0c70b-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="0c70b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c70b-140">Response</span></span>
<span data-ttu-id="0c70b-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0c70b-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c70b-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c70b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c70b-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c70b-143">Request</span></span>
<span data-ttu-id="0c70b-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c70b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="0c70b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c70b-145">Response</span></span>
<span data-ttu-id="0c70b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c70b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






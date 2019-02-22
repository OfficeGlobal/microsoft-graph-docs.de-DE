---
title: GroupPolicyPresentationValueBoolean aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValueBoolean-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 656e7f358023a7e5294fe1ab84e58492848806b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152675"
---
# <a name="update-grouppolicypresentationvalueboolean"></a><span data-ttu-id="65e7e-103">GroupPolicyPresentationValueBoolean aktualisieren</span><span class="sxs-lookup"><span data-stu-id="65e7e-103">Update groupPolicyPresentationValueBoolean</span></span>

> <span data-ttu-id="65e7e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65e7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65e7e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="65e7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e7e-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="65e7e-106">Update the properties of a [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65e7e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="65e7e-107">Prerequisites</span></span>
<span data-ttu-id="65e7e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="65e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="65e7e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65e7e-110">Permission type</span></span>|<span data-ttu-id="65e7e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65e7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65e7e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65e7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65e7e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65e7e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65e7e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65e7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65e7e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e7e-115">Not supported.</span></span>|
|<span data-ttu-id="65e7e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65e7e-116">Application</span></span>|<span data-ttu-id="65e7e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65e7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65e7e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="65e7e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65e7e-119">Request headers</span></span>
|<span data-ttu-id="65e7e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="65e7e-120">Header</span></span>|<span data-ttu-id="65e7e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="65e7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65e7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65e7e-122">Authorization</span></span>|<span data-ttu-id="65e7e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="65e7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65e7e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="65e7e-124">Accept</span></span>|<span data-ttu-id="65e7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65e7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65e7e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65e7e-126">Request body</span></span>
<span data-ttu-id="65e7e-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="65e7e-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object.</span></span>

<span data-ttu-id="65e7e-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="65e7e-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).</span></span>

|<span data-ttu-id="65e7e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65e7e-129">Property</span></span>|<span data-ttu-id="65e7e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="65e7e-130">Type</span></span>|<span data-ttu-id="65e7e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65e7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e7e-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65e7e-132">lastModifiedDateTime</span></span>|<span data-ttu-id="65e7e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e7e-133">DateTimeOffset</span></span>|<span data-ttu-id="65e7e-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65e7e-134">The date and time the object was last modified.</span></span> <span data-ttu-id="65e7e-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="65e7e-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="65e7e-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65e7e-136">createdDateTime</span></span>|<span data-ttu-id="65e7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65e7e-137">DateTimeOffset</span></span>|<span data-ttu-id="65e7e-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="65e7e-138">The date and time the object was created.</span></span> <span data-ttu-id="65e7e-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="65e7e-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="65e7e-140">id</span><span class="sxs-lookup"><span data-stu-id="65e7e-140">id</span></span>|<span data-ttu-id="65e7e-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65e7e-141">String</span></span>|<span data-ttu-id="65e7e-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="65e7e-142">Key of the entity.</span></span> <span data-ttu-id="65e7e-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="65e7e-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="65e7e-144">Wert</span><span class="sxs-lookup"><span data-stu-id="65e7e-144">value</span></span>|<span data-ttu-id="65e7e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="65e7e-145">Boolean</span></span>|<span data-ttu-id="65e7e-146">Ein boolescher Wert für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="65e7e-146">An boolean value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="65e7e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e7e-147">Response</span></span>
<span data-ttu-id="65e7e-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="65e7e-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65e7e-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65e7e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="65e7e-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65e7e-150">Request</span></span>
<span data-ttu-id="65e7e-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65e7e-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 95

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="65e7e-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="65e7e-152">Response</span></span>
<span data-ttu-id="65e7e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65e7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "be61344f-344f-be61-4f34-61be4f3461be",
  "value": true
}
```





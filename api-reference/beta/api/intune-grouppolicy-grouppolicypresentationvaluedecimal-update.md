---
title: GroupPolicyPresentationValueDecimal aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValueDecimal-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39d9fe3e0a6d9e54d951f1ee8bcf80f53ee1575f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152346"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="47e15-103">GroupPolicyPresentationValueDecimal aktualisieren</span><span class="sxs-lookup"><span data-stu-id="47e15-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="47e15-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47e15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47e15-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="47e15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e15-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="47e15-106">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47e15-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47e15-107">Prerequisites</span></span>
<span data-ttu-id="47e15-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47e15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47e15-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47e15-110">Permission type</span></span>|<span data-ttu-id="47e15-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47e15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47e15-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47e15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47e15-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e15-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47e15-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47e15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47e15-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47e15-115">Not supported.</span></span>|
|<span data-ttu-id="47e15-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47e15-116">Application</span></span>|<span data-ttu-id="47e15-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47e15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47e15-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47e15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="47e15-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47e15-119">Request headers</span></span>
|<span data-ttu-id="47e15-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47e15-120">Header</span></span>|<span data-ttu-id="47e15-121">Wert</span><span class="sxs-lookup"><span data-stu-id="47e15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47e15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47e15-122">Authorization</span></span>|<span data-ttu-id="47e15-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47e15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47e15-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47e15-124">Accept</span></span>|<span data-ttu-id="47e15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47e15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47e15-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47e15-126">Request body</span></span>
<span data-ttu-id="47e15-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="47e15-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="47e15-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="47e15-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="47e15-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47e15-129">Property</span></span>|<span data-ttu-id="47e15-130">Typ</span><span class="sxs-lookup"><span data-stu-id="47e15-130">Type</span></span>|<span data-ttu-id="47e15-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="47e15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e15-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47e15-132">lastModifiedDateTime</span></span>|<span data-ttu-id="47e15-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47e15-133">DateTimeOffset</span></span>|<span data-ttu-id="47e15-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="47e15-134">The date and time the object was last modified.</span></span> <span data-ttu-id="47e15-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="47e15-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="47e15-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47e15-136">createdDateTime</span></span>|<span data-ttu-id="47e15-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47e15-137">DateTimeOffset</span></span>|<span data-ttu-id="47e15-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="47e15-138">The date and time the object was created.</span></span> <span data-ttu-id="47e15-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="47e15-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="47e15-140">id</span><span class="sxs-lookup"><span data-stu-id="47e15-140">id</span></span>|<span data-ttu-id="47e15-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="47e15-141">String</span></span>|<span data-ttu-id="47e15-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="47e15-142">Key of the entity.</span></span> <span data-ttu-id="47e15-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="47e15-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="47e15-144">Wert</span><span class="sxs-lookup"><span data-stu-id="47e15-144">value</span></span>|<span data-ttu-id="47e15-145">Int64</span><span class="sxs-lookup"><span data-stu-id="47e15-145">Int64</span></span>|<span data-ttu-id="47e15-146">Ein ganzzahliger Wert ohne Vorzeichen für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="47e15-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="47e15-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="47e15-147">Response</span></span>
<span data-ttu-id="47e15-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47e15-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47e15-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47e15-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="47e15-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47e15-150">Request</span></span>
<span data-ttu-id="47e15-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47e15-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="47e15-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="47e15-152">Response</span></span>
<span data-ttu-id="47e15-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47e15-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```





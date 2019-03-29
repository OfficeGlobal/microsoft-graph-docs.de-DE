---
title: GroupPolicyPresentationText aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bc14acab2d290e2716dba471d2c6d37d8c1ebe6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967209"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="3fb59-103">GroupPolicyPresentationText aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3fb59-103">Update groupPolicyPresentationText</span></span>

> <span data-ttu-id="3fb59-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3fb59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fb59-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3fb59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb59-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3fb59-106">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fb59-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3fb59-107">Prerequisites</span></span>
<span data-ttu-id="3fb59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fb59-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3fb59-110">Permission type</span></span>|<span data-ttu-id="3fb59-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3fb59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb59-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3fb59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb59-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fb59-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3fb59-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3fb59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb59-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fb59-115">Not supported.</span></span>|
|<span data-ttu-id="3fb59-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3fb59-116">Application</span></span>|<span data-ttu-id="3fb59-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3fb59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb59-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fb59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="3fb59-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3fb59-119">Request headers</span></span>
|<span data-ttu-id="3fb59-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3fb59-120">Header</span></span>|<span data-ttu-id="3fb59-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3fb59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb59-122">Authorization</span></span>|<span data-ttu-id="3fb59-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3fb59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb59-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3fb59-124">Accept</span></span>|<span data-ttu-id="3fb59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb59-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3fb59-126">Request body</span></span>
<span data-ttu-id="3fb59-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3fb59-127">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="3fb59-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3fb59-128">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="3fb59-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3fb59-129">Property</span></span>|<span data-ttu-id="3fb59-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3fb59-130">Type</span></span>|<span data-ttu-id="3fb59-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fb59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb59-132">label</span><span class="sxs-lookup"><span data-stu-id="3fb59-132">label</span></span>|<span data-ttu-id="3fb59-133">String</span><span class="sxs-lookup"><span data-stu-id="3fb59-133">String</span></span>|<span data-ttu-id="3fb59-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="3fb59-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3fb59-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="3fb59-135">The default value is empty.</span></span> <span data-ttu-id="3fb59-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3fb59-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3fb59-137">id</span><span class="sxs-lookup"><span data-stu-id="3fb59-137">id</span></span>|<span data-ttu-id="3fb59-138">String</span><span class="sxs-lookup"><span data-stu-id="3fb59-138">String</span></span>|<span data-ttu-id="3fb59-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3fb59-139">Key of the entity.</span></span> <span data-ttu-id="3fb59-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3fb59-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3fb59-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb59-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3fb59-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb59-142">DateTimeOffset</span></span>|<span data-ttu-id="3fb59-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="3fb59-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="3fb59-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3fb59-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3fb59-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fb59-145">Response</span></span>
<span data-ttu-id="3fb59-146">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3fb59-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb59-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3fb59-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fb59-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3fb59-148">Request</span></span>
<span data-ttu-id="3fb59-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3fb59-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="3fb59-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="3fb59-150">Response</span></span>
<span data-ttu-id="3fb59-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3fb59-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





---
title: GroupPolicyPresentationText erstellen
description: Erstellen eines neuen groupPolicyPresentationText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85e7260839c7755b00e555c3a3da4877cd8489e8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962897"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="b426d-103">GroupPolicyPresentationText erstellen</span><span class="sxs-lookup"><span data-stu-id="b426d-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="b426d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b426d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b426d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b426d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b426d-106">Erstellen eines neuen [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b426d-106">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b426d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b426d-107">Prerequisites</span></span>
<span data-ttu-id="b426d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b426d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b426d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b426d-110">Permission type</span></span>|<span data-ttu-id="b426d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b426d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b426d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b426d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b426d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b426d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b426d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b426d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b426d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b426d-115">Not supported.</span></span>|
|<span data-ttu-id="b426d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b426d-116">Application</span></span>|<span data-ttu-id="b426d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b426d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b426d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b426d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="b426d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b426d-119">Request headers</span></span>
|<span data-ttu-id="b426d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b426d-120">Header</span></span>|<span data-ttu-id="b426d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b426d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b426d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b426d-122">Authorization</span></span>|<span data-ttu-id="b426d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b426d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b426d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b426d-124">Accept</span></span>|<span data-ttu-id="b426d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b426d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b426d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b426d-126">Request body</span></span>
<span data-ttu-id="b426d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationText-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b426d-127">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="b426d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationText erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b426d-128">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="b426d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b426d-129">Property</span></span>|<span data-ttu-id="b426d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b426d-130">Type</span></span>|<span data-ttu-id="b426d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b426d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b426d-132">label</span><span class="sxs-lookup"><span data-stu-id="b426d-132">label</span></span>|<span data-ttu-id="b426d-133">String</span><span class="sxs-lookup"><span data-stu-id="b426d-133">String</span></span>|<span data-ttu-id="b426d-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="b426d-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b426d-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="b426d-135">The default value is empty.</span></span> <span data-ttu-id="b426d-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b426d-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b426d-137">id</span><span class="sxs-lookup"><span data-stu-id="b426d-137">id</span></span>|<span data-ttu-id="b426d-138">String</span><span class="sxs-lookup"><span data-stu-id="b426d-138">String</span></span>|<span data-ttu-id="b426d-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b426d-139">Key of the entity.</span></span> <span data-ttu-id="b426d-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b426d-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b426d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b426d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b426d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b426d-142">DateTimeOffset</span></span>|<span data-ttu-id="b426d-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="b426d-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="b426d-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b426d-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b426d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b426d-145">Response</span></span>
<span data-ttu-id="b426d-146">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b426d-146">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b426d-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b426d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b426d-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b426d-148">Request</span></span>
<span data-ttu-id="b426d-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b426d-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="b426d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b426d-150">Response</span></span>
<span data-ttu-id="b426d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b426d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





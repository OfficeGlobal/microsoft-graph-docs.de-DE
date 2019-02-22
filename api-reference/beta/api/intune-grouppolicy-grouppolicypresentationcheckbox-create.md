---
title: GroupPolicyPresentationCheckBox erstellen
description: Erstellen eines neuen groupPolicyPresentationCheckBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6704ca00d90bab5679e0ab3bc5840272a6d0bc6e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159647"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="6c75b-103">GroupPolicyPresentationCheckBox erstellen</span><span class="sxs-lookup"><span data-stu-id="6c75b-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="6c75b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c75b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c75b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c75b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c75b-106">Erstellen eines neuen [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c75b-106">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c75b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c75b-107">Prerequisites</span></span>
<span data-ttu-id="6c75b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c75b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c75b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c75b-110">Permission type</span></span>|<span data-ttu-id="6c75b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c75b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c75b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c75b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c75b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c75b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c75b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c75b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c75b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c75b-115">Not supported.</span></span>|
|<span data-ttu-id="6c75b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c75b-116">Application</span></span>|<span data-ttu-id="6c75b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c75b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c75b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c75b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="6c75b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c75b-119">Request headers</span></span>
|<span data-ttu-id="6c75b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c75b-120">Header</span></span>|<span data-ttu-id="6c75b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6c75b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c75b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c75b-122">Authorization</span></span>|<span data-ttu-id="6c75b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c75b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c75b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6c75b-124">Accept</span></span>|<span data-ttu-id="6c75b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c75b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c75b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c75b-126">Request body</span></span>
<span data-ttu-id="6c75b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationCheckBox-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6c75b-127">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="6c75b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationCheckBox erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6c75b-128">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="6c75b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c75b-129">Property</span></span>|<span data-ttu-id="6c75b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6c75b-130">Type</span></span>|<span data-ttu-id="6c75b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c75b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c75b-132">label</span><span class="sxs-lookup"><span data-stu-id="6c75b-132">label</span></span>|<span data-ttu-id="6c75b-133">String</span><span class="sxs-lookup"><span data-stu-id="6c75b-133">String</span></span>|<span data-ttu-id="6c75b-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="6c75b-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6c75b-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="6c75b-135">The default value is empty.</span></span> <span data-ttu-id="6c75b-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6c75b-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6c75b-137">id</span><span class="sxs-lookup"><span data-stu-id="6c75b-137">id</span></span>|<span data-ttu-id="6c75b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c75b-138">String</span></span>|<span data-ttu-id="6c75b-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c75b-139">Key of the entity.</span></span> <span data-ttu-id="6c75b-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6c75b-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6c75b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c75b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6c75b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c75b-142">DateTimeOffset</span></span>|<span data-ttu-id="6c75b-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="6c75b-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6c75b-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6c75b-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6c75b-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="6c75b-145">defaultChecked</span></span>|<span data-ttu-id="6c75b-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c75b-146">Boolean</span></span>|<span data-ttu-id="6c75b-147">Standardwert für das Kontrollkästchen.</span><span class="sxs-lookup"><span data-stu-id="6c75b-147">Default value for the check box.</span></span> <span data-ttu-id="6c75b-148">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="6c75b-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="6c75b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c75b-149">Response</span></span>
<span data-ttu-id="6c75b-150">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c75b-150">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c75b-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c75b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c75b-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c75b-152">Request</span></span>
<span data-ttu-id="6c75b-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c75b-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="6c75b-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c75b-154">Response</span></span>
<span data-ttu-id="6c75b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c75b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```





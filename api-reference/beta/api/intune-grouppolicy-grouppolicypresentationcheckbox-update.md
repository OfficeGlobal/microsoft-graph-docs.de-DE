---
title: GroupPolicyPresentationCheckBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationCheckBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92f5af7496dda48aced995e33e077be7fa6ff5f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962393"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="9cbfb-103">GroupPolicyPresentationCheckBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9cbfb-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="9cbfb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cbfb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbfb-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-106">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cbfb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9cbfb-107">Prerequisites</span></span>
<span data-ttu-id="9cbfb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cbfb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9cbfb-110">Permission type</span></span>|<span data-ttu-id="9cbfb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cbfb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9cbfb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cbfb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9cbfb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cbfb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cbfb-115">Not supported.</span></span>|
|<span data-ttu-id="9cbfb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9cbfb-116">Application</span></span>|<span data-ttu-id="9cbfb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cbfb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cbfb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cbfb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="9cbfb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9cbfb-119">Request headers</span></span>
|<span data-ttu-id="9cbfb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9cbfb-120">Header</span></span>|<span data-ttu-id="9cbfb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9cbfb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cbfb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cbfb-122">Authorization</span></span>|<span data-ttu-id="9cbfb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9cbfb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cbfb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9cbfb-124">Accept</span></span>|<span data-ttu-id="9cbfb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9cbfb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cbfb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9cbfb-126">Request body</span></span>
<span data-ttu-id="9cbfb-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-127">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="9cbfb-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-128">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="9cbfb-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cbfb-129">Property</span></span>|<span data-ttu-id="9cbfb-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9cbfb-130">Type</span></span>|<span data-ttu-id="9cbfb-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cbfb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbfb-132">label</span><span class="sxs-lookup"><span data-stu-id="9cbfb-132">label</span></span>|<span data-ttu-id="9cbfb-133">String</span><span class="sxs-lookup"><span data-stu-id="9cbfb-133">String</span></span>|<span data-ttu-id="9cbfb-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9cbfb-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-135">The default value is empty.</span></span> <span data-ttu-id="9cbfb-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9cbfb-137">id</span><span class="sxs-lookup"><span data-stu-id="9cbfb-137">id</span></span>|<span data-ttu-id="9cbfb-138">String</span><span class="sxs-lookup"><span data-stu-id="9cbfb-138">String</span></span>|<span data-ttu-id="9cbfb-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9cbfb-139">Key of the entity.</span></span> <span data-ttu-id="9cbfb-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9cbfb-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cbfb-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9cbfb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cbfb-142">DateTimeOffset</span></span>|<span data-ttu-id="9cbfb-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="9cbfb-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9cbfb-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9cbfb-145">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="9cbfb-145">defaultChecked</span></span>|<span data-ttu-id="9cbfb-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9cbfb-146">Boolean</span></span>|<span data-ttu-id="9cbfb-147">Standardwert für das Kontrollkästchen.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-147">Default value for the check box.</span></span> <span data-ttu-id="9cbfb-148">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="9cbfb-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cbfb-149">Response</span></span>
<span data-ttu-id="9cbfb-150">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cbfb-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cbfb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cbfb-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cbfb-152">Request</span></span>
<span data-ttu-id="9cbfb-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="9cbfb-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cbfb-154">Response</span></span>
<span data-ttu-id="9cbfb-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cbfb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





---
title: GroupPolicyPresentationComboBox erstellen
description: Erstellen eines neuen groupPolicyPresentationComboBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30952aa522378b3c8a881ddb6549e8a48946f493
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975968"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="893a8-103">GroupPolicyPresentationComboBox erstellen</span><span class="sxs-lookup"><span data-stu-id="893a8-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="893a8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="893a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="893a8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="893a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="893a8-106">Erstellen eines neuen [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="893a8-106">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="893a8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="893a8-107">Prerequisites</span></span>
<span data-ttu-id="893a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="893a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="893a8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="893a8-110">Permission type</span></span>|<span data-ttu-id="893a8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="893a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="893a8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="893a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="893a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="893a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="893a8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="893a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="893a8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="893a8-115">Not supported.</span></span>|
|<span data-ttu-id="893a8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="893a8-116">Application</span></span>|<span data-ttu-id="893a8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="893a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="893a8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="893a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="893a8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="893a8-119">Request headers</span></span>
|<span data-ttu-id="893a8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="893a8-120">Header</span></span>|<span data-ttu-id="893a8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="893a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="893a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="893a8-122">Authorization</span></span>|<span data-ttu-id="893a8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="893a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="893a8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="893a8-124">Accept</span></span>|<span data-ttu-id="893a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="893a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="893a8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="893a8-126">Request body</span></span>
<span data-ttu-id="893a8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationComboBox-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="893a8-127">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="893a8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationComboBox erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="893a8-128">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="893a8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="893a8-129">Property</span></span>|<span data-ttu-id="893a8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="893a8-130">Type</span></span>|<span data-ttu-id="893a8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="893a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893a8-132">label</span><span class="sxs-lookup"><span data-stu-id="893a8-132">label</span></span>|<span data-ttu-id="893a8-133">String</span><span class="sxs-lookup"><span data-stu-id="893a8-133">String</span></span>|<span data-ttu-id="893a8-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="893a8-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="893a8-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="893a8-135">The default value is empty.</span></span> <span data-ttu-id="893a8-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="893a8-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="893a8-137">id</span><span class="sxs-lookup"><span data-stu-id="893a8-137">id</span></span>|<span data-ttu-id="893a8-138">String</span><span class="sxs-lookup"><span data-stu-id="893a8-138">String</span></span>|<span data-ttu-id="893a8-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="893a8-139">Key of the entity.</span></span> <span data-ttu-id="893a8-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="893a8-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="893a8-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="893a8-141">lastModifiedDateTime</span></span>|<span data-ttu-id="893a8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="893a8-142">DateTimeOffset</span></span>|<span data-ttu-id="893a8-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="893a8-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="893a8-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="893a8-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="893a8-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="893a8-145">defaultValue</span></span>|<span data-ttu-id="893a8-146">String</span><span class="sxs-lookup"><span data-stu-id="893a8-146">String</span></span>|<span data-ttu-id="893a8-147">Im Kombinationsfeld angezeigte lokalisierte Standardzeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="893a8-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="893a8-148">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="893a8-148">The default value is empty.</span></span>|
|<span data-ttu-id="893a8-149">Vorschläge</span><span class="sxs-lookup"><span data-stu-id="893a8-149">suggestions</span></span>|<span data-ttu-id="893a8-150">String collection</span><span class="sxs-lookup"><span data-stu-id="893a8-150">String collection</span></span>|<span data-ttu-id="893a8-151">Lokalisierte Zeichenfolgen, die in der Dropdownliste des Kombinationsfelds aufgeführt sind.</span><span class="sxs-lookup"><span data-stu-id="893a8-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="893a8-152">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="893a8-152">The default value is empty.</span></span>|
|<span data-ttu-id="893a8-153">erforderlich</span><span class="sxs-lookup"><span data-stu-id="893a8-153">required</span></span>|<span data-ttu-id="893a8-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="893a8-154">Boolean</span></span>|<span data-ttu-id="893a8-155">Gibt an, ob ein Wert für den Parameter angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="893a8-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="893a8-156">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="893a8-156">The default value is false.</span></span>|
|<span data-ttu-id="893a8-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="893a8-157">maxLength</span></span>|<span data-ttu-id="893a8-158">Int64</span><span class="sxs-lookup"><span data-stu-id="893a8-158">Int64</span></span>|<span data-ttu-id="893a8-159">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen für den Parameter angibt.</span><span class="sxs-lookup"><span data-stu-id="893a8-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="893a8-160">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="893a8-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="893a8-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="893a8-161">Response</span></span>
<span data-ttu-id="893a8-162">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="893a8-162">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="893a8-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="893a8-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="893a8-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="893a8-164">Request</span></span>
<span data-ttu-id="893a8-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="893a8-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="893a8-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="893a8-166">Response</span></span>
<span data-ttu-id="893a8-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="893a8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```





---
title: GroupPolicyPresentationComboBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationComboBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 404bb813d37c01186e694765dfed3c7809e02058
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149392"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="4a30c-103">GroupPolicyPresentationComboBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4a30c-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="4a30c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a30c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a30c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4a30c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a30c-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a30c-106">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a30c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a30c-107">Prerequisites</span></span>
<span data-ttu-id="4a30c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a30c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a30c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a30c-110">Permission type</span></span>|<span data-ttu-id="4a30c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a30c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a30c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a30c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a30c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a30c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a30c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a30c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a30c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a30c-115">Not supported.</span></span>|
|<span data-ttu-id="4a30c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a30c-116">Application</span></span>|<span data-ttu-id="4a30c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a30c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a30c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a30c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a30c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a30c-119">Request headers</span></span>
|<span data-ttu-id="4a30c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4a30c-120">Header</span></span>|<span data-ttu-id="4a30c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4a30c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a30c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a30c-122">Authorization</span></span>|<span data-ttu-id="4a30c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a30c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a30c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a30c-124">Accept</span></span>|<span data-ttu-id="4a30c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a30c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a30c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a30c-126">Request body</span></span>
<span data-ttu-id="4a30c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4a30c-127">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="4a30c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4a30c-128">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="4a30c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a30c-129">Property</span></span>|<span data-ttu-id="4a30c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4a30c-130">Type</span></span>|<span data-ttu-id="4a30c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a30c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a30c-132">label</span><span class="sxs-lookup"><span data-stu-id="4a30c-132">label</span></span>|<span data-ttu-id="4a30c-133">String</span><span class="sxs-lookup"><span data-stu-id="4a30c-133">String</span></span>|<span data-ttu-id="4a30c-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="4a30c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="4a30c-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="4a30c-135">The default value is empty.</span></span> <span data-ttu-id="4a30c-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4a30c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4a30c-137">id</span><span class="sxs-lookup"><span data-stu-id="4a30c-137">id</span></span>|<span data-ttu-id="4a30c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a30c-138">String</span></span>|<span data-ttu-id="4a30c-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4a30c-139">Key of the entity.</span></span> <span data-ttu-id="4a30c-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4a30c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4a30c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a30c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4a30c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a30c-142">DateTimeOffset</span></span>|<span data-ttu-id="4a30c-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="4a30c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="4a30c-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="4a30c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="4a30c-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="4a30c-145">defaultValue</span></span>|<span data-ttu-id="4a30c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a30c-146">String</span></span>|<span data-ttu-id="4a30c-147">Im Kombinationsfeld angezeigte lokalisierte Standardzeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="4a30c-147">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="4a30c-148">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="4a30c-148">The default value is empty.</span></span>|
|<span data-ttu-id="4a30c-149">Vorschläge</span><span class="sxs-lookup"><span data-stu-id="4a30c-149">suggestions</span></span>|<span data-ttu-id="4a30c-150">String collection</span><span class="sxs-lookup"><span data-stu-id="4a30c-150">String collection</span></span>|<span data-ttu-id="4a30c-151">Lokalisierte Zeichenfolgen, die in der Dropdownliste des Kombinationsfelds aufgeführt sind.</span><span class="sxs-lookup"><span data-stu-id="4a30c-151">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="4a30c-152">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="4a30c-152">The default value is empty.</span></span>|
|<span data-ttu-id="4a30c-153">erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a30c-153">required</span></span>|<span data-ttu-id="4a30c-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a30c-154">Boolean</span></span>|<span data-ttu-id="4a30c-155">Gibt an, ob ein Wert für den Parameter angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="4a30c-155">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="4a30c-156">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="4a30c-156">The default value is false.</span></span>|
|<span data-ttu-id="4a30c-157">maxLength</span><span class="sxs-lookup"><span data-stu-id="4a30c-157">maxLength</span></span>|<span data-ttu-id="4a30c-158">Int64</span><span class="sxs-lookup"><span data-stu-id="4a30c-158">Int64</span></span>|<span data-ttu-id="4a30c-159">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen für den Parameter angibt.</span><span class="sxs-lookup"><span data-stu-id="4a30c-159">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="4a30c-160">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="4a30c-160">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="4a30c-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a30c-161">Response</span></span>
<span data-ttu-id="4a30c-162">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4a30c-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a30c-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a30c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a30c-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a30c-164">Request</span></span>
<span data-ttu-id="4a30c-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a30c-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="4a30c-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a30c-166">Response</span></span>
<span data-ttu-id="4a30c-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a30c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





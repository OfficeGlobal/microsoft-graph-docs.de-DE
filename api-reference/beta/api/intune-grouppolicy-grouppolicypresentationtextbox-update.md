---
title: GroupPolicyPresentationTextBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f9cc29531d8318be47e1738fdc6d51dca8f044b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152136"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="04b56-103">GroupPolicyPresentationTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="04b56-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="04b56-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04b56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04b56-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="04b56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b56-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="04b56-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b56-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04b56-107">Prerequisites</span></span>
<span data-ttu-id="04b56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04b56-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04b56-110">Permission type</span></span>|<span data-ttu-id="04b56-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04b56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b56-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04b56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04b56-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b56-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04b56-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04b56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b56-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04b56-115">Not supported.</span></span>|
|<span data-ttu-id="04b56-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04b56-116">Application</span></span>|<span data-ttu-id="04b56-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04b56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b56-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="04b56-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04b56-119">Request headers</span></span>
|<span data-ttu-id="04b56-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04b56-120">Header</span></span>|<span data-ttu-id="04b56-121">Wert</span><span class="sxs-lookup"><span data-stu-id="04b56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b56-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04b56-122">Authorization</span></span>|<span data-ttu-id="04b56-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04b56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b56-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04b56-124">Accept</span></span>|<span data-ttu-id="04b56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04b56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b56-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04b56-126">Request body</span></span>
<span data-ttu-id="04b56-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="04b56-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="04b56-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="04b56-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="04b56-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04b56-129">Property</span></span>|<span data-ttu-id="04b56-130">Typ</span><span class="sxs-lookup"><span data-stu-id="04b56-130">Type</span></span>|<span data-ttu-id="04b56-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04b56-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b56-132">label</span><span class="sxs-lookup"><span data-stu-id="04b56-132">label</span></span>|<span data-ttu-id="04b56-133">String</span><span class="sxs-lookup"><span data-stu-id="04b56-133">String</span></span>|<span data-ttu-id="04b56-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="04b56-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="04b56-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="04b56-135">The default value is empty.</span></span> <span data-ttu-id="04b56-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="04b56-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="04b56-137">id</span><span class="sxs-lookup"><span data-stu-id="04b56-137">id</span></span>|<span data-ttu-id="04b56-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04b56-138">String</span></span>|<span data-ttu-id="04b56-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="04b56-139">Key of the entity.</span></span> <span data-ttu-id="04b56-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="04b56-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="04b56-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04b56-141">lastModifiedDateTime</span></span>|<span data-ttu-id="04b56-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04b56-142">DateTimeOffset</span></span>|<span data-ttu-id="04b56-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="04b56-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="04b56-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="04b56-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="04b56-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="04b56-145">defaultValue</span></span>|<span data-ttu-id="04b56-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04b56-146">String</span></span>|<span data-ttu-id="04b56-147">Lokalisierte Standardzeichenfolge, die im Textfeld angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="04b56-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="04b56-148">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="04b56-148">The default value is empty.</span></span>|
|<span data-ttu-id="04b56-149">erforderlich</span><span class="sxs-lookup"><span data-stu-id="04b56-149">required</span></span>|<span data-ttu-id="04b56-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b56-150">Boolean</span></span>|<span data-ttu-id="04b56-151">Anforderung zur Eingabe eines Werts in das Textfeld.</span><span class="sxs-lookup"><span data-stu-id="04b56-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="04b56-152">Der Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="04b56-152">Default value is false.</span></span>|
|<span data-ttu-id="04b56-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="04b56-153">maxLength</span></span>|<span data-ttu-id="04b56-154">Int64</span><span class="sxs-lookup"><span data-stu-id="04b56-154">Int64</span></span>|<span data-ttu-id="04b56-155">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="04b56-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="04b56-156">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="04b56-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="04b56-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b56-157">Response</span></span>
<span data-ttu-id="04b56-158">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04b56-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b56-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04b56-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b56-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04b56-160">Request</span></span>
<span data-ttu-id="04b56-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04b56-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="04b56-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="04b56-162">Response</span></span>
<span data-ttu-id="04b56-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04b56-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```





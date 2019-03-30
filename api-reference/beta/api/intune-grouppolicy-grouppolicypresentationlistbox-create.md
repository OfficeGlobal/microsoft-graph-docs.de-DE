---
title: GroupPolicyPresentationListBox erstellen
description: Erstellen eines neuen groupPolicyPresentationListBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e57fa0a5ce0f4bbaa3bd9a50383a6c7505083cf4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979417"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="67ef4-103">GroupPolicyPresentationListBox erstellen</span><span class="sxs-lookup"><span data-stu-id="67ef4-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="67ef4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67ef4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67ef4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="67ef4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67ef4-106">Erstellen eines neuen [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="67ef4-106">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67ef4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="67ef4-107">Prerequisites</span></span>
<span data-ttu-id="67ef4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ef4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="67ef4-110">Permission type</span></span>|<span data-ttu-id="67ef4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="67ef4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67ef4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="67ef4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67ef4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ef4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67ef4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="67ef4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67ef4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67ef4-115">Not supported.</span></span>|
|<span data-ttu-id="67ef4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="67ef4-116">Application</span></span>|<span data-ttu-id="67ef4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="67ef4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67ef4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67ef4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="67ef4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67ef4-119">Request headers</span></span>
|<span data-ttu-id="67ef4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="67ef4-120">Header</span></span>|<span data-ttu-id="67ef4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="67ef4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67ef4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67ef4-122">Authorization</span></span>|<span data-ttu-id="67ef4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="67ef4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67ef4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="67ef4-124">Accept</span></span>|<span data-ttu-id="67ef4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67ef4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67ef4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="67ef4-126">Request body</span></span>
<span data-ttu-id="67ef4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationListBox-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="67ef4-127">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="67ef4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationListBox erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="67ef4-128">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="67ef4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67ef4-129">Property</span></span>|<span data-ttu-id="67ef4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="67ef4-130">Type</span></span>|<span data-ttu-id="67ef4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67ef4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67ef4-132">label</span><span class="sxs-lookup"><span data-stu-id="67ef4-132">label</span></span>|<span data-ttu-id="67ef4-133">String</span><span class="sxs-lookup"><span data-stu-id="67ef4-133">String</span></span>|<span data-ttu-id="67ef4-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="67ef4-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="67ef4-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="67ef4-135">The default value is empty.</span></span> <span data-ttu-id="67ef4-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67ef4-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67ef4-137">id</span><span class="sxs-lookup"><span data-stu-id="67ef4-137">id</span></span>|<span data-ttu-id="67ef4-138">String</span><span class="sxs-lookup"><span data-stu-id="67ef4-138">String</span></span>|<span data-ttu-id="67ef4-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="67ef4-139">Key of the entity.</span></span> <span data-ttu-id="67ef4-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67ef4-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67ef4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67ef4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="67ef4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67ef4-142">DateTimeOffset</span></span>|<span data-ttu-id="67ef4-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="67ef4-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="67ef4-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="67ef4-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="67ef4-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="67ef4-145">explicitValue</span></span>|<span data-ttu-id="67ef4-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67ef4-146">Boolean</span></span>|<span data-ttu-id="67ef4-147">Wenn diese Option auf true festgelegt ist, muss der Benutzer den Registrierungsunterschlüssel-Wert und den Registrierungsunterschlüssel Namen angeben.</span><span class="sxs-lookup"><span data-stu-id="67ef4-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="67ef4-148">Das Listenfeld enthält zwei Spalten, eine für den Namen und einen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="67ef4-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="67ef4-149">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="67ef4-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="67ef4-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="67ef4-150">Response</span></span>
<span data-ttu-id="67ef4-151">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="67ef4-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67ef4-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67ef4-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="67ef4-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67ef4-153">Request</span></span>
<span data-ttu-id="67ef4-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="67ef4-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="67ef4-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="67ef4-155">Response</span></span>
<span data-ttu-id="67ef4-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67ef4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```





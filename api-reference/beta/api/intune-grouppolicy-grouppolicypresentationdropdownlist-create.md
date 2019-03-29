---
title: GroupPolicyPresentationDropdownList erstellen
description: Erstellen eines neuen groupPolicyPresentationDropdownList-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91865f26463dc1e690a1b5191ae47fbcf887a897
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979627"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="9e826-103">GroupPolicyPresentationDropdownList erstellen</span><span class="sxs-lookup"><span data-stu-id="9e826-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="9e826-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e826-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e826-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e826-106">Erstellen eines neuen [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e826-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e826-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e826-107">Prerequisites</span></span>
<span data-ttu-id="9e826-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e826-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e826-110">Permission type</span></span>|<span data-ttu-id="9e826-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e826-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e826-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e826-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e826-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e826-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9e826-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e826-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e826-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e826-115">Not supported.</span></span>|
|<span data-ttu-id="9e826-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e826-116">Application</span></span>|<span data-ttu-id="9e826-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e826-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e826-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e826-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="9e826-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e826-119">Request headers</span></span>
|<span data-ttu-id="9e826-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e826-120">Header</span></span>|<span data-ttu-id="9e826-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9e826-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e826-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e826-122">Authorization</span></span>|<span data-ttu-id="9e826-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e826-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e826-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e826-124">Accept</span></span>|<span data-ttu-id="9e826-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e826-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e826-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e826-126">Request body</span></span>
<span data-ttu-id="9e826-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationDropdownList-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9e826-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="9e826-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationDropdownList erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9e826-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="9e826-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e826-129">Property</span></span>|<span data-ttu-id="9e826-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9e826-130">Type</span></span>|<span data-ttu-id="9e826-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e826-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e826-132">label</span><span class="sxs-lookup"><span data-stu-id="9e826-132">label</span></span>|<span data-ttu-id="9e826-133">String</span><span class="sxs-lookup"><span data-stu-id="9e826-133">String</span></span>|<span data-ttu-id="9e826-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="9e826-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9e826-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="9e826-135">The default value is empty.</span></span> <span data-ttu-id="9e826-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e826-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e826-137">id</span><span class="sxs-lookup"><span data-stu-id="9e826-137">id</span></span>|<span data-ttu-id="9e826-138">String</span><span class="sxs-lookup"><span data-stu-id="9e826-138">String</span></span>|<span data-ttu-id="9e826-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9e826-139">Key of the entity.</span></span> <span data-ttu-id="9e826-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e826-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e826-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e826-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9e826-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e826-142">DateTimeOffset</span></span>|<span data-ttu-id="9e826-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="9e826-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="9e826-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9e826-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9e826-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="9e826-145">defaultItem</span></span>|[<span data-ttu-id="9e826-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="9e826-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="9e826-147">Lokalisierter Zeichenfolgenwert, der die Standardauswahl der Liste von Elementen identifiziert.</span><span class="sxs-lookup"><span data-stu-id="9e826-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="9e826-148">items</span><span class="sxs-lookup"><span data-stu-id="9e826-148">items</span></span>|<span data-ttu-id="9e826-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e826-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="9e826-150">Stellt eine Gruppe von lokalisierten Anzeigenamen und deren zugeordneten Werten dar.</span><span class="sxs-lookup"><span data-stu-id="9e826-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="9e826-151">erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e826-151">required</span></span>|<span data-ttu-id="9e826-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9e826-152">Boolean</span></span>|<span data-ttu-id="9e826-153">Anforderung zur Eingabe eines Werts im Parameterfeld.</span><span class="sxs-lookup"><span data-stu-id="9e826-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="9e826-154">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="9e826-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="9e826-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e826-155">Response</span></span>
<span data-ttu-id="9e826-156">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e826-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e826-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e826-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e826-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e826-158">Request</span></span>
<span data-ttu-id="9e826-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e826-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="9e826-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e826-160">Response</span></span>
<span data-ttu-id="9e826-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e826-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```





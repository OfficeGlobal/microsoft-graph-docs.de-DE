---
title: GroupPolicyPresentationDropdownList aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationDropdownList-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 170034d102f0d03bad1ca35e36f1d8219ab249ba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989058"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="7e678-103">GroupPolicyPresentationDropdownList aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7e678-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="7e678-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e678-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e678-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7e678-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e678-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7e678-106">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e678-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e678-107">Prerequisites</span></span>
<span data-ttu-id="7e678-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e678-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e678-110">Permission type</span></span>|<span data-ttu-id="7e678-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e678-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e678-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e678-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e678-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e678-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7e678-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e678-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e678-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e678-115">Not supported.</span></span>|
|<span data-ttu-id="7e678-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e678-116">Application</span></span>|<span data-ttu-id="7e678-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e678-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e678-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e678-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="7e678-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e678-119">Request headers</span></span>
|<span data-ttu-id="7e678-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7e678-120">Header</span></span>|<span data-ttu-id="7e678-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7e678-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e678-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e678-122">Authorization</span></span>|<span data-ttu-id="7e678-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e678-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e678-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7e678-124">Accept</span></span>|<span data-ttu-id="7e678-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e678-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e678-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e678-126">Request body</span></span>
<span data-ttu-id="7e678-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="7e678-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="7e678-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7e678-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="7e678-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e678-129">Property</span></span>|<span data-ttu-id="7e678-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7e678-130">Type</span></span>|<span data-ttu-id="7e678-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e678-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e678-132">label</span><span class="sxs-lookup"><span data-stu-id="7e678-132">label</span></span>|<span data-ttu-id="7e678-133">String</span><span class="sxs-lookup"><span data-stu-id="7e678-133">String</span></span>|<span data-ttu-id="7e678-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="7e678-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7e678-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="7e678-135">The default value is empty.</span></span> <span data-ttu-id="7e678-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e678-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e678-137">id</span><span class="sxs-lookup"><span data-stu-id="7e678-137">id</span></span>|<span data-ttu-id="7e678-138">String</span><span class="sxs-lookup"><span data-stu-id="7e678-138">String</span></span>|<span data-ttu-id="7e678-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7e678-139">Key of the entity.</span></span> <span data-ttu-id="7e678-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e678-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e678-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e678-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7e678-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e678-142">DateTimeOffset</span></span>|<span data-ttu-id="7e678-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="7e678-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="7e678-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7e678-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e678-145">defaultItem</span><span class="sxs-lookup"><span data-stu-id="7e678-145">defaultItem</span></span>|[<span data-ttu-id="7e678-146">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="7e678-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="7e678-147">Lokalisierter Zeichenfolgenwert, der die Standardauswahl der Liste von Elementen identifiziert.</span><span class="sxs-lookup"><span data-stu-id="7e678-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="7e678-148">items</span><span class="sxs-lookup"><span data-stu-id="7e678-148">items</span></span>|<span data-ttu-id="7e678-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="7e678-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="7e678-150">Stellt eine Gruppe von lokalisierten Anzeigenamen und deren zugeordneten Werten dar.</span><span class="sxs-lookup"><span data-stu-id="7e678-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="7e678-151">erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e678-151">required</span></span>|<span data-ttu-id="7e678-152">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7e678-152">Boolean</span></span>|<span data-ttu-id="7e678-153">Anforderung zur Eingabe eines Werts im Parameterfeld.</span><span class="sxs-lookup"><span data-stu-id="7e678-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="7e678-154">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="7e678-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="7e678-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e678-155">Response</span></span>
<span data-ttu-id="7e678-156">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7e678-156">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e678-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e678-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e678-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e678-158">Request</span></span>
<span data-ttu-id="7e678-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e678-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="7e678-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e678-160">Response</span></span>
<span data-ttu-id="7e678-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e678-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





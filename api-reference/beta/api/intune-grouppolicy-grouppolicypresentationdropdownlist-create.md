---
title: Erstellen von groupPolicyPresentationDropdownList
description: Erstellen eines neuen GroupPolicyPresentationDropdownList-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 415ccd634e4206b2849fc5feecc4131d2f417d16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431561"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="3ab36-103">Erstellen von groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="3ab36-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="3ab36-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3ab36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ab36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ab36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ab36-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ab36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab36-107">Erstellen eines neuen [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3ab36-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ab36-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3ab36-108">Prerequisites</span></span>
<span data-ttu-id="3ab36-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ab36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3ab36-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ab36-111">Permission type</span></span>|<span data-ttu-id="3ab36-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ab36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ab36-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ab36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ab36-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab36-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3ab36-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ab36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ab36-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ab36-116">Not supported.</span></span>|
|<span data-ttu-id="3ab36-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ab36-117">Application</span></span>|<span data-ttu-id="3ab36-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ab36-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ab36-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ab36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="3ab36-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ab36-120">Request headers</span></span>
|<span data-ttu-id="3ab36-121">Header</span><span class="sxs-lookup"><span data-stu-id="3ab36-121">Header</span></span>|<span data-ttu-id="3ab36-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3ab36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ab36-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3ab36-123">Authorization</span></span>|<span data-ttu-id="3ab36-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ab36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ab36-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3ab36-125">Accept</span></span>|<span data-ttu-id="3ab36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ab36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ab36-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ab36-127">Request body</span></span>
<span data-ttu-id="3ab36-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationDropdownList eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3ab36-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="3ab36-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationDropdownList erstellen.</span><span class="sxs-lookup"><span data-stu-id="3ab36-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="3ab36-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ab36-130">Property</span></span>|<span data-ttu-id="3ab36-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3ab36-131">Type</span></span>|<span data-ttu-id="3ab36-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ab36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ab36-133">label</span><span class="sxs-lookup"><span data-stu-id="3ab36-133">label</span></span>|<span data-ttu-id="3ab36-134">String</span><span class="sxs-lookup"><span data-stu-id="3ab36-134">String</span></span>|<span data-ttu-id="3ab36-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="3ab36-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3ab36-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="3ab36-136">The default value is empty.</span></span> <span data-ttu-id="3ab36-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3ab36-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3ab36-138">id</span><span class="sxs-lookup"><span data-stu-id="3ab36-138">id</span></span>|<span data-ttu-id="3ab36-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3ab36-139">String</span></span>|<span data-ttu-id="3ab36-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3ab36-140">Key of the entity.</span></span> <span data-ttu-id="3ab36-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3ab36-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3ab36-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ab36-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3ab36-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ab36-143">DateTimeOffset</span></span>|<span data-ttu-id="3ab36-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="3ab36-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="3ab36-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3ab36-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3ab36-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="3ab36-146">defaultItem</span></span>|[<span data-ttu-id="3ab36-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="3ab36-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="3ab36-148">Lokalisierter Zeichenfolgenwert, der die Standardauswahl der Liste der Elemente angibt.</span><span class="sxs-lookup"><span data-stu-id="3ab36-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="3ab36-149">Elemente</span><span class="sxs-lookup"><span data-stu-id="3ab36-149">items</span></span>|<span data-ttu-id="3ab36-150">[GroupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3ab36-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="3ab36-151">Stellt eine Reihe von lokalisierten Anzeigenamen und die zugeordneten Werte.</span><span class="sxs-lookup"><span data-stu-id="3ab36-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="3ab36-152">erforderlich</span><span class="sxs-lookup"><span data-stu-id="3ab36-152">required</span></span>|<span data-ttu-id="3ab36-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ab36-153">Boolean</span></span>|<span data-ttu-id="3ab36-154">Anforderung im Parameter einen Wert eingeben.</span><span class="sxs-lookup"><span data-stu-id="3ab36-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="3ab36-155">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="3ab36-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="3ab36-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ab36-156">Response</span></span>
<span data-ttu-id="3ab36-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3ab36-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ab36-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ab36-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ab36-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ab36-159">Request</span></span>
<span data-ttu-id="3ab36-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ab36-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ab36-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ab36-161">Response</span></span>
<span data-ttu-id="3ab36-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ab36-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




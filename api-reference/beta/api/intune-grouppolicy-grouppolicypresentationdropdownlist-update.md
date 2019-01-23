---
title: GroupPolicyPresentationDropdownList aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationDropdownList-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cb39764767eba6bda56c4763660f7981f0e71db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430177"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="9ac91-103">GroupPolicyPresentationDropdownList aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9ac91-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="9ac91-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9ac91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ac91-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ac91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ac91-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ac91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac91-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ac91-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac91-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ac91-108">Prerequisites</span></span>
<span data-ttu-id="9ac91-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ac91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ac91-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ac91-111">Permission type</span></span>|<span data-ttu-id="9ac91-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ac91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac91-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ac91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac91-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac91-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac91-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ac91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac91-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac91-116">Not supported.</span></span>|
|<span data-ttu-id="9ac91-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ac91-117">Application</span></span>|<span data-ttu-id="9ac91-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac91-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ac91-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ac91-120">Request headers</span></span>
|<span data-ttu-id="9ac91-121">Header</span><span class="sxs-lookup"><span data-stu-id="9ac91-121">Header</span></span>|<span data-ttu-id="9ac91-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9ac91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac91-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9ac91-123">Authorization</span></span>|<span data-ttu-id="9ac91-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ac91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac91-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ac91-125">Accept</span></span>|<span data-ttu-id="9ac91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac91-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ac91-127">Request body</span></span>
<span data-ttu-id="9ac91-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9ac91-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="9ac91-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="9ac91-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="9ac91-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ac91-130">Property</span></span>|<span data-ttu-id="9ac91-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9ac91-131">Type</span></span>|<span data-ttu-id="9ac91-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ac91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac91-133">label</span><span class="sxs-lookup"><span data-stu-id="9ac91-133">label</span></span>|<span data-ttu-id="9ac91-134">String</span><span class="sxs-lookup"><span data-stu-id="9ac91-134">String</span></span>|<span data-ttu-id="9ac91-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="9ac91-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9ac91-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="9ac91-136">The default value is empty.</span></span> <span data-ttu-id="9ac91-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9ac91-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9ac91-138">id</span><span class="sxs-lookup"><span data-stu-id="9ac91-138">id</span></span>|<span data-ttu-id="9ac91-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ac91-139">String</span></span>|<span data-ttu-id="9ac91-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ac91-140">Key of the entity.</span></span> <span data-ttu-id="9ac91-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9ac91-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9ac91-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac91-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9ac91-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac91-143">DateTimeOffset</span></span>|<span data-ttu-id="9ac91-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="9ac91-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="9ac91-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9ac91-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9ac91-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="9ac91-146">defaultItem</span></span>|[<span data-ttu-id="9ac91-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="9ac91-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="9ac91-148">Lokalisierter Zeichenfolgenwert, der die Standardauswahl der Liste der Elemente angibt.</span><span class="sxs-lookup"><span data-stu-id="9ac91-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="9ac91-149">Elemente</span><span class="sxs-lookup"><span data-stu-id="9ac91-149">items</span></span>|<span data-ttu-id="9ac91-150">[GroupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9ac91-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="9ac91-151">Stellt eine Reihe von lokalisierten Anzeigenamen und die zugeordneten Werte.</span><span class="sxs-lookup"><span data-stu-id="9ac91-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="9ac91-152">erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ac91-152">required</span></span>|<span data-ttu-id="9ac91-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac91-153">Boolean</span></span>|<span data-ttu-id="9ac91-154">Anforderung im Parameter einen Wert eingeben.</span><span class="sxs-lookup"><span data-stu-id="9ac91-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="9ac91-155">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="9ac91-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="9ac91-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac91-156">Response</span></span>
<span data-ttu-id="9ac91-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9ac91-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac91-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ac91-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac91-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac91-159">Request</span></span>
<span data-ttu-id="9ac91-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ac91-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ac91-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac91-161">Response</span></span>
<span data-ttu-id="9ac91-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ac91-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





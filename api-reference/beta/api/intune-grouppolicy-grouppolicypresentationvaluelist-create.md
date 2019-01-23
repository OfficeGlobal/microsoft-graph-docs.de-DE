---
title: Erstellen von groupPolicyPresentationValueList
description: Erstellen eines neuen GroupPolicyPresentationValueList-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a27fd61c30e56942965cf8df426e65064f82527
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429974"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="fa797-103">Erstellen von groupPolicyPresentationValueList</span><span class="sxs-lookup"><span data-stu-id="fa797-103">Create groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="fa797-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fa797-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa797-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa797-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa797-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa797-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa797-107">Erstellen eines neuen [GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa797-107">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa797-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa797-108">Prerequisites</span></span>
<span data-ttu-id="fa797-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa797-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa797-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa797-111">Permission type</span></span>|<span data-ttu-id="fa797-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa797-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa797-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa797-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa797-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa797-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa797-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa797-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa797-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa797-116">Not supported.</span></span>|
|<span data-ttu-id="fa797-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa797-117">Application</span></span>|<span data-ttu-id="fa797-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa797-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa797-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa797-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="fa797-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa797-120">Request headers</span></span>
|<span data-ttu-id="fa797-121">Header</span><span class="sxs-lookup"><span data-stu-id="fa797-121">Header</span></span>|<span data-ttu-id="fa797-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fa797-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa797-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fa797-123">Authorization</span></span>|<span data-ttu-id="fa797-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa797-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa797-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa797-125">Accept</span></span>|<span data-ttu-id="fa797-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa797-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa797-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa797-127">Request body</span></span>
<span data-ttu-id="fa797-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValueList eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fa797-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="fa797-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValueList erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa797-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="fa797-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa797-130">Property</span></span>|<span data-ttu-id="fa797-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fa797-131">Type</span></span>|<span data-ttu-id="fa797-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa797-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa797-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa797-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fa797-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa797-134">DateTimeOffset</span></span>|<span data-ttu-id="fa797-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="fa797-135">The date and time the object was last modified.</span></span> <span data-ttu-id="fa797-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fa797-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fa797-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa797-137">createdDateTime</span></span>|<span data-ttu-id="fa797-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa797-138">DateTimeOffset</span></span>|<span data-ttu-id="fa797-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="fa797-139">The date and time the object was created.</span></span> <span data-ttu-id="fa797-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fa797-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fa797-141">id</span><span class="sxs-lookup"><span data-stu-id="fa797-141">id</span></span>|<span data-ttu-id="fa797-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa797-142">String</span></span>|<span data-ttu-id="fa797-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa797-143">Key of the entity.</span></span> <span data-ttu-id="fa797-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fa797-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fa797-145">values</span><span class="sxs-lookup"><span data-stu-id="fa797-145">values</span></span>|<span data-ttu-id="fa797-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fa797-146">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fa797-147">Eine Liste der Paare für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="fa797-147">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="fa797-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa797-148">Response</span></span>
<span data-ttu-id="fa797-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fa797-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa797-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa797-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa797-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa797-151">Request</span></span>
<span data-ttu-id="fa797-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa797-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="fa797-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa797-153">Response</span></span>
<span data-ttu-id="fa797-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa797-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```





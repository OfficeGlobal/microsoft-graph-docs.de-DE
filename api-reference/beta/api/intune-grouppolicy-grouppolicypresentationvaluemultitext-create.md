---
title: Erstellen von groupPolicyPresentationValueMultiText
description: Erstellen eines neuen GroupPolicyPresentationValueMultiText-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 53f31f53808515fadf7130f8037b0d2a50be3dd1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430184"
---
# <a name="create-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="09795-103">Erstellen von groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="09795-103">Create groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="09795-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="09795-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09795-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09795-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09795-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="09795-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09795-107">Erstellen eines neuen [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="09795-107">Create a new [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09795-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09795-108">Prerequisites</span></span>
<span data-ttu-id="09795-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="09795-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="09795-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09795-111">Permission type</span></span>|<span data-ttu-id="09795-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09795-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09795-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09795-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09795-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09795-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09795-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09795-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09795-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09795-116">Not supported.</span></span>|
|<span data-ttu-id="09795-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09795-117">Application</span></span>|<span data-ttu-id="09795-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09795-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09795-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09795-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="09795-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09795-120">Request headers</span></span>
|<span data-ttu-id="09795-121">Header</span><span class="sxs-lookup"><span data-stu-id="09795-121">Header</span></span>|<span data-ttu-id="09795-122">Wert</span><span class="sxs-lookup"><span data-stu-id="09795-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09795-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="09795-123">Authorization</span></span>|<span data-ttu-id="09795-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09795-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09795-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09795-125">Accept</span></span>|<span data-ttu-id="09795-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09795-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09795-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09795-127">Request body</span></span>
<span data-ttu-id="09795-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValueMultiText eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="09795-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueMultiText object.</span></span>

<span data-ttu-id="09795-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValueMultiText erstellen.</span><span class="sxs-lookup"><span data-stu-id="09795-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueMultiText.</span></span>

|<span data-ttu-id="09795-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09795-130">Property</span></span>|<span data-ttu-id="09795-131">Typ</span><span class="sxs-lookup"><span data-stu-id="09795-131">Type</span></span>|<span data-ttu-id="09795-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09795-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09795-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09795-133">lastModifiedDateTime</span></span>|<span data-ttu-id="09795-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09795-134">DateTimeOffset</span></span>|<span data-ttu-id="09795-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="09795-135">The date and time the object was last modified.</span></span> <span data-ttu-id="09795-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="09795-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="09795-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09795-137">createdDateTime</span></span>|<span data-ttu-id="09795-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09795-138">DateTimeOffset</span></span>|<span data-ttu-id="09795-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="09795-139">The date and time the object was created.</span></span> <span data-ttu-id="09795-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="09795-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="09795-141">id</span><span class="sxs-lookup"><span data-stu-id="09795-141">id</span></span>|<span data-ttu-id="09795-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="09795-142">String</span></span>|<span data-ttu-id="09795-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="09795-143">Key of the entity.</span></span> <span data-ttu-id="09795-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="09795-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="09795-145">values</span><span class="sxs-lookup"><span data-stu-id="09795-145">values</span></span>|<span data-ttu-id="09795-146">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="09795-146">String collection</span></span>|<span data-ttu-id="09795-147">Eine Auflistung von nicht leeren Zeichenfolgen für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="09795-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="09795-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="09795-148">Response</span></span>
<span data-ttu-id="09795-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="09795-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09795-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09795-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="09795-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09795-151">Request</span></span>
<span data-ttu-id="09795-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09795-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="09795-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="09795-153">Response</span></span>
<span data-ttu-id="09795-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09795-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```





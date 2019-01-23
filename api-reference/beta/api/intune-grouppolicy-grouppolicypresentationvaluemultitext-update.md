---
title: GroupPolicyPresentationValueMultiText aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationValueMultiText-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 030f1a422106eeda59e77f06ce37d60688744b53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430205"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="7355d-103">GroupPolicyPresentationValueMultiText aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7355d-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="7355d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7355d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7355d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7355d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7355d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7355d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7355d-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7355d-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7355d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7355d-108">Prerequisites</span></span>
<span data-ttu-id="7355d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7355d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7355d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7355d-111">Permission type</span></span>|<span data-ttu-id="7355d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7355d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7355d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7355d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7355d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7355d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7355d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7355d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7355d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7355d-116">Not supported.</span></span>|
|<span data-ttu-id="7355d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7355d-117">Application</span></span>|<span data-ttu-id="7355d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7355d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7355d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7355d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="7355d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7355d-120">Request headers</span></span>
|<span data-ttu-id="7355d-121">Header</span><span class="sxs-lookup"><span data-stu-id="7355d-121">Header</span></span>|<span data-ttu-id="7355d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7355d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7355d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7355d-123">Authorization</span></span>|<span data-ttu-id="7355d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7355d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7355d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7355d-125">Accept</span></span>|<span data-ttu-id="7355d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7355d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7355d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7355d-127">Request body</span></span>
<span data-ttu-id="7355d-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7355d-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="7355d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="7355d-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="7355d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7355d-130">Property</span></span>|<span data-ttu-id="7355d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7355d-131">Type</span></span>|<span data-ttu-id="7355d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7355d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7355d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7355d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7355d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7355d-134">DateTimeOffset</span></span>|<span data-ttu-id="7355d-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="7355d-135">The date and time the object was last modified.</span></span> <span data-ttu-id="7355d-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7355d-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7355d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7355d-137">createdDateTime</span></span>|<span data-ttu-id="7355d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7355d-138">DateTimeOffset</span></span>|<span data-ttu-id="7355d-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7355d-139">The date and time the object was created.</span></span> <span data-ttu-id="7355d-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7355d-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7355d-141">id</span><span class="sxs-lookup"><span data-stu-id="7355d-141">id</span></span>|<span data-ttu-id="7355d-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7355d-142">String</span></span>|<span data-ttu-id="7355d-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7355d-143">Key of the entity.</span></span> <span data-ttu-id="7355d-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="7355d-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="7355d-145">values</span><span class="sxs-lookup"><span data-stu-id="7355d-145">values</span></span>|<span data-ttu-id="7355d-146">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7355d-146">String collection</span></span>|<span data-ttu-id="7355d-147">Eine Auflistung von nicht leeren Zeichenfolgen für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="7355d-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="7355d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="7355d-148">Response</span></span>
<span data-ttu-id="7355d-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7355d-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7355d-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7355d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="7355d-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7355d-151">Request</span></span>
<span data-ttu-id="7355d-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7355d-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="7355d-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="7355d-153">Response</span></span>
<span data-ttu-id="7355d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7355d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





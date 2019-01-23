---
title: Erstellen von groupPolicyPresentationValueDecimal
description: Erstellen eines neuen GroupPolicyPresentationValueDecimal-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32e1947ccbda3b7c7e153daf6058dfc558460a02
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431553"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="60971-103">Erstellen von groupPolicyPresentationValueDecimal</span><span class="sxs-lookup"><span data-stu-id="60971-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="60971-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="60971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60971-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60971-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60971-107">Erstellen eines neuen [GroupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="60971-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60971-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="60971-108">Prerequisites</span></span>
<span data-ttu-id="60971-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="60971-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60971-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60971-111">Permission type</span></span>|<span data-ttu-id="60971-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60971-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60971-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60971-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="60971-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60971-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60971-116">Not supported.</span></span>|
|<span data-ttu-id="60971-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60971-117">Application</span></span>|<span data-ttu-id="60971-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60971-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60971-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60971-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="60971-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60971-120">Request headers</span></span>
|<span data-ttu-id="60971-121">Header</span><span class="sxs-lookup"><span data-stu-id="60971-121">Header</span></span>|<span data-ttu-id="60971-122">Wert</span><span class="sxs-lookup"><span data-stu-id="60971-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60971-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="60971-123">Authorization</span></span>|<span data-ttu-id="60971-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="60971-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60971-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="60971-125">Accept</span></span>|<span data-ttu-id="60971-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60971-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60971-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60971-127">Request body</span></span>
<span data-ttu-id="60971-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValueDecimal eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="60971-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="60971-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValueDecimal erstellen.</span><span class="sxs-lookup"><span data-stu-id="60971-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="60971-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60971-130">Property</span></span>|<span data-ttu-id="60971-131">Typ</span><span class="sxs-lookup"><span data-stu-id="60971-131">Type</span></span>|<span data-ttu-id="60971-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60971-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60971-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60971-133">lastModifiedDateTime</span></span>|<span data-ttu-id="60971-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60971-134">DateTimeOffset</span></span>|<span data-ttu-id="60971-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="60971-135">The date and time the object was last modified.</span></span> <span data-ttu-id="60971-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60971-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60971-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60971-137">createdDateTime</span></span>|<span data-ttu-id="60971-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60971-138">DateTimeOffset</span></span>|<span data-ttu-id="60971-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="60971-139">The date and time the object was created.</span></span> <span data-ttu-id="60971-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60971-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60971-141">id</span><span class="sxs-lookup"><span data-stu-id="60971-141">id</span></span>|<span data-ttu-id="60971-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60971-142">String</span></span>|<span data-ttu-id="60971-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="60971-143">Key of the entity.</span></span> <span data-ttu-id="60971-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="60971-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="60971-145">Wert</span><span class="sxs-lookup"><span data-stu-id="60971-145">value</span></span>|<span data-ttu-id="60971-146">Int64</span><span class="sxs-lookup"><span data-stu-id="60971-146">Int64</span></span>|<span data-ttu-id="60971-147">Ein Ganzzahlwert ohne Vorzeichen für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="60971-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="60971-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="60971-148">Response</span></span>
<span data-ttu-id="60971-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="60971-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60971-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60971-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="60971-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60971-151">Request</span></span>
<span data-ttu-id="60971-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60971-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="60971-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="60971-153">Response</span></span>
<span data-ttu-id="60971-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60971-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```





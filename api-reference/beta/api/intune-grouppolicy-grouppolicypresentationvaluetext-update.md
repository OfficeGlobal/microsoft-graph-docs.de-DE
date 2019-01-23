---
title: GroupPolicyPresentationValueText aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationValueText-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f0a1222c9abac4cbc459f25444e3cb37d6576a7e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430142"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="6e020-103">GroupPolicyPresentationValueText aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6e020-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="6e020-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6e020-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6e020-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e020-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e020-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e020-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e020-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6e020-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e020-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6e020-108">Prerequisites</span></span>
<span data-ttu-id="6e020-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e020-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e020-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e020-111">Permission type</span></span>|<span data-ttu-id="6e020-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e020-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e020-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e020-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e020-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e020-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6e020-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e020-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e020-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e020-116">Not supported.</span></span>|
|<span data-ttu-id="6e020-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e020-117">Application</span></span>|<span data-ttu-id="6e020-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e020-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e020-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e020-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="6e020-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e020-120">Request headers</span></span>
|<span data-ttu-id="6e020-121">Header</span><span class="sxs-lookup"><span data-stu-id="6e020-121">Header</span></span>|<span data-ttu-id="6e020-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6e020-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e020-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6e020-123">Authorization</span></span>|<span data-ttu-id="6e020-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6e020-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e020-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6e020-125">Accept</span></span>|<span data-ttu-id="6e020-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e020-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e020-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e020-127">Request body</span></span>
<span data-ttu-id="6e020-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6e020-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="6e020-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6e020-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="6e020-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e020-130">Property</span></span>|<span data-ttu-id="6e020-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6e020-131">Type</span></span>|<span data-ttu-id="6e020-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e020-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e020-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e020-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6e020-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e020-134">DateTimeOffset</span></span>|<span data-ttu-id="6e020-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="6e020-135">The date and time the object was last modified.</span></span> <span data-ttu-id="6e020-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e020-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e020-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e020-137">createdDateTime</span></span>|<span data-ttu-id="6e020-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e020-138">DateTimeOffset</span></span>|<span data-ttu-id="6e020-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="6e020-139">The date and time the object was created.</span></span> <span data-ttu-id="6e020-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e020-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e020-141">id</span><span class="sxs-lookup"><span data-stu-id="6e020-141">id</span></span>|<span data-ttu-id="6e020-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e020-142">String</span></span>|<span data-ttu-id="6e020-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6e020-143">Key of the entity.</span></span> <span data-ttu-id="6e020-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e020-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="6e020-145">Wert</span><span class="sxs-lookup"><span data-stu-id="6e020-145">value</span></span>|<span data-ttu-id="6e020-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e020-146">String</span></span>|<span data-ttu-id="6e020-147">Ein String-Wert für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="6e020-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="6e020-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e020-148">Response</span></span>
<span data-ttu-id="6e020-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6e020-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e020-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e020-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e020-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e020-151">Request</span></span>
<span data-ttu-id="6e020-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e020-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="6e020-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e020-153">Response</span></span>
<span data-ttu-id="6e020-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e020-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```





---
title: GroupPolicyPresentationValue aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValue-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf476988493577d750f3a249bf684d3c5db9a47f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983652"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="3552b-103">GroupPolicyPresentationValue aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3552b-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="3552b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3552b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3552b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3552b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3552b-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3552b-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3552b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3552b-107">Prerequisites</span></span>
<span data-ttu-id="3552b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3552b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3552b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3552b-110">Permission type</span></span>|<span data-ttu-id="3552b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3552b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3552b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3552b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3552b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3552b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3552b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3552b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3552b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3552b-115">Not supported.</span></span>|
|<span data-ttu-id="3552b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3552b-116">Application</span></span>|<span data-ttu-id="3552b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3552b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3552b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3552b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="3552b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3552b-119">Request headers</span></span>
|<span data-ttu-id="3552b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3552b-120">Header</span></span>|<span data-ttu-id="3552b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3552b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3552b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3552b-122">Authorization</span></span>|<span data-ttu-id="3552b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3552b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3552b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3552b-124">Accept</span></span>|<span data-ttu-id="3552b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3552b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3552b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3552b-126">Request body</span></span>
<span data-ttu-id="3552b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="3552b-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="3552b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3552b-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="3552b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3552b-129">Property</span></span>|<span data-ttu-id="3552b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3552b-130">Type</span></span>|<span data-ttu-id="3552b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3552b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3552b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3552b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="3552b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3552b-133">DateTimeOffset</span></span>|<span data-ttu-id="3552b-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3552b-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="3552b-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3552b-135">createdDateTime</span></span>|<span data-ttu-id="3552b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3552b-136">DateTimeOffset</span></span>|<span data-ttu-id="3552b-137">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3552b-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="3552b-138">id</span><span class="sxs-lookup"><span data-stu-id="3552b-138">id</span></span>|<span data-ttu-id="3552b-139">String</span><span class="sxs-lookup"><span data-stu-id="3552b-139">String</span></span>|<span data-ttu-id="3552b-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3552b-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3552b-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3552b-141">Response</span></span>
<span data-ttu-id="3552b-142">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3552b-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3552b-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3552b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3552b-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3552b-144">Request</span></span>
<span data-ttu-id="3552b-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3552b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="3552b-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="3552b-146">Response</span></span>
<span data-ttu-id="3552b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3552b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```





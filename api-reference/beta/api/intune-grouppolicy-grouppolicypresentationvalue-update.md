---
title: GroupPolicyPresentationValue aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationValue-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfec8c5c0a228bf4ba1ed360339d4194cc877faf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430120"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="88c9c-103">GroupPolicyPresentationValue aktualisieren</span><span class="sxs-lookup"><span data-stu-id="88c9c-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="88c9c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="88c9c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88c9c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88c9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88c9c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88c9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c9c-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="88c9c-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88c9c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88c9c-108">Prerequisites</span></span>
<span data-ttu-id="88c9c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="88c9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="88c9c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88c9c-111">Permission type</span></span>|<span data-ttu-id="88c9c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88c9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88c9c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88c9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88c9c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c9c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88c9c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88c9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88c9c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88c9c-116">Not supported.</span></span>|
|<span data-ttu-id="88c9c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88c9c-117">Application</span></span>|<span data-ttu-id="88c9c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88c9c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88c9c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88c9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="88c9c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88c9c-120">Request headers</span></span>
|<span data-ttu-id="88c9c-121">Header</span><span class="sxs-lookup"><span data-stu-id="88c9c-121">Header</span></span>|<span data-ttu-id="88c9c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="88c9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88c9c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="88c9c-123">Authorization</span></span>|<span data-ttu-id="88c9c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88c9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88c9c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="88c9c-125">Accept</span></span>|<span data-ttu-id="88c9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88c9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88c9c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88c9c-127">Request body</span></span>
<span data-ttu-id="88c9c-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="88c9c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="88c9c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="88c9c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="88c9c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88c9c-130">Property</span></span>|<span data-ttu-id="88c9c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="88c9c-131">Type</span></span>|<span data-ttu-id="88c9c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88c9c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c9c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88c9c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="88c9c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c9c-134">DateTimeOffset</span></span>|<span data-ttu-id="88c9c-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="88c9c-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="88c9c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88c9c-136">createdDateTime</span></span>|<span data-ttu-id="88c9c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88c9c-137">DateTimeOffset</span></span>|<span data-ttu-id="88c9c-138">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="88c9c-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="88c9c-139">id</span><span class="sxs-lookup"><span data-stu-id="88c9c-139">id</span></span>|<span data-ttu-id="88c9c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88c9c-140">String</span></span>|<span data-ttu-id="88c9c-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="88c9c-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="88c9c-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="88c9c-142">Response</span></span>
<span data-ttu-id="88c9c-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="88c9c-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88c9c-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88c9c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="88c9c-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88c9c-145">Request</span></span>
<span data-ttu-id="88c9c-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88c9c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="88c9c-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="88c9c-147">Response</span></span>
<span data-ttu-id="88c9c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88c9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





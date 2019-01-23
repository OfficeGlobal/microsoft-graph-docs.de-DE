---
title: GroupPolicyDefinitionValue aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyDefinitionValue-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d346a40e5ee8c2cba6f1510cf52d747e85a0b788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429936"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="c27d1-103">GroupPolicyDefinitionValue aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c27d1-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="c27d1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c27d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c27d1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c27d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c27d1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c27d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c27d1-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c27d1-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c27d1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c27d1-108">Prerequisites</span></span>
<span data-ttu-id="c27d1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c27d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c27d1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c27d1-111">Permission type</span></span>|<span data-ttu-id="c27d1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c27d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c27d1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c27d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c27d1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c27d1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c27d1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c27d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c27d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c27d1-116">Not supported.</span></span>|
|<span data-ttu-id="c27d1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c27d1-117">Application</span></span>|<span data-ttu-id="c27d1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c27d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c27d1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c27d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="c27d1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c27d1-120">Request headers</span></span>
|<span data-ttu-id="c27d1-121">Header</span><span class="sxs-lookup"><span data-stu-id="c27d1-121">Header</span></span>|<span data-ttu-id="c27d1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c27d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c27d1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c27d1-123">Authorization</span></span>|<span data-ttu-id="c27d1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c27d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c27d1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c27d1-125">Accept</span></span>|<span data-ttu-id="c27d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c27d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c27d1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c27d1-127">Request body</span></span>
<span data-ttu-id="c27d1-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c27d1-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="c27d1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c27d1-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="c27d1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c27d1-130">Property</span></span>|<span data-ttu-id="c27d1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c27d1-131">Type</span></span>|<span data-ttu-id="c27d1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c27d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c27d1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c27d1-133">createdDateTime</span></span>|<span data-ttu-id="c27d1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c27d1-134">DateTimeOffset</span></span>|<span data-ttu-id="c27d1-135">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="c27d1-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="c27d1-136">enabled</span><span class="sxs-lookup"><span data-stu-id="c27d1-136">enabled</span></span>|<span data-ttu-id="c27d1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c27d1-137">Boolean</span></span>|<span data-ttu-id="c27d1-138">Aktiviert oder deaktiviert die Richtliniendefinition zugeordneten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c27d1-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="c27d1-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="c27d1-139">configurationType</span></span>|[<span data-ttu-id="c27d1-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="c27d1-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="c27d1-141">Gibt an, wie der Wert konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c27d1-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="c27d1-142">Dies kann als Richtlinie oder als Einstellung sein.</span><span class="sxs-lookup"><span data-stu-id="c27d1-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="c27d1-143">Mögliche Werte sind: `policy` und `preference`.</span><span class="sxs-lookup"><span data-stu-id="c27d1-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="c27d1-144">id</span><span class="sxs-lookup"><span data-stu-id="c27d1-144">id</span></span>|<span data-ttu-id="c27d1-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c27d1-145">String</span></span>|<span data-ttu-id="c27d1-146">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c27d1-146">Key of the entity.</span></span>|
|<span data-ttu-id="c27d1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c27d1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="c27d1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c27d1-148">DateTimeOffset</span></span>|<span data-ttu-id="c27d1-149">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="c27d1-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c27d1-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="c27d1-150">Response</span></span>
<span data-ttu-id="c27d1-151">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c27d1-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c27d1-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c27d1-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c27d1-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c27d1-153">Request</span></span>
<span data-ttu-id="c27d1-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c27d1-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="c27d1-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="c27d1-155">Response</span></span>
<span data-ttu-id="c27d1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c27d1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





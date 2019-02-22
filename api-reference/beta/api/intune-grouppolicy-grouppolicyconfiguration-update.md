---
title: GroupPolicyConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 867d70f3978db683cb154b9e5405df08b315b4b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160032"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="506c5-103">GroupPolicyConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="506c5-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="506c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="506c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="506c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="506c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="506c5-106">Aktualisieren der Eigenschaften eines [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="506c5-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="506c5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="506c5-107">Prerequisites</span></span>
<span data-ttu-id="506c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="506c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="506c5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="506c5-110">Permission type</span></span>|<span data-ttu-id="506c5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="506c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="506c5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="506c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="506c5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506c5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="506c5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="506c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="506c5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="506c5-115">Not supported.</span></span>|
|<span data-ttu-id="506c5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="506c5-116">Application</span></span>|<span data-ttu-id="506c5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="506c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="506c5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="506c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="506c5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="506c5-119">Request headers</span></span>
|<span data-ttu-id="506c5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="506c5-120">Header</span></span>|<span data-ttu-id="506c5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="506c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="506c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="506c5-122">Authorization</span></span>|<span data-ttu-id="506c5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="506c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="506c5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="506c5-124">Accept</span></span>|<span data-ttu-id="506c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="506c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="506c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="506c5-126">Request body</span></span>
<span data-ttu-id="506c5-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="506c5-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="506c5-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="506c5-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="506c5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="506c5-129">Property</span></span>|<span data-ttu-id="506c5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="506c5-130">Type</span></span>|<span data-ttu-id="506c5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="506c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="506c5-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="506c5-132">createdDateTime</span></span>|<span data-ttu-id="506c5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="506c5-133">DateTimeOffset</span></span>|<span data-ttu-id="506c5-134">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="506c5-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="506c5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="506c5-135">displayName</span></span>|<span data-ttu-id="506c5-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="506c5-136">String</span></span>|<span data-ttu-id="506c5-137">Vom Benutzer bereitgestellter Name für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="506c5-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="506c5-138">description</span><span class="sxs-lookup"><span data-stu-id="506c5-138">description</span></span>|<span data-ttu-id="506c5-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="506c5-139">String</span></span>|<span data-ttu-id="506c5-140">Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="506c5-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="506c5-141">id</span><span class="sxs-lookup"><span data-stu-id="506c5-141">id</span></span>|<span data-ttu-id="506c5-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="506c5-142">String</span></span>|<span data-ttu-id="506c5-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="506c5-143">Key of the entity.</span></span>|
|<span data-ttu-id="506c5-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="506c5-144">lastModifiedDateTime</span></span>|<span data-ttu-id="506c5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="506c5-145">DateTimeOffset</span></span>|<span data-ttu-id="506c5-146">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="506c5-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="506c5-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="506c5-147">Response</span></span>
<span data-ttu-id="506c5-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="506c5-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506c5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="506c5-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="506c5-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="506c5-150">Request</span></span>
<span data-ttu-id="506c5-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="506c5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="506c5-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="506c5-152">Response</span></span>
<span data-ttu-id="506c5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="506c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





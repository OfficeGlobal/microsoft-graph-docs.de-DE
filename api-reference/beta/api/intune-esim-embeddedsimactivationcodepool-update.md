---
title: EmbeddedSIMActivationCodePool aktualisieren
description: Aktualisieren der Eigenschaften eines embeddedSIMActivationCodePool-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3d8ee2180f9d687974327bb9d7d018ea8c21dbb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983701"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="d667d-103">EmbeddedSIMActivationCodePool aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d667d-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="d667d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d667d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d667d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d667d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d667d-106">Aktualisieren der Eigenschaften eines [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d667d-106">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d667d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d667d-107">Prerequisites</span></span>
<span data-ttu-id="d667d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d667d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d667d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d667d-110">Permission type</span></span>|<span data-ttu-id="d667d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d667d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d667d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d667d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d667d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d667d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d667d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d667d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d667d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d667d-115">Not supported.</span></span>|
|<span data-ttu-id="d667d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d667d-116">Application</span></span>|<span data-ttu-id="d667d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d667d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d667d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d667d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="d667d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d667d-119">Request headers</span></span>
|<span data-ttu-id="d667d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d667d-120">Header</span></span>|<span data-ttu-id="d667d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d667d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d667d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d667d-122">Authorization</span></span>|<span data-ttu-id="d667d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d667d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d667d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d667d-124">Accept</span></span>|<span data-ttu-id="d667d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d667d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d667d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d667d-126">Request body</span></span>
<span data-ttu-id="d667d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d667d-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="d667d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d667d-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="d667d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d667d-129">Property</span></span>|<span data-ttu-id="d667d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d667d-130">Type</span></span>|<span data-ttu-id="d667d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d667d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d667d-132">id</span><span class="sxs-lookup"><span data-stu-id="d667d-132">id</span></span>|<span data-ttu-id="d667d-133">String</span><span class="sxs-lookup"><span data-stu-id="d667d-133">String</span></span>|<span data-ttu-id="d667d-134">Eindeutiger Bezeichner für den eingebetteten SIM-Aktivierungscode Pool.</span><span class="sxs-lookup"><span data-stu-id="d667d-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="d667d-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="d667d-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d667d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d667d-136">displayName</span></span>|<span data-ttu-id="d667d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d667d-137">String</span></span>|<span data-ttu-id="d667d-138">Der vom Administrator definierte Name des eingebetteten SIM-Aktivierungscode Pools.</span><span class="sxs-lookup"><span data-stu-id="d667d-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="d667d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d667d-139">createdDateTime</span></span>|<span data-ttu-id="d667d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d667d-140">DateTimeOffset</span></span>|<span data-ttu-id="d667d-141">Der Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d667d-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="d667d-142">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="d667d-142">Generated service side.</span></span>|
|<span data-ttu-id="d667d-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d667d-143">modifiedDateTime</span></span>|<span data-ttu-id="d667d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d667d-144">DateTimeOffset</span></span>|<span data-ttu-id="d667d-145">Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d667d-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="d667d-146">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="d667d-146">Updated service side.</span></span>|
|<span data-ttu-id="d667d-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="d667d-147">activationCodes</span></span>|<span data-ttu-id="d667d-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d667d-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="d667d-149">Die Aktivierungscodes, die zu diesem Pool gehören.</span><span class="sxs-lookup"><span data-stu-id="d667d-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="d667d-150">Diese Navigationseigenschaft wird verwendet, um Aktivierungscodes in InTune bereitzustellen, kann jedoch nicht zum Lesen von Aktivierungscodes aus InTune verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d667d-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="d667d-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="d667d-151">activationCodeCount</span></span>|<span data-ttu-id="d667d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d667d-152">Int32</span></span>|<span data-ttu-id="d667d-153">Die Gesamtanzahl der Aktivierungscodes, die zu diesem Pool gehören.</span><span class="sxs-lookup"><span data-stu-id="d667d-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="d667d-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="d667d-154">Response</span></span>
<span data-ttu-id="d667d-155">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d667d-155">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d667d-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d667d-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d667d-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d667d-157">Request</span></span>
<span data-ttu-id="d667d-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d667d-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d667d-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="d667d-159">Response</span></span>
<span data-ttu-id="d667d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d667d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```





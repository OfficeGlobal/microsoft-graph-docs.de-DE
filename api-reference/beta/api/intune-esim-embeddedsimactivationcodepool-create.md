---
title: Erstellen von embeddedSIMActivationCodePool
description: Erstellen eines neuen EmbeddedSIMActivationCodePool-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a5d01b376c886ef5753abbb59d0be557702e394f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891357"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="72d89-103">Erstellen von embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="72d89-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="72d89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="72d89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72d89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72d89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72d89-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72d89-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72d89-107">Erstellen eines neuen [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="72d89-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72d89-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="72d89-108">Prerequisites</span></span>
<span data-ttu-id="72d89-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d89-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="72d89-111">Permission type</span></span>|<span data-ttu-id="72d89-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="72d89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72d89-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="72d89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72d89-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d89-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72d89-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="72d89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72d89-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72d89-116">Not supported.</span></span>|
|<span data-ttu-id="72d89-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="72d89-117">Application</span></span>|<span data-ttu-id="72d89-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="72d89-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72d89-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="72d89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="72d89-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="72d89-120">Request headers</span></span>
|<span data-ttu-id="72d89-121">Header</span><span class="sxs-lookup"><span data-stu-id="72d89-121">Header</span></span>|<span data-ttu-id="72d89-122">Wert</span><span class="sxs-lookup"><span data-stu-id="72d89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72d89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d89-123">Authorization</span></span>|<span data-ttu-id="72d89-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="72d89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72d89-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="72d89-125">Accept</span></span>|<span data-ttu-id="72d89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72d89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d89-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="72d89-127">Request body</span></span>
<span data-ttu-id="72d89-128">Geben Sie im Textkörper Anforderung für das Objekt EmbeddedSIMActivationCodePool eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="72d89-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="72d89-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die EmbeddedSIMActivationCodePool erstellen.</span><span class="sxs-lookup"><span data-stu-id="72d89-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="72d89-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72d89-130">Property</span></span>|<span data-ttu-id="72d89-131">Typ</span><span class="sxs-lookup"><span data-stu-id="72d89-131">Type</span></span>|<span data-ttu-id="72d89-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72d89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d89-133">id</span><span class="sxs-lookup"><span data-stu-id="72d89-133">id</span></span>|<span data-ttu-id="72d89-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72d89-134">String</span></span>|<span data-ttu-id="72d89-135">Eindeutiger Bezeichner für den eingebetteten SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="72d89-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="72d89-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="72d89-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="72d89-137">displayName</span><span class="sxs-lookup"><span data-stu-id="72d89-137">displayName</span></span>|<span data-ttu-id="72d89-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72d89-138">String</span></span>|<span data-ttu-id="72d89-139">Der Administrator definierten Namen des eingebetteten SIM Aktivierung Code Pools.</span><span class="sxs-lookup"><span data-stu-id="72d89-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="72d89-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72d89-140">createdDateTime</span></span>|<span data-ttu-id="72d89-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d89-141">DateTimeOffset</span></span>|<span data-ttu-id="72d89-142">Der Zeitpunkt, zu der eingebettete SIM Aktivierung Code Pool erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="72d89-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="72d89-143">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="72d89-143">Generated service side.</span></span>|
|<span data-ttu-id="72d89-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72d89-144">modifiedDateTime</span></span>|<span data-ttu-id="72d89-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72d89-145">DateTimeOffset</span></span>|<span data-ttu-id="72d89-146">Der Zeitpunkt der letzten Änderung der eingebettete SIM Aktivierung Code Pool.</span><span class="sxs-lookup"><span data-stu-id="72d89-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="72d89-147">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="72d89-147">Updated service side.</span></span>|
|<span data-ttu-id="72d89-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="72d89-148">activationCodes</span></span>|<span data-ttu-id="72d89-149">[EmbeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="72d89-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="72d89-150">Die Aktivierungscodes in diesem Pool angehören.</span><span class="sxs-lookup"><span data-stu-id="72d89-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="72d89-151">Diese Navigationseigenschaft wird verwendet, um die Aktivierungscodes Intune buchen aber kann nicht zum Lesen von Aktivierungscodes aus Intune verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="72d89-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="72d89-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="72d89-152">activationCodeCount</span></span>|<span data-ttu-id="72d89-153">Int32</span><span class="sxs-lookup"><span data-stu-id="72d89-153">Int32</span></span>|<span data-ttu-id="72d89-154">Die Gesamtzahl der Aktivierungscodes in diesem Pool angehören.</span><span class="sxs-lookup"><span data-stu-id="72d89-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="72d89-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="72d89-155">Response</span></span>
<span data-ttu-id="72d89-156">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="72d89-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72d89-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="72d89-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="72d89-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="72d89-158">Request</span></span>
<span data-ttu-id="72d89-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="72d89-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
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

### <a name="response"></a><span data-ttu-id="72d89-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="72d89-160">Response</span></span>
<span data-ttu-id="72d89-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="72d89-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






---
title: Erstellen von „termsAndConditionsAcceptanceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97aca6b10d092301873536e436c825f3483d4a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990971"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="bad9a-103">Erstellen von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="bad9a-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="bad9a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bad9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bad9a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bad9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bad9a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bad9a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bad9a-107">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bad9a-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bad9a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bad9a-108">Prerequisites</span></span>
<span data-ttu-id="bad9a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bad9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bad9a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bad9a-111">Permission type</span></span>|<span data-ttu-id="bad9a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bad9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bad9a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bad9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bad9a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bad9a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bad9a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bad9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bad9a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bad9a-116">Not supported.</span></span>|
|<span data-ttu-id="bad9a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bad9a-117">Application</span></span>|<span data-ttu-id="bad9a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bad9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bad9a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bad9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bad9a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bad9a-120">Request headers</span></span>
|<span data-ttu-id="bad9a-121">Header</span><span class="sxs-lookup"><span data-stu-id="bad9a-121">Header</span></span>|<span data-ttu-id="bad9a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bad9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bad9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bad9a-123">Authorization</span></span>|<span data-ttu-id="bad9a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bad9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bad9a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bad9a-125">Accept</span></span>|<span data-ttu-id="bad9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bad9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bad9a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bad9a-127">Request body</span></span>
<span data-ttu-id="bad9a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAcceptanceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="bad9a-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="bad9a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAcceptanceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="bad9a-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="bad9a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bad9a-130">Property</span></span>|<span data-ttu-id="bad9a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bad9a-131">Type</span></span>|<span data-ttu-id="bad9a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bad9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bad9a-133">id</span><span class="sxs-lookup"><span data-stu-id="bad9a-133">id</span></span>|<span data-ttu-id="bad9a-134">String</span><span class="sxs-lookup"><span data-stu-id="bad9a-134">String</span></span>|<span data-ttu-id="bad9a-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="bad9a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="bad9a-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bad9a-136">userDisplayName</span></span>|<span data-ttu-id="bad9a-137">String</span><span class="sxs-lookup"><span data-stu-id="bad9a-137">String</span></span>|<span data-ttu-id="bad9a-138">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="bad9a-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="bad9a-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="bad9a-139">acceptedVersion</span></span>|<span data-ttu-id="bad9a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bad9a-140">Int32</span></span>|<span data-ttu-id="bad9a-141">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="bad9a-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="bad9a-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="bad9a-142">acceptedDateTime</span></span>|<span data-ttu-id="bad9a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bad9a-143">DateTimeOffset</span></span>|<span data-ttu-id="bad9a-144">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="bad9a-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="bad9a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="bad9a-145">Response</span></span>
<span data-ttu-id="bad9a-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bad9a-146">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bad9a-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bad9a-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="bad9a-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bad9a-148">Request</span></span>
<span data-ttu-id="bad9a-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bad9a-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bad9a-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="bad9a-150">Response</span></span>
<span data-ttu-id="bad9a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bad9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```






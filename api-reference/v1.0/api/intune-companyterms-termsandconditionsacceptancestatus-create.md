---
title: Erstellen von „termsAndConditionsAcceptanceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
ms.openlocfilehash: 4a371d2ac03ef47ad0af4ae70aa248dcd96e4bf0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348300"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="b7197-103">Erstellen von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="b7197-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="b7197-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b7197-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7197-105">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7197-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7197-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b7197-106">Prerequisites</span></span>
<span data-ttu-id="b7197-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7197-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7197-109">Permission type</span></span>|<span data-ttu-id="b7197-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7197-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7197-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7197-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7197-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7197-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7197-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7197-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7197-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7197-114">Not supported.</span></span>|
|<span data-ttu-id="b7197-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7197-115">Application</span></span>|<span data-ttu-id="b7197-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7197-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7197-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7197-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b7197-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7197-118">Request headers</span></span>
|<span data-ttu-id="b7197-119">Header</span><span class="sxs-lookup"><span data-stu-id="b7197-119">Header</span></span>|<span data-ttu-id="b7197-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b7197-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7197-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b7197-121">Authorization</span></span>|<span data-ttu-id="b7197-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b7197-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7197-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b7197-123">Accept</span></span>|<span data-ttu-id="b7197-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7197-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7197-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7197-125">Request body</span></span>
<span data-ttu-id="b7197-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAcceptanceStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="b7197-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="b7197-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAcceptanceStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b7197-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="b7197-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7197-128">Property</span></span>|<span data-ttu-id="b7197-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b7197-129">Type</span></span>|<span data-ttu-id="b7197-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7197-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7197-131">id</span><span class="sxs-lookup"><span data-stu-id="b7197-131">id</span></span>|<span data-ttu-id="b7197-132">String</span><span class="sxs-lookup"><span data-stu-id="b7197-132">String</span></span>|<span data-ttu-id="b7197-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="b7197-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b7197-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7197-134">userDisplayName</span></span>|<span data-ttu-id="b7197-135">String</span><span class="sxs-lookup"><span data-stu-id="b7197-135">String</span></span>|<span data-ttu-id="b7197-136">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="b7197-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="b7197-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="b7197-137">acceptedVersion</span></span>|<span data-ttu-id="b7197-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b7197-138">Int32</span></span>|<span data-ttu-id="b7197-139">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="b7197-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="b7197-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7197-140">acceptedDateTime</span></span>|<span data-ttu-id="b7197-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7197-141">DateTimeOffset</span></span>|<span data-ttu-id="b7197-142">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="b7197-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="b7197-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7197-143">Response</span></span>
<span data-ttu-id="b7197-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b7197-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7197-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7197-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7197-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7197-146">Request</span></span>
<span data-ttu-id="b7197-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7197-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b7197-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7197-148">Response</span></span>
<span data-ttu-id="b7197-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7197-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




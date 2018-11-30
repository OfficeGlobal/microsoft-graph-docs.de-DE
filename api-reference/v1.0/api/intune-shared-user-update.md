---
title: Benutzer aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
ms.openlocfilehash: cfb8a7d46d8383cdaae4f012cff4ed0a0ad93594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018495"
---
# <a name="update-user"></a><span data-ttu-id="74d21-103">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74d21-103">Update user</span></span>

> <span data-ttu-id="74d21-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="74d21-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74d21-105">Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="74d21-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74d21-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74d21-106">Prerequisites</span></span>
<span data-ttu-id="74d21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d21-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74d21-109">Permission type</span></span>|<span data-ttu-id="74d21-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74d21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74d21-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74d21-111">Delegated (work or school account)</span></span>| <span data-ttu-id="74d21-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="74d21-112">_varies by context_</span></span>|
| <span data-ttu-id="74d21-113">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="74d21-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="74d21-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d21-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="74d21-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="74d21-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="74d21-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d21-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="74d21-117">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="74d21-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="74d21-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d21-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="74d21-119">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="74d21-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="74d21-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d21-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="74d21-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74d21-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74d21-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74d21-122">Not supported.</span></span>|
|<span data-ttu-id="74d21-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74d21-123">Application</span></span>|<span data-ttu-id="74d21-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74d21-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74d21-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74d21-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="74d21-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74d21-126">Request headers</span></span>
|<span data-ttu-id="74d21-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="74d21-127">Header</span></span>|<span data-ttu-id="74d21-128">Wert</span><span class="sxs-lookup"><span data-stu-id="74d21-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74d21-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="74d21-129">Authorization</span></span>|<span data-ttu-id="74d21-130">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74d21-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74d21-131">Accept</span><span class="sxs-lookup"><span data-stu-id="74d21-131">Accept</span></span>|<span data-ttu-id="74d21-132">application/json</span><span class="sxs-lookup"><span data-stu-id="74d21-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74d21-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74d21-133">Request body</span></span>
<span data-ttu-id="74d21-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune-shared-user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="74d21-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="74d21-135">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune-shared-user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="74d21-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="74d21-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74d21-136">Property</span></span>|<span data-ttu-id="74d21-137">Typ</span><span class="sxs-lookup"><span data-stu-id="74d21-137">Type</span></span>|<span data-ttu-id="74d21-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74d21-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74d21-139">id</span><span class="sxs-lookup"><span data-stu-id="74d21-139">id</span></span>|<span data-ttu-id="74d21-140">String</span><span class="sxs-lookup"><span data-stu-id="74d21-140">String</span></span>|<span data-ttu-id="74d21-141">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="74d21-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="74d21-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="74d21-142">**Onboarding**</span></span>|
|<span data-ttu-id="74d21-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="74d21-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="74d21-144">Int32</span><span class="sxs-lookup"><span data-stu-id="74d21-144">Int32</span></span>|<span data-ttu-id="74d21-145">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="74d21-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="74d21-146">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="74d21-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="74d21-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="74d21-147">Response</span></span>
<span data-ttu-id="74d21-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74d21-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74d21-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74d21-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="74d21-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74d21-150">Request</span></span>
<span data-ttu-id="74d21-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74d21-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="74d21-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="74d21-152">Response</span></span>
<span data-ttu-id="74d21-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74d21-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




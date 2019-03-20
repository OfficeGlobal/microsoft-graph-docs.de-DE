---
title: Benutzer erstellen
description: Dient zum Erstellen eines neuen Benutzerobjekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46fbbc365e52ae9e46db9f6c05c3c8e8eeddc92
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572257"
---
# <a name="create-user"></a><span data-ttu-id="3c5ac-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="3c5ac-103">Create user</span></span>

> <span data-ttu-id="3c5ac-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3c5ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c5ac-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c5ac-107">Dient zum Erstellen eines neuen [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c5ac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3c5ac-108">Prerequisites</span></span>

<span data-ttu-id="3c5ac-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3c5ac-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c5ac-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="3c5ac-111">Die erforderliche Berechtigung hängt vom Kontext ab.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="3c5ac-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c5ac-112">Permission type</span></span>|<span data-ttu-id="3c5ac-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c5ac-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c5ac-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c5ac-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c5ac-115">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="3c5ac-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3c5ac-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5ac-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3c5ac-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3c5ac-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3c5ac-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5ac-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3c5ac-119">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="3c5ac-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3c5ac-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5ac-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3c5ac-121">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="3c5ac-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3c5ac-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c5ac-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3c5ac-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c5ac-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c5ac-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c5ac-124">Not supported.</span></span>|
|<span data-ttu-id="3c5ac-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c5ac-125">Application</span></span>|<span data-ttu-id="3c5ac-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c5ac-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c5ac-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c5ac-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="3c5ac-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3c5ac-128">Request headers</span></span>

|<span data-ttu-id="3c5ac-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3c5ac-129">Header</span></span>|<span data-ttu-id="3c5ac-130">Wert</span><span class="sxs-lookup"><span data-stu-id="3c5ac-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c5ac-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c5ac-131">Authorization</span></span>|<span data-ttu-id="3c5ac-132">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3c5ac-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c5ac-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3c5ac-133">Accept</span></span>|<span data-ttu-id="3c5ac-134">application/json</span><span class="sxs-lookup"><span data-stu-id="3c5ac-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c5ac-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3c5ac-135">Request body</span></span>

<span data-ttu-id="3c5ac-136">Geben Sie im Anforderungstext eine JSON-Darstellung des Benutzerobjekts an.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="3c5ac-137">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="3c5ac-138">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c5ac-138">Property</span></span>|<span data-ttu-id="3c5ac-139">Typ</span><span class="sxs-lookup"><span data-stu-id="3c5ac-139">Type</span></span>|<span data-ttu-id="3c5ac-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c5ac-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c5ac-141">id</span><span class="sxs-lookup"><span data-stu-id="3c5ac-141">id</span></span>|<span data-ttu-id="3c5ac-142">String</span><span class="sxs-lookup"><span data-stu-id="3c5ac-142">String</span></span>|<span data-ttu-id="3c5ac-143">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="3c5ac-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="3c5ac-144">**On-Boarding**</span><span class="sxs-lookup"><span data-stu-id="3c5ac-144">**On-boarding**</span></span>||
|<span data-ttu-id="3c5ac-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="3c5ac-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="3c5ac-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3c5ac-146">Int32</span></span>|<span data-ttu-id="3c5ac-147">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="3c5ac-148">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="3c5ac-149">Die Unterstützung für den Body-Anforderungstext variiert je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="3c5ac-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c5ac-150">Response</span></span>

<span data-ttu-id="3c5ac-151">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c5ac-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c5ac-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c5ac-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c5ac-153">Request</span></span>

<span data-ttu-id="3c5ac-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="3c5ac-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c5ac-155">Response</span></span>

<span data-ttu-id="3c5ac-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-156">Here is an example of the response.</span></span> <span data-ttu-id="3c5ac-157">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3c5ac-158">Von einem tatsächlichen Aufruf zurückgegebene Eigenschaften variieren je nach Kontext.</span><span class="sxs-lookup"><span data-stu-id="3c5ac-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




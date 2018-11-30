---
title: roleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines roleAssignment-Objekts.
ms.openlocfilehash: 64ec4aa3c885ce2c9de475faef1e00fd14f2576d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060022"
---
# <a name="update-roleassignment"></a><span data-ttu-id="0b40b-103">roleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0b40b-103">Update roleAssignment</span></span>

> <span data-ttu-id="0b40b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b40b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b40b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b40b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b40b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b40b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b40b-107">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0b40b-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b40b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b40b-108">Prerequisites</span></span>
<span data-ttu-id="0b40b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b40b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b40b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b40b-111">Permission type</span></span>|<span data-ttu-id="0b40b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b40b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b40b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b40b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b40b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b40b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0b40b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b40b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b40b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b40b-116">Not supported.</span></span>|
|<span data-ttu-id="0b40b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b40b-117">Application</span></span>|<span data-ttu-id="0b40b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b40b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b40b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b40b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0b40b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b40b-120">Request headers</span></span>
|<span data-ttu-id="0b40b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b40b-121">Header</span></span>|<span data-ttu-id="0b40b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b40b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b40b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b40b-123">Authorization</span></span>|<span data-ttu-id="0b40b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b40b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b40b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b40b-125">Accept</span></span>|<span data-ttu-id="0b40b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b40b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b40b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b40b-127">Request body</span></span>
<span data-ttu-id="0b40b-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="0b40b-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="0b40b-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleAssignment](../resources/intune-rbac-roleassignment.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0b40b-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="0b40b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b40b-130">Property</span></span>|<span data-ttu-id="0b40b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0b40b-131">Type</span></span>|<span data-ttu-id="0b40b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b40b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b40b-133">id</span><span class="sxs-lookup"><span data-stu-id="0b40b-133">id</span></span>|<span data-ttu-id="0b40b-134">String</span><span class="sxs-lookup"><span data-stu-id="0b40b-134">String</span></span>|<span data-ttu-id="0b40b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0b40b-135">Key of the entity.</span></span> <span data-ttu-id="0b40b-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="0b40b-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0b40b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0b40b-137">displayName</span></span>|<span data-ttu-id="0b40b-138">String</span><span class="sxs-lookup"><span data-stu-id="0b40b-138">String</span></span>|<span data-ttu-id="0b40b-139">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0b40b-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="0b40b-140">description</span><span class="sxs-lookup"><span data-stu-id="0b40b-140">description</span></span>|<span data-ttu-id="0b40b-141">String</span><span class="sxs-lookup"><span data-stu-id="0b40b-141">String</span></span>|<span data-ttu-id="0b40b-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0b40b-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="0b40b-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="0b40b-143">scopeMembers</span></span>|<span data-ttu-id="0b40b-144">String collection</span><span class="sxs-lookup"><span data-stu-id="0b40b-144">String collection</span></span>|<span data-ttu-id="0b40b-145">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="0b40b-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0b40b-146">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0b40b-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="0b40b-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="0b40b-147">scopeType</span></span>|[<span data-ttu-id="0b40b-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="0b40b-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="0b40b-149">Gibt den Typ des Bereichs für eine Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="0b40b-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="0b40b-150">Standardtyp 'ResourceScope' ermöglicht die Zuweisung von ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="0b40b-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="0b40b-151">Für 'AllDevices', 'AllLicensedUsers' und 'AllDevicesAndLicensedUsers' sollte die ResourceScopes-Eigenschaft leer bleiben.</span><span class="sxs-lookup"><span data-stu-id="0b40b-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="0b40b-152">Mögliche Werte: sind `resourceScope`, `allDevices`, `allLicensedUsers` und `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="0b40b-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="0b40b-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0b40b-153">resourceScopes</span></span>|<span data-ttu-id="0b40b-154">String collection</span><span class="sxs-lookup"><span data-stu-id="0b40b-154">String collection</span></span>|<span data-ttu-id="0b40b-155">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="0b40b-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0b40b-156">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0b40b-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="0b40b-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b40b-157">Response</span></span>
<span data-ttu-id="0b40b-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b40b-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b40b-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b40b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b40b-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b40b-160">Request</span></span>
<span data-ttu-id="0b40b-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b40b-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 224

{
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0b40b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b40b-162">Response</span></span>
<span data-ttu-id="0b40b-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b40b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```






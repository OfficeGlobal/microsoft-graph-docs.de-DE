---
title: deviceAndAppManagementRoleDefinition aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
ms.openlocfilehash: 74a66dc0480d9b856ee97f8a1c794659469d06b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309135"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="75c0e-103">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="75c0e-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="75c0e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="75c0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75c0e-105">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75c0e-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75c0e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75c0e-106">Prerequisites</span></span>
<span data-ttu-id="75c0e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c0e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75c0e-109">Permission type</span></span>|<span data-ttu-id="75c0e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75c0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75c0e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75c0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75c0e-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c0e-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="75c0e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75c0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75c0e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75c0e-114">Not supported.</span></span>|
|<span data-ttu-id="75c0e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75c0e-115">Application</span></span>|<span data-ttu-id="75c0e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75c0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75c0e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75c0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="75c0e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75c0e-118">Request headers</span></span>
|<span data-ttu-id="75c0e-119">Header</span><span class="sxs-lookup"><span data-stu-id="75c0e-119">Header</span></span>|<span data-ttu-id="75c0e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="75c0e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75c0e-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="75c0e-121">Authorization</span></span>|<span data-ttu-id="75c0e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="75c0e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75c0e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="75c0e-123">Accept</span></span>|<span data-ttu-id="75c0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="75c0e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75c0e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75c0e-125">Request body</span></span>
<span data-ttu-id="75c0e-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="75c0e-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="75c0e-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="75c0e-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="75c0e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75c0e-128">Property</span></span>|<span data-ttu-id="75c0e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="75c0e-129">Type</span></span>|<span data-ttu-id="75c0e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75c0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c0e-131">id</span><span class="sxs-lookup"><span data-stu-id="75c0e-131">id</span></span>|<span data-ttu-id="75c0e-132">String</span><span class="sxs-lookup"><span data-stu-id="75c0e-132">String</span></span>|<span data-ttu-id="75c0e-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="75c0e-133">Key of the entity.</span></span> <span data-ttu-id="75c0e-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="75c0e-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="75c0e-135">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75c0e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="75c0e-136">displayName</span></span>|<span data-ttu-id="75c0e-137">String</span><span class="sxs-lookup"><span data-stu-id="75c0e-137">String</span></span>|<span data-ttu-id="75c0e-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="75c0e-138">Display Name of the Role definition.</span></span> <span data-ttu-id="75c0e-139">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75c0e-140">description</span><span class="sxs-lookup"><span data-stu-id="75c0e-140">description</span></span>|<span data-ttu-id="75c0e-141">String</span><span class="sxs-lookup"><span data-stu-id="75c0e-141">String</span></span>|<span data-ttu-id="75c0e-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="75c0e-142">Description of the Role definition.</span></span> <span data-ttu-id="75c0e-143">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75c0e-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="75c0e-144">rolePermissions</span></span>|<span data-ttu-id="75c0e-145">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="75c0e-146">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="75c0e-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="75c0e-147">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="75c0e-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="75c0e-148">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="75c0e-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="75c0e-149">isBuiltIn</span></span>|<span data-ttu-id="75c0e-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="75c0e-150">Boolean</span></span>|<span data-ttu-id="75c0e-151">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="75c0e-151">Type of Role.</span></span> <span data-ttu-id="75c0e-152">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="75c0e-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="75c0e-153">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="75c0e-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="75c0e-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="75c0e-154">Response</span></span>
<span data-ttu-id="75c0e-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75c0e-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75c0e-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75c0e-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="75c0e-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75c0e-157">Request</span></span>
<span data-ttu-id="75c0e-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75c0e-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="75c0e-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="75c0e-159">Response</span></span>
<span data-ttu-id="75c0e-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75c0e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```




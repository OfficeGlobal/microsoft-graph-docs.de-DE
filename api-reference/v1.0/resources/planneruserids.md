# <a name="planneruserids-resource-type"></a><span data-ttu-id="47d05-101">plannerUserIds-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="47d05-101">plannerUserIds resource type</span></span>

<span data-ttu-id="47d05-p101">Die **plannerUserIds**-Ressource stellt die Liste der Benutzer-IDs dar, für die ein [Plan](plannerplan.md) freigegeben wird. Es handelt sich um einen offenen Typ. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="47d05-p101">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with. This is an Open Type. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="47d05-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47d05-106">Properties</span></span>
<span data-ttu-id="47d05-p102">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall sollte der Client Benutzer-IDs als Eigenschaften angeben, deren Wert das boolesche `true` ist. Wenn für Benutzer-IDs keine Freigabe mehr erfolgt, werden Eigenschaften automatisch entfernt, indem ihre Werte auf das boolesche `false` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="47d05-p102">Properties of an Open Type can be defined by the client. In this case, the client should provide user ids as properties with their values being the `true` boolean. When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="47d05-110">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47d05-110">JSON representation</span></span>

<span data-ttu-id="47d05-111">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47d05-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="47d05-112">// Beispiel</span><span class="sxs-lookup"><span data-stu-id="47d05-112">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
# ParticipationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acquired_at** | **date** | Datum des Erwerbs der Beteiligung. | [optional] 
**board_appointment** | **bool** | Bestellungsrecht für Geschäftsführung/Aufsichtsrat (§ 290 Abs. 2 Nr. 2 HGB). | [optional] 
**company_name** | **str** | Name des Beteiligungsunternehmens (§ 271 HGB). | [optional] 
**control_agreement** | **bool** | Beherrschungsvertrag (§ 290 Abs. 2 Nr. 3 HGB). | [optional] 
**legal_form** | **str** | Rechtsform, z. B. \&quot;GmbH\&quot;. | [optional] 
**ownership_pct** | **str** | Anteilsquote in Prozent (§ 271 HGB; &gt; 20 % widerlegbare Vermutung). | [optional] 
**purpose_vehicle** | **bool** | Zweckgesellschaft (§ 290 Abs. 2 Nr. 4 HGB). | [optional] 
**voting_majority** | **bool** | Stimmrechtsmehrheit (§ 290 Abs. 2 Nr. 1 HGB). | [optional] 

## Example

```python
from simplebilly_api.models.participation_update import ParticipationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ParticipationUpdate from a JSON string
participation_update_instance = ParticipationUpdate.from_json(json)
# print the JSON string representation of the object
print(ParticipationUpdate.to_json())

# convert the object into a dict
participation_update_dict = participation_update_instance.to_dict()
# create an instance of ParticipationUpdate from a dict
participation_update_from_dict = ParticipationUpdate.from_dict(participation_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



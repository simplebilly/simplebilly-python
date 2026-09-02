# Contact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_holder** | **str** |  | [optional] 
**acquisition_cost** | **str** |  | [optional] 
**address_supplement** | **str** |  | [optional] 
**attention** | **str** |  | [optional] 
**bank_name** | **str** |  | [optional] 
**bic** | **str** |  | [optional] 
**buyer_reference** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**certificate_authority** | **str** |  | [optional] 
**certificate_number** | **str** |  | [optional] 
**certificate_paragraph** | **str** |  | [optional] 
**certificate_valid_until** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**company_name** | **str** |  | [optional] 
**contact_id** | **str** |  | 
**contact_persons** | **object** |  | 
**contact_type** | **str** |  | 
**country** | **str** |  | [optional] 
**created_at** | **str** |  | [readonly] 
**credit_limit** | **str** |  | [optional] 
**creditor_account_skr03** | **str** |  | [optional] 
**creditor_account_skr04** | **str** |  | [optional] 
**currency** | **str** |  | [optional] 
**customer_number** | **str** |  | [optional] 
**debitor_account_skr03** | **str** |  | [optional] 
**debitor_account_skr04** | **str** |  | [optional] 
**default_debitor_number** | **str** |  | [optional] 
**delivery_block** | **bool** |  | [optional] 
**department** | **str** |  | [optional] 
**discount_days** | **int** |  | [optional] 
**discount_percentage** | **str** |  | [optional] 
**donation_receipt_eligible** | **bool** |  | [optional] 
**email** | **str** |  | [optional] 
**external_id** | **str** |  | [optional] 
**fax** | **str** |  | [optional] 
**iban** | **str** |  | [optional] 
**industry** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**is_member** | **bool** |  | [optional] 
**is_nonprofit** | **bool** |  | [optional] 
**last_contact_date** | **str** |  | [optional] 
**last_purchase_date** | **str** |  | [optional] 
**leitweg_id** | **str** |  | [optional] 
**lifetime_value** | **str** |  | [optional] 
**mandate_date** | **str** |  | [optional] 
**mandate_reference** | **str** |  | [optional] 
**marketing_consent** | **bool** |  | [optional] 
**marketing_consent_at** | **str** |  | [optional] 
**marketing_consent_source** | **str** |  | [optional] 
**mobile** | **str** |  | [optional] 
**name** | **str** |  | 
**next_contact_date** | **str** |  | [optional] 
**notes** | **str** |  | [optional] 
**opening_balance** | **str** |  | [optional] 
**opening_balance_date** | **str** |  | [optional] 
**order_reference** | **str** |  | [optional] 
**payment_block** | **bool** |  | [optional] 
**payment_grace_period_days** | **int** |  | [optional] 
**payment_methods** | **List[str]** |  | [optional] 
**payment_terms** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**rating** | **int** |  | [optional] 
**sales_representative** | **str** |  | [optional] 
**social_media** | **object** |  | 
**source** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**street** | **str** |  | [optional] 
**street_number** | **str** |  | [optional] 
**supplier_number** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**tax_country** | **str** |  | [optional] 
**tax_number** | **str** |  | [optional] 
**tax_office** | **str** |  | [optional] 
**total_invoices** | **int** |  | [optional] 
**total_revenue** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] [readonly] 
**vat_id** | **str** |  | [optional] 
**vat_id_validated** | **bool** |  | [optional] 
**vat_id_validation_date** | **str** |  | [optional] 
**website** | **str** |  | [optional] 
**zip** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.contact import Contact

# TODO update the JSON string below
json = "{}"
# create an instance of Contact from a JSON string
contact_instance = Contact.from_json(json)
# print the JSON string representation of the object
print(Contact.to_json())

# convert the object into a dict
contact_dict = contact_instance.to_dict()
# create an instance of Contact from a dict
contact_from_dict = Contact.from_dict(contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



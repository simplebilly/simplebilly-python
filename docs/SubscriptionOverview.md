# SubscriptionOverview

Tenant subscription overview for the billing page: current plan, status, period end, trial state, effective limits, current usage and feature flags. Backed by Paddle Billing webhook data written into `billing_info` + `tenants.plan`, and by the canonical plans in `crate::saasy::plans`.  JSON contract (camelCase, matches the frontend): `plan`, `planName`, `priceEur`, `status`, `currentPeriodEnd`, `manageUrl`, `trialEndsAt`, `isTrialing`, `limits:{maxUsers,maxInvoicesPerMonth,maxConnectors}`, `usage:{users,invoicesThisMonth,connectors,overageSeats}`, `features:{taxAutomations,fancyReports,erp}`.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_period_end** | **datetime** |  | [optional] 
**features** | [**PlanFeatures**](PlanFeatures.md) |  | 
**is_trialing** | **bool** |  | 
**limits** | [**PlanLimits**](PlanLimits.md) |  | 
**manage_url** | **str** |  | [optional] 
**plan** | **str** | Resolved plan id (free/starter/business/enterprise, or a custom override id). | 
**plan_name** | **str** |  | 
**price_eur** | **float** | Monthly price in EUR; &#x60;-1.0&#x60; &#x3D; custom pricing (enterprise). | 
**quantity** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**subscription_id** | **str** |  | [optional] 
**trial_ends_at** | **datetime** |  | [optional] 
**usage** | [**UsageSnapshot**](UsageSnapshot.md) |  | 

## Example

```python
from simplebilly_api.models.subscription_overview import SubscriptionOverview

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionOverview from a JSON string
subscription_overview_instance = SubscriptionOverview.from_json(json)
# print the JSON string representation of the object
print(SubscriptionOverview.to_json())

# convert the object into a dict
subscription_overview_dict = subscription_overview_instance.to_dict()
# create an instance of SubscriptionOverview from a dict
subscription_overview_from_dict = SubscriptionOverview.from_dict(subscription_overview_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



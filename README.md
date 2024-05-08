# Subscription Contract README

## Overview
This repository contains the code for a subscription contract implemented using the Soroban SDK. The contract allows users to create and manage subscriptions for various services.

## File Breakdown
- `lib.rs`: Contains the implementation of the subscription contract.
  
## Code Structure
- `Subscription`: Structure to store a single subscription, including user address, service ID, start time, and end time.
- `DataKey`: Enum defining the data key for storing subscriptions.
- `SubscriptionContract`: Trait defining contract functions such as creating subscriptions and checking if a subscription is active.
  
## Usage
To use this contract, integrate it into your Soroban-based application and implement the necessary environment and data handlers.

## Functions
### `create_subscription`
Creates a new subscription for a user to a specific service for a given duration.

#### Parameters
- `env`: Environment context.
- `user`: User address.
- `service_id`: Identifier of the service.
- `duration`: Duration of the subscription in seconds.

### `is_subscription_active`
Checks if a subscription for a user to a specific service is active.

#### Parameters
- `env`: Environment context.
- `user`: User address.
- `service_id`: Identifier of the service.

#### Returns
- `true` if the subscription is active, `false` otherwise.

## Additional Functions
Additional functions can be added to the `SubscriptionContract` trait as needed, such as renewing or canceling subscriptions.



---
title: HomeViewModel
description: A placeholder page for your new documentation site.
---

# HomeViewModel Documentation

The `HomeViewModel` is responsible for managing the state and business logic for the home screen of the application. It follows the MVVM (Model-View-ViewModel) architecture pattern to separate concerns and improve testability.

## Properties

### `isLoading: Bool`
A boolean value indicating whether the view is currently in a loading state. This is used to show or hide loading indicators in the UI.

### `errorMessage: String?`
An optional string that contains an error message to be displayed to the user if an operation fails. This is typically set when an API call or data fetch operation encounters an error.

### `featuredItems: [Item]`
An array of `Item` objects representing the featured items to be displayed on the home screen. These items are typically fetched from a remote API or local database.

## Methods

### `fetchFeaturedItems()`
Fetches the featured items from the data source (e.g., API or database) and updates the `featuredItems` property. This method also handles loading states and errors.

### `refreshData()`
Refreshes the data on the home screen by calling `fetchFeaturedItems()` and optionally performing additional refresh operations.

## Example Usage
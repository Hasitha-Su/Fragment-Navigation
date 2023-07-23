# Fragment Navigation in Android with Kotlin

This repository contains the code for an Android application that demonstrates the implementation of fragment navigation in Kotlin. Currently, the application supports navigation between two fragments using the FragmentManager and FragmentTransaction.

## Branch: feature/fragment-transaction-navigation

The `feature/fragment-transaction-navigation` branch contains the implementation of fragment navigation using FragmentTransactions. This involves replacing one fragment with another when a button is clicked. The application currently supports navigation between two fragments: `Fragment1` and `Fragment2`.

The code in this branch consists of:

1. `MainActivity`: The primary activity which hosts the fragments. It also contains button click listeners that trigger the fragment transactions.
2. `Fragment1` and `Fragment2`: The two fragments between which the application navigates. Currently, these fragments only inflate their respective layout files.

### Improvements

1. **Use Android Navigation Component**: Part of Android Jetpack, the Navigation Component simplifies the implementation of navigation, including the back stack, deep linking, and navigating to dialogs and menus.
2. **Use ViewModel and LiveData (or StateFlow)**: ViewModel can help manage and store UI-related data in a lifecycle-conscious way, allowing it to survive configuration changes. LiveData or Kotlin's StateFlow can be used to observe data and update the UI accordingly.
3. **Fragment Encapsulation**: Encapsulate the creation of fragments inside the fragments themselves. This can improve the modularity and readability of the code.

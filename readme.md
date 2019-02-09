# Accessible App - Central briefing
v1.0, December 01, 2018

## Introduction
The goal is to build a Single Page Application in React, Vue, and Angular respectively. This SPA is called "Accessibooks" and will be a dummy e-commerce app. It will be having typical features for this kind of app and Accessible App's goal is to showcase how these features can be built in an accessible way.

## Requirements
To do this it is necessary to research:

* If the JavaScript framework supplies accessible components by default
* If the JavaScript framework's documentation promotes inclusive design strategies
* If there are ready-made, accessible components available from third parties
* Strategies to use the frameworks abilities to reach an accessible result anyways, if none of the above is provided

## Scope
The example app shall be a simple e-commerce app where you can buy books about accessibility. As routing is common place in Single Page Applications the example book store will consist of several page states that can be accessed by their own URI. With the aid of typical e-commerce features like a shopping cart the app aims to showcase, for example, the use of notifications, focus management and buttons in a web app. Furthermore the app will include typical widgets that you often find outside Single Page Applications, such as: Off Canvas navigation, (modal) dialog windows, menu buttons and data-tables.

## Schema
```YAML
App
    Wrapper
        Header
            Logo
            Nav (1)
            User Actions
                Account (2)
                ShoppingCart
        MainContent (3)
            ProductListing
                ProductTable (4)
                    InfoButton, opens dialog (5)
                    AddToCart button
            AboutPage
    ModalPortal (5)
```
## Legend
1. Route Links
2. Menu Button
3. Where focus will be sent to after route transition (either via Reach Router in the React version of the sample app, [a Vue routing strategy, see blog post](https://marcus.io/blog/accessible-routing-vuejs), or via I-don't-know-yet in Angular)
4. Data table for book products, sortable by table head (author, title, year published, price)
5. This is the part of the DOM where dialogs will be placed.

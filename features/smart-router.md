---
description: Infinite control over managing your payments
---

# 🛣 Smart Router

{% hint style="info" %}
With this section, understand how the Hyperswitch Smart Router works to improve your conversion rates and reduces processing costs by intelligently routing payments across various processors
{% endhint %}

## Prerequisites

To get started with Smart Router, ensure to have one or more payment processors integrated. You can integrate the payment processor of your choice on the Control Center by following the [Connector Integration](../hyperswitch-cloud/connectors/) guide.

## What is smart payment routing?

Selling globally or otherwise invariably brings in a requirement to adopt multiple payment processors to cater to a wide range of payment method needs of the customers and gives you the flexibility to switch between processors to manage down-time and , it could be vital to optimising your payment processing costs as your business can choose the most optimal payment processors for every payment based on the cost, region and customer.

Hence, Hyperswitch’s smart router is designed as a no-code tool to provide complete control and transparency in creating and modifying payment routing rules. Hyperswitch supports below formats of Smart Routing.

**Volume Based Configuration:** Define volume distribution among multiple payment processors using percentages.

**Rule Based Configuration:** More granular control which allows to define custom routing logics based on different parameters of payment.

**Default Fallback Routing :** If the active routing rules are not applicable, the priority order of all configured payment processors is used to route payments. This priority order is configurable from the Dashboard.

**Cost Based Configuration** (submit a feature request [here](https://github.com/juspay/hyperswitch/discussions/new?category=ideas-feature-requests))**:** Automatically routes transaction to the payment processor charging the least MDR (merchant discount rate) for the opted payment method.

## How does the Smart Router work?

Hyperswitch Smart Router Engine evaluates every payment request against your predefined routing logic and makes a decision on the best payment processor for the payment, and executes the transaction. If the payment fails or if the payment processor is down, the payment is automatically retried through a different processor.

<figure><img src="../.gitbook/assets/Smart Routing Flow.drawio.png" alt=""><figcaption><p>Hyperswitch Smart Router Flow</p></figcaption></figure>

## How to configure the Smart Router?

[Hyperswitch dashboard](https://app.hyperswitch.io/routing) provides a simple, intuitive UI to configure multiple Routing rules on your dashboard under the **Routing** tab. There are three routing rule formats that Hyperswitch currently supports.\
\


<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td><strong>Rule Based Routing</strong></td><td></td><td></td><td><a href="merchant-controls/smart-router/rule-based-routing.md">rule-based-routing.md</a></td><td><a href="../.gitbook/assets/rule-based.png">rule-based.png</a></td></tr><tr><td><strong>Volume Based Routing</strong></td><td></td><td></td><td><a href="merchant-controls/smart-router/volume-based-routing.md">volume-based-routing.md</a></td><td><a href="../.gitbook/assets/volume-based.png">volume-based.png</a></td></tr><tr><td><strong>Default Fallback Routing</strong></td><td></td><td></td><td><a href="merchant-controls/smart-router/default-fallback-routing.md">default-fallback-routing.md</a></td><td><a href="../.gitbook/assets/default.png">default.png</a></td></tr></tbody></table>

## Next step&#x20;

To test the Smart Router, after activating one rule, we can make a Test Payment using the [Hyperswitch Dashboard ](https://app.hyperswitch.io/sdk)

{% content-ref url="../hyperswitch-open-source/test-a-payment.md" %}
[test-a-payment.md](../hyperswitch-open-source/test-a-payment.md)
{% endcontent-ref %}

## How to setup the Smart Router?

{% embed url="https://hyperswitch.io/video/edit_conf.mp4" %}


# Shipyard

## Overview

Shipyard unblocks DevOps teams from bulky, outdated production pipelines. We resolve the pre-production or staging bottleneck with our agile on-demand ephemeral (testing or preview) environments.

The Datadog Shipyard integration automatically passes your [Shipyard][1] ephemeral environment logs to your Datadog dashboard. For every application you have enables the Datadog logs for, Shipyard sends the runtime logs of your application to your dashboard. 

This is useful for: 

- monitoring your application’s runtime status
- using Datadog to enrich and parse your runtime logs
- uncover trends and compare the logs from your application’s environments using Datadog’s easy to use interface

## Setup

These instructions assume you have a Shipyard account and application set up. If you do not, you can get started [for free][2]. For more information about setting up the Datadog integration, see the [Shipyard documentation][7]. 

### Configuration

1. Navigate to the [API Keys page][5] and create an API key.
2. In your Shipyard dashboard, go to **Settings**. 
3. Under the Datadog section, enter your Datadog API key and the Datadog site URL. *Note: The site URL is not required and therefore we suggest you try your connection with just your API key to begin with*
   ![datadog-input][6]
   1. If you do not see a Datadog section here, email [support@shipyard.build][3] to enable this feature for your organization.
   2. To get the Datadog site URL, see [Getting Started with Datadog Sites][4] and compare your dashboard's site URL to the ones in the table.
3. Click **Install Datadog**.
   1. Optionally, toggle `enable Datadog logging for all environments`, Shipyard will automatically send the logs for all your environments.
4. To select specific environments from which you want to send logs for each repo, see the [Configure Application page][10]. 
   1. Select the **Notification Settings** tab. 
   2. Toggle `Enable Datadog logging` for this environment.

## Data Collected

### Metrics

Shipyard does not include any metrics.

### Service Checks

Shipyard does not include any service checks.

### Events

Shipyard does not include any events.

## Troubleshooting

Need help? Contact [Shipyard support][3].

[1]: https://shipyard.build/
[2]: https://shipyard.build/signup
[3]: mailto:support@shipyard.build
[4]: https://docs.datadoghq.com/getting_started/site/#access-the-datadog-site
[5]: https://app.datadoghq.com/organization-settings/api-keys
[6]: https://raw.githubusercontent.com/mesmith027/DataDog-integrations-extras/shipyard-integration/shipyard/images/datadog-input.png
[7]: https://docs.shipyard.build/docs/integrations/#send-logs-to-datadog
[8]: https://www.datadoghq.com/solutions/log-analysis-and-correlation/
[9]: https://www.datadoghq.com/solutions/shift-left-testing/
[10]: https://docs.shipyard.build/docs/config
# Google Cloud Platform Integration

This integration is used to fetches logs and metrics from 
[Google Cloud Platform](https://cloud.google.com/).

## GCP Credentials
GCP credentials are required for running GCP integration. 

### Configuration parameters
* *project_id*: ID of the GCP project.
* *credentials_file*: Path to JSON file with GCP credentials. Required when not using `credentials_json`.
* *credentials_json*: Raw JSON text of GCP Credentials. Required when not using `credentials_file`.

<<<<<<< HEAD
This is the `audit` dataset.

{{event "audit"}}

{{fields "audit"}}

### Firewall

This is the `firewall` dataset.

{{event "firewall"}}

{{fields "firewall"}}

### VPC Flow

This is the `VPC Flow` dataset.

{{event "vpcflow"}}

{{fields "vpcflow"}}

### DNS

This is the `DNS` dataset.

{{event "dns"}}

{{fields "dns"}}
=======
#### Data stream specific configuration parameters
* *period*: How often the data stream is executed.
* *region*: Specify which GCP regions to query metrics from. If the `region`
is not set in the config, then by default, the integration will query metrics
from all available GCP regions. If both `region` and `zone` is set, `region` takes precedent.
* *zone*: Specify which GCP zones to query metrics from. If the `zone`
is not set in the config, then by default, the integration will query metrics
from all available GCP zone. If both `region` and `zone` is set, `region` takes precedent.
* *exclude_labels*: Exclude additional labels from metrics.  Defaults to false.
>>>>>>> 64004cdad ([GCP] Add GCP Billing Metricset (#2141))

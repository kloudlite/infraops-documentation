---
description: Step-by-Step Guide to setup your cloud provider
---

# Add your Cloud Provider

You can setup your cloud provider while creating your account.&#x20;

If you already have an existing kloudlite account you can create cloud providers from dashboard&#x20;

`Dashboard > Settings > Cloud Providers`

**Step-by-Step Guide to setup your cloud provider.**

{% tabs %}
{% tab title="AWS" %}
### **Create a New Cloud Provider**:

<figure><img src="../.gitbook/assets/Screenshot 2024-01-26 at 8.36.31 AM.png" alt=""><figcaption></figcaption></figure>

* Give relevant name to cloud provider
* Choose 'Amazon Web Services' and enter your Account ID and **proceed** to generate cloudformation stack URL.

### **Create CloudFormation Stack**

<figure><img src="../.gitbook/assets/Screenshot 2024-01-26 at 8.37.00 AM (2).png" alt=""><figcaption><p>Open the URL generated to create cloud formation stack in your AWS account.</p></figcaption></figure>

* Copy the provided URL for cloud-formation stack creation.
* Open this URL in a browser where you are already logged into your AWS account/sub-account.
* Proceed with the CloudFormation stack creation steps as guided.

<mark style="color:orange;background-color:yellow;">**Note:**</mark> <mark style="color:orange;background-color:yellow;"></mark><mark style="color:orange;background-color:yellow;">If you want to use Kloudlite with less expansive permissions than what is provisioned by the CloudFormation stack, please</mark> [<mark style="color:orange;background-color:yellow;">contact us</mark>](https://cal.com/talk-to-porter/15min) <mark style="color:orange;background-color:yellow;">to inquire about Kloudlite Enterprise. In Kloudlite Enterprise we can customise the scope based on your requirements. You can explore all other benefits of Kloudlite Enterprise from here.</mark>

### **Verification**

* Once the stack installation is complete, Kloudlite will gain access to your AWS account.
* Verify this connection in your Kloudlite dashboard to ensure everything is set up correctly.
{% endtab %}

{% tab title="GCP" %}
### **Enable GCP APIs**

<figure><img src="https://imagedelivery.net/l4LYM_vOYKe7O1NCT_Nc_g/75c924c8-88d4-40a7-5a35-5e29261f4d00/large" alt=""><figcaption></figcaption></figure>

To use Kloudlite on GCP, you must first enable some APIs on your project.

* Navigate to the **APIs & Services** tab of your project.
* Click on the **Enable APIs and Services** button at the top. This will bring up a catalog of APIs that you can enable on GCP. Enable the following APIs:
  * Compute Engine API
  * Cloud Resource Manager API

It might take a few minutes for each of these APIs to be enabled. Once you can confirm that all five APIs are enabled from the **APIs & Services** tab, proceed to the next section.

### Create Service Account

First, go to your [Google Cloud console](https://console.cloud.google.com/) and navigate to **IAM & Admin** -> **Service Accounts**

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Select Create Service Account

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

After naming your service account, grant the service account these three permissions:

1. **Cloud Storage > Storage Admin**
2. **Compute Engine > Compute Admin**
3. **Service Accounts > Service Account User**

Select **Done** to create the service account.

### Generate Access Keys

Once the service account has been created, under **Actions** select **Manage keys**.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

Select **ADD KEY** -> **Create new key** and then choose **JSON** as your key type. After creation, your JSON key will automatically be downloaded as a file. You will need this key later.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

### Create Cloud Provider

<figure><img src="../.gitbook/assets/Screenshot 2024-01-26 at 8.36.31 AM.png" alt=""><figcaption></figcaption></figure>

* Give relevant name to cloud provider
* Choose 'Google Cloud Provider' & Upload the generated key and **proceed**
* Validate your key and proceed
{% endtab %}

{% tab title="Azure (Coming Soon)" %}
Will be available soon!
{% endtab %}

{% tab title="Suggest More..." %}
Feel free to suggest your favourite providers!! Drop your suggestions [here](https://github.com/orgs/kloudlite/discussions/categories/ideas)!
{% endtab %}
{% endtabs %}

With your cloud provider creation completed, you are now ready to [create your first cluster](create-your-first-cluster.md) using Kloudlite!

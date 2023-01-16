## Building Transformations and Preparing Data with Wrangler in Cloud Data Fusion

This project uses a CSV file stored in a google bucket. 

### Project Permissions:
Before you begin working on Google Cloud, you must ensure that your project has the correct permissions within Identity and Access Management (IAM).

In the Google Cloud console, on the Navigation menu (Navigation menu icon), click IAM & Admin > IAM.

Confirm that the default compute Service Account {project-number}-compute@developer.gserviceaccount.com is present and has the editor role assigned. The account prefix is the project number, which you can find on Navigation menu > Cloud overview.

### Grant Cloud Data Fusion required IAM access

#### Add necessary permissions for your Cloud Data Fusion instance
In the Cloud console, from the Navigation menu select Data Fusion > Instances. You should see a Cloud Data Fusion instance already setup and ready for use.
Next, you will grant permissions to the service account associated with the instance, using the following steps.

Click on the instance name. On the Instance details page copy the Service Account to your clipboard.

From the Cloud Console navigate to the IAM & Admin > IAM.

On the IAM Permissions page, click +Grant Access.

In the New principals field paste the service account.

Click into the Select a role field and start typing "Cloud Data Fusion API Service Agent", then select it.

Click Save.
:original_name: seller.html

Seller
======

In this section we talk about how to use Marketplace as a “Seller”. This includes how to become a marketplace seller and how to on-board, manage and eventually off-board a product.

Become a Seller
---------------

Anyone who has a Tennent in Open Telekom Cloud can request to become a seller in Marketplace. The process is quite straight forward.

As shown in the picture there is a link available to request for that when you click on Login as a Seller.

.. image:: /_static/images/image1.png
   :width: 6.53194in
   :height: 1.88264in

After clicking you would be redirected to a page where you are supposed to login with your OTC account.

.. image:: /_static/images/image2.png
   :width: 6.53194in
   :height: 4.09097in

Please be aware that only users which has “Tenant Administrator” role can submit a request for their tenant to become a Seller.

After login, as show below, you need to accept the terms and conditions and provide an email which would be used by Marketplace to contact Seller for any notification.

When the request has been submitted, you would receive an email which let you know the process of on boarding you as a Seller in Marketplace has been started and soon you would be informed about that.

As Open Telekom Cloud needs to follow some procedures this action might take few working-days.

Eventually, you would receive an email which informs you that you have become a Marketplace Seller would be able to start offering your products in Marketplace.

Login
-----

As shown in the picture Login to Marketplace as a Seller is straight forward and you can login using your IAM account.

Note: It is recommended to use Chrome or Microsoft Edge to login as the seller.

Please be aware that to login as the “Seller” you first need to become a seller in OTC Marketplace.

.. image:: /_static/images/image3.png
   :width: 6.53194in
   :height: 1.69097in

Please be aware that only users which has “Tenant Administrator” role can login to the Marketplace as a Seller.

.. image:: /_static/images/image4.png
   :width: 6.53194in
   :height: 3.28681in

If the login is successful, then you would see the page as bellow. There you can select a product to deploy and use.

.. image:: /_static/images/image5.png
   :width: 6.53194in
   :height: 4.06944in

.. _publish-product-offering-1:

Publish Product Offering
------------------------

In Section we would talk about how to create a product to be offered to Customers. Based on the type of product and licensing the procedure mightily differ. The main step would be first deciding what type of Product with which type of licensing the offer would be.

Please be aware that type and licensing model of the product are not changeable at all. This means if the product has been created as a “Free” licensing for a CCE type application, it cannot be changed to any other type of product with different licensing model.

CCE Open Source, Free or Trial
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you have a Helm Chart to deploy an application and your product is free to be used (as Open Source, Free or Trial), then this is the right choice to on-board that on Marketplace.

First step would be login Marketplace as a Seller as show in this picture.

.. image:: /_static/images/image6.png
   :width: 6.53194in
   :height: 1.79306in

Please be aware that only users which has “Tenant Administrator” role can login to the Marketplace as a Seller.

.. image:: /_static/images/image7.png
   :width: 6.53194in
   :height: 3.53889in

On the right side of the page, you would see a button named “Dashboard”.

.. image:: /_static/images/image8.png
   :width: 6.53194in
   :height: 2.42431in

Please click that and then select “Offering”.

.. image:: /_static/images/image9.png
   :width: 6.53194in
   :height: 2.35139in

Click on the new Offering to be forwarded to the new page to create your product. There you should fill out all the required information as needed.

.. image:: /_static/images/image10.png
   :width: 6.53194in
   :height: 3.05278in

Product Offering Name
^^^^^^^^^^^^^^^^^^^^^

Here you should pick up a name for your product. Customers would find you product in Marketplace with that name.

Please be aware that the product name is permanent and cannot be change as marketplace is committed to Customers that they always refer to the same name for specific product.

Service Type
^^^^^^^^^^^^

Here you should choose which type of product it would be. So far you can only choose CCE as the type of Product which is for Helm Charts to be offered.

License Type
^^^^^^^^^^^^

As mentioned before, you are supposed to choose between Open Source, Free or Trial. This means that customer will get charged 0.00€ if they deploy that product.

License Info
^^^^^^^^^^^^

Here you can put information about licensing of your product which would be shown to customers when they select your Product inside Marketplace.

EULA
^^^^

Each company has some terms and conditions that clients need to agree on before using that product. Here Seller can add his/her EULA. When a customer wants to deploy that product, he/she needs to agree on that before being able to deploy that application.

Category
^^^^^^^^

Here you can select in which category your product would fit in. Customer would filter product inside marketplace based on specific Category.

Version
^^^^^^^

Here you can set the version of your application so Customers would know which version of that has been presented in Marketplace.

Short Description
^^^^^^^^^^^^^^^^^

Short Description is the information that would be shown to Customers when they find it inside main page of Marketplace. This could be a brief introduction about the product that seller is offering.

Full Description
^^^^^^^^^^^^^^^^

When a customer would find and select a product, this description would go into details of that product and Customer can read and find more information about that product.

Logo
^^^^

Here Seller is supposed to upload the logo of his/her product.

“Used Software”, “Used Software License Name” and “Link to License”
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As each application might have used other applications as component, Customers has the right to know which software has been used for that product. This include the name of that and name of the license that has been used for that (Such as MIT or Apache v2.0) so they could be able to review that and make sure this does not violate their policies.

This list of component's license information would be shown as the detail of the product.

Add Configuration
^^^^^^^^^^^^^^^^^

As the product is a Helm Chart, it has many keys that customer can customized by overwriting with new values. Although Helm Chart could have many keys to get customized, it is up to seller with of them should be on-boarded on Marketplace, so Customers be able to manipulate them.

Please be aware that some keys that have been added by seller to customize deployment could also be hidden to customer. This can be used when your help chart needs to be modified based on Open Telekom Cloud CCE and seller wants to make that change permanent, so customers did not change it by mistake.

Configurations could be a “Text input” (Text or Array), Option (Text or Array) which is like “Text Input” but default values are fixed and customer can only select from those values to choose or a Toggle (Boolean) that customer needs to make it as True or False.

Text input
''''''''''

This can be used for adding a key which is the type of string or array.

.. image:: /_static/images/image11.png
   :width: 6.53194in
   :height: 3.77361in

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

Text input label
                

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

Required
        

There are some configurations that could be optional or mandatory. If customer sets it then during deployment it would be overwrite and if not the default value form “values.yaml” would be picked up.

If there is a configuration that seller wants the customer to change it, then he/she can enable the required toggle so customers should put value for that.

Confidential
            

Some keys include some confidential information that during filling the key by customer, it should be treated as a confidential information and the content should be hidden.

For example, if the key is the default password of the application, then the seller can enable this feature. During the configuration it would be treated as a password and content cannot be seen during filling the information.

Validation Rule
               

If sellers want to restrict the content that customer would write as the value of that key, he/she can put regex rule, so customer are forced to follow that rule during filling the value. For that regex rule there is a “Error message” which seller can put hint or example to help customers to understand about the condition that is required.

Hidden
      

If seller enables that, then that configuration would be overwrite default helm chart value. However, customers are not able to see or change the content of that.

Please be aware that in that case “Default value” needs to be filled.

Multiple
        

This is the place where seller can set this configuration as an array. If multiple has been enabled, then customer can put more than one value for that key.

Default value
             

If seller wants, he/she can default value for that configuration. Customers would still be able to overwrite that.

Hint text
         

This column could help customers by adding a hint under the label which could provide more help for Customers. It appears as a short line beneath that configuration label.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Hint text as “Kubernetes Storage Class for disk”. In that case customer would see a label named “storageClass” and beneath that a like which says, “Kubernetes Storage Class for disk”.

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global.storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

Option
''''''

This can be used for adding a key which is the type of string or array. The only difference is that Seller makes the values to pick up prepared so customers can only pick from those lists. For instance, imagine you have a key “serviceType” and the answer should only be “ClusterIP”, “Nodeport” or “LoadBalancer”. Then the seller can pick that as the type of configuration and already add those as the pre-defined values.

.. image:: /_static/images/image12.png
   :width: 6.53194in
   :height: 3.69097in

.. _configuration-key-1:

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

Optional label
              

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

Label/Value
           

There should a list of possible values to choose and a label for reach to help customer to understand which one to choose based on the situation.

.. _multiple-1:

Multiple
        

This is the place where seller can set this configuration as an array. If multiple has been enabled, then customer can put more than one value for that key.

.. _default-value-1:

Default value
             

If seller wants, he/she can default value for that configuration. Customers would still be able to overwrite that.

.. _hint-text-1:

Hint text
         

This column could help customers by adding a hint under the label which could provide more help for Customers. It appears as a short line beneath that configuration label.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Hint text as “Kubernetes Storage Class for disk”. In that case customer would see a label named “storageClass” and beneath that a like which says, “Kubernetes Storage Class for disk”.

.. _tooltip-text-1:

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

Toggle
''''''

This can be used for adding a key which is the type of Boolean.

.. image:: /_static/images/image13.png
   :width: 6.53194in
   :height: 3.75764in

.. _configuration-key-2:

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

Toggle/label
            

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

Default State
             

This variable by default is whether true or false.

.. _hidden-1:

Hidden
      

If seller enables that, then that configuration would be overwrite default helm chart value. However, customers are not able to see or change the content of that.

Please be aware that in that case “Default value” needs to be filled.

.. _tooltip-text-2:

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

Add pre-Deployment guide
^^^^^^^^^^^^^^^^^^^^^^^^

When a customer selects a product, this message would be show on the screen to him/her. Here seller can provide pre-deployment hints or guidance that customer can be aware before the deployment.

This is a good place for guiding customers who wants to use that product.

.. image:: /_static/images/image14.png
   :width: 6.53194in
   :height: 2.74583in

Add deployment guide
^^^^^^^^^^^^^^^^^^^^

Although hints and tooltips that seller would add to each configuration could be descriptive, seller needs to prepare small document to depict how to deploy and customize that product. The whole content would be shown to customer as an installation guide.

.. image:: /_static/images/image15.png
   :width: 6.53194in
   :height: 2.72431in

Post post-deployment guide
^^^^^^^^^^^^^^^^^^^^^^^^^^

When a customer selects a product and deploys that, this message would be show on the screen to him/her. Here seller can provide day-2 operation hints or guidance that customer can be aware after the deployment.

This is a good place for guiding customers who has deployed and used that product.

.. image:: /_static/images/image16.png
   :width: 6.53194in
   :height: 2.71528in

Seller Helm Chart Address
^^^^^^^^^^^^^^^^^^^^^^^^^

Marketplace would require grabbing the Helm Chart of product from a helm registry. Here seller is supposed to put the address of that.

Seller Helm Chart Version
^^^^^^^^^^^^^^^^^^^^^^^^^

As each Helm Chart has different versions available, seller is supposed to mention which version from helm chart should be presented to customers. Marketplace would grab and on board only that specific version of helm chart.

Requested Release Date
^^^^^^^^^^^^^^^^^^^^^^

Based on the preference or company's policy, seller can let Marketplace knows when a proper time for that product (or product update) would be to get released and customers can use that.

Please be aware that Marketplace does not have any commitment to this date as there might be some technical efforts that marketplace needs to tackle before releasing that to customer.

Submit the request
^^^^^^^^^^^^^^^^^^

When seller is happy with the information, he/she has provided for the product and if all required data has been added and the product has been assessed by the seller itself, then it would be time to submit that for further investigation by Marketplace and set a release time for that. Please be aware that this might be a time consuming as marketplace should take care of some technical matters before preparing the product for release.

Seller would be notified by email when the product has been approved with a release time or has been rejected because of a reason.

CCE Bring Your Own License
~~~~~~~~~~~~~~~~~~~~~~~~~~

If you have a Helm Chart to deploy an application and your product needs a license in advance (Bring Your Own License), then this is the right choice to on-board that on Marketplace.

First step would be login Marketplace as a Seller as show in this picture.

.. image:: /_static/images/image6.png
   :width: 6.53194in
   :height: 1.79306in

Please be aware that only users which has “Tenant Administrator” role can login to the Marketplace as a Seller.

.. image:: /_static/images/image2.png
   :width: 6.53194in
   :height: 4.08958in

On the right side of the page, you would see a button named “Dashboard”.

.. image:: /_static/images/image17.jpg
   :width: 6.53194in
   :height: 2.42222in

Please click that and then select “Offering”.

.. image:: /_static/images/image18.jpg
   :width: 6.53194in
   :height: 2.35347in

Click on the new Offering to be forwarded to the new page to create your product. There you should fill out all the required information as needed.

.. image:: /_static/images/image10.png
   :width: 6.53194in
   :height: 3.05278in

Product Name
^^^^^^^^^^^^

Here you should pick up a name for your product. Customers would find you product in Marketplace with that name.

Please be aware that the product name is permanent and cannot be change as marketplace is committed to Customers that they always refer to the same name for specific product.

.. _service-type-1:

Service Type
^^^^^^^^^^^^

Here you should choose which type of product it would be. So far you can only choose CCE as the type of Product which is for Helm Charts to be offered.

.. _license-type-1:

License Type
^^^^^^^^^^^^

As mentioned before, seller is supposed to choose BYOL. This means that customer will get charged 0.00€ if they deploy that product. However, he/she is supposed to reach seller purchase website to buy a license before deploying that application.

.. _license-info-1:

License Info
^^^^^^^^^^^^

Here you can put information about licensing of your product which would be shown to customers when they select your Product inside Marketplace.

Secret Based License
^^^^^^^^^^^^^^^^^^^^

For Cloud-native products, normally customers are supposed to prepare a Kubernetes secret including the content of secret as a license file. Seller can user this toggle to activate that.

When this has been activated then seller can let the customers know what the secret name inside Kubernetes would be and what would be the file name of the license inside that secret. This means that anytime a customer deploys that product then before the deployment a Kubernetes secret named “Secret Name” having a file name as “License File Name” containing customer's license key would be created.

Webshop Link
^^^^^^^^^^^^

Seller would put the shopping link here so customers who want to use that product would use this link to be redirected to sellers' shopping address and purchase the license.

Secret Name
^^^^^^^^^^^

If the product is a cloud-native application and the activation would be automatically, then Kubernetes Secret is required. Here seller can set the secret name which is supposed to be created before deployment of the Helm Chart

Filename in the secret
^^^^^^^^^^^^^^^^^^^^^^

Here seller can set the license filename inside the Kubernetes secret.

Licensing Guide
^^^^^^^^^^^^^^^

If the product is not a cloud-native application and the activation would be manually, then no Kubernetes Secret is required. Then the seller is supposed to deactivate the “License Secret Creation”.

In that case the seller might have documentation already available and all he/she should do is to put the documentation link here so Customers can reach and learn about the activation.

.. _eula-1:

EULA
^^^^

Each company has some terms and conditions that clients need to agree on before using that product. Here Seller can add his/her EULA. When a customer wants to deploy that product, he/she needs to agree on that before being able to deploy that application.

.. _category-1:

Category
^^^^^^^^

Here seller can select in which category his/her product would fit in. Customer would filter product inside marketplace based on specific Category.

.. _version-1:

Version
^^^^^^^

Here you can set the version of your application so Customers would know which version of that has been presented in Marketplace.

.. _short-description-1:

Short Description
^^^^^^^^^^^^^^^^^

Short Description is the information that would be shown to Customers when they find it inside main page of Marketplace. This could be a brief introduction about the product that seller is offering.

.. _full-description-1:

Full Description
^^^^^^^^^^^^^^^^

When a customer would find and select a product, this description would go into details of that product and Customer can read and find more information about that product.

.. _logo-1:

Logo
^^^^

Here Seller is supposed to upload the logo of his/her product.

.. _used-software-used-software-license-name-and-link-to-license-1:

“Used Software”, “Used Software License Name” and “Link to License”
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As each application might have used other applications as component, Customers has the right to know which software has been used for that product. This include the name of that and name of the license that has been used for that (Such as MIT or Apache v2.0) so they could be able to review that and make sure this does not violate their policies.

This list of component's license information would be shown as the detail of the product.

Post Deployment Information
^^^^^^^^^^^^^^^^^^^^^^^^^^^

When a customer selects a product and deploys that, this message would be show on the screen to him/her. Here seller can provide day-2 operation hints or guidance that customer can be aware after the deployment.

This is a good place for guiding customers who has deployed and used that product.

.. _add-configuration-1:

Add Configuration
^^^^^^^^^^^^^^^^^

As the product is a Helm Chart, it has many keys that customer can customized by overwriting with new values. Although Helm Chart could have many keys to get customized, it is up to seller with of them should be on-boarded on Marketplace, so Customers be able to manipulate them.

Please be aware that some keys that have been added by seller to customize deployment could also be hidden to customer. This can be used when your help chart needs to be modified based on Open Telekom Cloud CCE and seller wants to make that change permanent, so customers did not change it by mistake.

Configurations could be a “Text input” (Text or Array), Option (Text or Array) which is like “Text Input” but default values are fixed and customer can only select from those values to choose or a Toggle (Boolean) that customer needs to make it as True or False.

.. _text-input-1:

Text input
''''''''''

This can be used for adding a key which is the type of string or array.

.. image:: /_static/images/image11.png
   :width: 6.53194in
   :height: 3.77361in

.. _configuration-key-3:

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

.. _text-input-label-1:

Text input label
                

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

.. _required-1:

Required
        

There are some configurations that could be optional or mandatory. If customer sets it then during deployment it would be overwrite and if not the default value form “values.yaml” would be picked up.

If there is a configuration that seller wants the customer to change it, then he/she can enable the required toggle so customers should put value for that.

.. _confidential-1:

Confidential
            

Some keys include some confidential information that during filling the key by customer, it should be treated as a confidential information and the content should be hidden.

For example, if the key is the default password of the application, then the seller can enable this feature. During the configuration it would be treated as a password and content cannot be seen during filling the information.

.. _validation-rule-1:

Validation Rule
               

If sellers want to restrict the content that customer would write as the value of that key, he/she can put regex rule, so customer are forced to follow that rule during filling the value. For that regex rule there is a “Error message” which seller can put hint or example to help customers to understand about the condition that is required.

.. _hidden-2:

Hidden
      

If seller enables that, then that configuration would be overwrite default helm chart value. However, customers are not able to see or change the content of that.

Please be aware that in that case “Default value” needs to be filled.

.. _multiple-2:

Multiple
        

This is the place where seller can set this configuration as an array. If multiple has been enabled, then customer can put more than one value for that key.

.. _default-value-2:

Default value
             

If seller wants, he/she can default value for that configuration. Customers would still be able to overwrite that.

.. _hint-text-2:

Hint text
         

This column could help customers by adding a hint under the label which could provide more help for Customers. It appears as a short line beneath that configuration label.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Hint text as “Kubernetes Storage Class for disk”. In that case customer would see a label named “storageClass” and beneath that a like which says, “Kubernetes Storage Class for disk”.

.. _tooltip-text-3:

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

.. _option-1:

Option
''''''

This can be used for adding a key which is the type of string or array. The only difference is that Seller makes the values to pick up prepared so customers can only pick from those lists. For instance, imagine you have a key “serviceType” and the answer should only be “ClusterIP”, “Nodeport” or “LoadBalancer”. Then the seller can pick that as the type of configuration and already add those as the pre-defined values.

.. image:: /_static/images/image12.png
   :width: 6.53194in
   :height: 3.69097in

.. _configuration-key-4:

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

.. _optional-label-1:

Optional label
              

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

.. _labelvalue-1:

Label/Value
           

There should a list of possible values to choose and a label for reach to help customer to understand which one to choose based on the situation.

.. _multiple-3:

Multiple
        

This is the place where seller can set this configuration as an array. If multiple has been enabled, then customer can put more than one value for that key.

.. _default-value-3:

Default value
             

If seller wants, he/she can default value for that configuration. Customers would still be able to overwrite that.

.. _hint-text-3:

Hint text
         

This column could help customers by adding a hint under the label which could provide more help for Customers. It appears as a short line beneath that configuration label.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Hint text as “Kubernetes Storage Class for disk”. In that case customer would see a label named “storageClass” and beneath that a like which says, “Kubernetes Storage Class for disk”.

.. _tooltip-text-4:

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

.. _toggle-1:

Toggle
''''''

This can be used for adding a key which is the type of Boolean.

.. image:: /_static/images/image13.png
   :width: 6.53194in
   :height: 3.75764in

.. _configuration-key-5:

Configuration Key
                 

Is the equivalent of Helm Chart key. It means that rules of the Yaml shall be followed here.

For example, if inside values.yaml file there is main key as “global” and then “storageClass” as sub key, then the content of “Configuration Key” would be “global. storageClass”

.. _togglelabel-1:

Toggle/label
            

This column is the label that customer see during configuration of deployment. Instead of the content of the key they would see this name for that configuration which means the name should be clear to understand for customer.

For example, for the key as “global. storageClass”, seller can pick up the label as “storageClass”. In that case customers would understand that they are supposed to put the name of the preferred Storage Class in here.

.. _default-state-1:

Default State
             

This variable by default is whether true or false.

.. _hidden-3:

Hidden
      

If seller enables that, then that configuration would be overwrite default helm chart value. However, customers are not able to see or change the content of that.

Please be aware that in that case “Default value” needs to be filled.

.. _tooltip-text-5:

Tooltip text
            

This column would be used to show additional help when customer hover his/her mouse on that configuration column.

For example, for the key as “global. storageClass” with the label of “storageClass”, seller can pick up the Tooltip text as “You can use kubectl get storageclass to list them”. In that case customer would see a label named “storageClass” and whenever hover his/her mouse over that label would see “You can use kubectl get storageclass to list them” above that column.

.. _add-pre-deployment-guide-1:

Add pre-Deployment guide
^^^^^^^^^^^^^^^^^^^^^^^^

When a customer selects a product, this message would be show on the screen to him/her. Here seller can provide pre-deployment hints or guidance that customer can be aware before the deployment.

This is a good place for guiding customers who wants to use that product.

.. image:: /_static/images/image14.png
   :width: 6.53194in
   :height: 2.74583in

.. _add-deployment-guide-1:

Add deployment guide
^^^^^^^^^^^^^^^^^^^^

Although hints and tooltips that seller would add to each configuration could be descriptive, seller needs to prepare small document to depict how to deploy and customize that product. The whole content would be shown to customer as an installation guide.

.. image:: /_static/images/image15.png
   :width: 6.53194in
   :height: 2.72431in

.. _post-post-deployment-guide-1:

Post post-deployment guide
^^^^^^^^^^^^^^^^^^^^^^^^^^

When a customer selects a product and deploys that, this message would be show on the screen to him/her. Here seller can provide day-2 operation hints or guidance that customer can be aware after the deployment.

This is a good place for guiding customers who has deployed and used that product.

.. image:: /_static/images/image16.png
   :width: 6.53194in
   :height: 2.71528in

.. _seller-helm-chart-address-1:

Seller Helm Chart Address
~~~~~~~~~~~~~~~~~~~~~~~~~

Marketplace would require grabbing the Helm Chart of product from a helm registry. Here seller is supposed to put the address of that.

.. _seller-helm-chart-version-1:

Seller Helm Chart Version
~~~~~~~~~~~~~~~~~~~~~~~~~

As each Helm Chart has different versions available, seller is supposed to mention which version from helm chart should be presented to customers. Marketplace would grab and on board only that specific version of helm chart.

.. _requested-release-date-1:

Requested Release Date
~~~~~~~~~~~~~~~~~~~~~~

Based on the preference or company's policy, seller can let Marketplace knows when a proper time for that product (or product update) would be to get released and customers can use that.

Please be aware that Marketplace does not have any commitment to this date as there might be some technical efforts that marketplace needs to tackle before releasing that to customer.

.. _submit-the-request-1:

Submit the request
~~~~~~~~~~~~~~~~~~

When seller is happy with the information, he/she has provided for the product and if all required data has been added and the product has been evaluated by the seller itself, then it would be time to submit that for further investigation by Marketplace and set a release time for that. Please be aware that this might be a time consuming as marketplace should take care of some technical matters before preparing the product for release.

Seller would be notified by email when the product has been approved with a release time or has been rejected because of a reason.

Test Deploy
~~~~~~~~~~~

Before offering a product to the customer, seller needs to make sure that the deployment would be successful, and customer would be able to use that. Marketplace provide this chance that before submitting a request to be reviewed and published, sellers can try that deployment and check any failure or issue.

It is highly recommended that seller try their product with different configuration to make sure customers would not face any failure during deployment.

This can be done when a new product is created or when a new update of old product is about to be presented.

To run it simply select the dashboard on the top right of the corner. Then select “Products”. There you can pick the product that you want to have test. Then you would see a list of available revision and can pick the one you want to evaluate the deployment. Below there must be a button named “Test deploy”. When you click on that you would see the list of configurations as customers can see to customize the deployment and deploy it to make sure everything is working fine.

Seller Dashboard
----------------

After a successful login, Seller would use the dashboard to manage the Offerings. This page is available to click on the top right corner of the page. Dashboard has been divided into two sections which we would discuss the details in below.

.. image:: /_static/images/image19.png
   :width: 6.53194in
   :height: 2.44931in

Offering
~~~~~~~~

By clicking in Product section in dashboard, Sellers can see all the products which have been created by themselves. It would show the status of them, available revisions which customers can see and use (In any has been approved by Marketplace to be shown), the type of the product (which could be CCE), Licensing Model (which could be Free, Open source or BYOL) and if the Product EOL has been set for that or not.

Seller can Edit each “Product Offering” to manage the it by updating, Unpublish/Publish or even putting it to the “End of Life status”.

Details of how to do each action would be discussed in the corresponding pages.

.. image:: /_static/images/image20.png
   :width: 6.53194in
   :height: 1.84653in

Workloads
~~~~~~~~~

Every time a deployment has been happened by seller, the status of that including the State, time and the name of the product would be recorded here so sellers can see if the deployment has been successful or not.

.. image:: /_static/images/image21.png
   :width: 6.53194in
   :height: 1.71111in

Product Lifecycle
-----------------

When a product has been created in Marketplace there are some activities which need to be done which requires some technical activities. Having said that, a product would have states as “Unpublished”, “Published” and “End of Life (EOL)”.

Unpublished
~~~~~~~~~~~

Unpublish is a temporary state which hide a product from customers to find and use which is revertible. When a Product born, the status of that would be “Unpublished”. This means this could not be seen by any customer at all. When the first version of its details (revision) gets approved then State of the product would change to “Published” that makes it possible for customers to see and use it in Marketplace. The state of product remains “Published” until Seller or Marketplace decide to change the status of that.

Please keep this in mind that status of Product and its revisions decide when a product would be visible to use.

Published
~~~~~~~~~

This the status of the product when it is active and can be shown to customers. Normally a product would remain as “Published” until a decision to hide temporarily or permanently that from Marketplace has been planned.

Please keep this in mind that status of Product and its revisions decide when a product would be visible to use.

“End of Life (EOL)”
~~~~~~~~~~~~~~~~~~~

A product would be available in Marketplace forever, until the seller has decided to off-board that from Marketplace. For instance, when a seller decides to retire his/her product form market and not support that anymore or when a re-branding has happened, and the product is supposed to be presented with new commercial name. in that case the seller can off-board the product from Marketplace. In Marketplace there a concrete rule for off-boarding based on the time of request as following:

-  If the request submitted until the middle of current month, then Marketplace would set the EOL time as the end of current month.

-  If the request submitted in the next half of the month, then Marketplace would set the EOL time as the end of upcoming month.

After the time for EOL has been reached, then none can see and use that product in the Marketplace.

Please be aware that this process is irreversible, and Seller cannot bring that product back to business anymore!

Revision Lifecycle
------------------

A Product is just an entity that represent an output regarding the application that seller wants to present inside Marketplace It would remain the same forever until a product get retired. Revision, however, is the list of attributes of that product which would change eventually. For instance, description, logo, configurations or even the price can change anytime. Revisions are the why to present changes of the same product every time the seller wants to update his/her product.

Revisions as needed to be approved by Marketplace has also lifecycle. Every time the seller wants to update a product, he/she should create a new revision and make sure that it is fine for the customers to use then Marketplace would take care of the reset of technical tasks. Eventually the new update of product (by on boarding the new revision) would be shown to customers on specific time that has been set for that revision by Marketplace.

Revision lifecycle would be as bellow.

Draft
~~~~~

The first time a revision has been created the status of that revision is “Draft”. This means this the time that Seller can play with the details and add as much information as he/she wants. During this time seller has the option to spend as much time as he/she needs to prepare the update for that product.

Read-to-Review
~~~~~~~~~~~~~~

After all changes that the seller wanted has been done, he/she would submit this new revision to marketplace. It is time for Marketplace to review the information of that and make sure all technical requirements have been done and customers would be able to use the product with this revision or not.

Rejected
~~~~~~~~

There might be some situations that the revision which has been offered by seller has some technical issue and marketplace want seller to take care of that. In that case the revision gets rejected and Seller would get informed about the reason of rejection.

A rejected revision can simply get back to “Draft” so seller can take care of the reason of rejection.

Approved
~~~~~~~~

Finally, when the revision got reviewed by Marketplace and passed all the concerns of Marketplace, then the revision gets approved and can be shown to the customer at specific time which has been set by Marketplace.

Please be aware when a new revision of a product got approve, at the time of release, the old approve one will not be shown to customer and would be replaced by new one.

Update Product Offering
-----------------------

When a product has been released, it means it has the first revision approved that all details has been approved by marketplace. However, as all products eventually got new technical updates, Seller can update the content by updating that product by a new revision.

This process looks the same when seller created the Offering for the first time with only slight changes that the name, service type and the license type cannot be changed as we discussed previously during product creation.

The rest of the procedure and configuration would be the same as creating the product for the first time.

To update the product seller needs to click on “Dashboard” on the top right corner and then “Offering”.

.. image:: /_static/images/image19.png
   :width: 6.53194in
   :height: 2.44931in

There he/she can pick up the Offering he/she wants to update.

.. image:: /_static/images/image20.png
   :width: 6.53194in
   :height: 1.84653in

If there is already a revision with the status of “Draft”, then seller can edit that and continue working on that. If not, Seller has two options to create a new revision to update the product.

One way is to click on “New Revision” which automatically create a new revision with the exact data of the last approved revision for the ease of convenience.

The other way is to edit any already-approved revision and click to create a new revision out of it.

.. image:: /_static/images/image22.png
   :width: 6.53194in
   :height: 2.49306in

Unpublish/Re-Publish Product
----------------------------

There might be some reason that the seller/Marketplace want a product to be hidden from customers for coupe of day because of specific reason.

For instance, if there is a security issue on the current product and seller needs time to come up with a new version then the seller can temporarily hide the product by switching the product to “Unpublish”.

To unpublish a product, seller needs to click on “Dashboard” on the top right corner and then “Products”.

|image1|\ There he/she can pick up the Offering he/she wants to Unpublish.

.. image:: /_static/images/image20.png
   :width: 6.53194in
   :height: 1.84653in

Then there is a button named “Unpublish”. Seller can select that and change that product state to “Unpublished”.

.. image:: /_static/images/image22.png
   :width: 6.53194in
   :height: 2.49375in

Reverting the process is as Unpublishing. Seller just needs to select the product and this time click on the button named “Publish”.

Put Offering into “End of Life”
-------------------------------

A product would be available in Marketplace forever, until the seller has decided to off-board that from Marketplace. For instance, when a seller decides to retire his/her product form market and not support that anymore or when a re-branding has happened, and the product is supposed to be presented with new commercial name. in that case the seller can off-board the product from Marketplace. In Marketplace there a concrete rule for off-boarding based on the time of request as following:

-  If the request submitted until the middle of current month, then Marketplace would set the EOL time as the end of current month.

-  If the request submitted in the next half of the month, then Marketplace would set the EOL time as the end of upcoming month.

To put a product into “End of Life”, seller needs to click on “Dashboard” on the top right corner.

.. image:: /_static/images/image19.png
   :width: 6.53194in
   :height: 2.44931in

Then select “Offering”. There he/she can pick up the Product he/she wants to retire.

.. image:: /_static/images/image20.png
   :width: 6.53194in
   :height: 1.84653in

Then there is a button named “End of Life”.

.. image:: /_static/images/image22.png
   :width: 6.53194in
   :height: 2.49375in

Please be aware that this process is irreversible, and Seller cannot bring that product back to business anymore!

.. |image1| image:: /_static/images/image19.png
   :width: 6.53194in
   :height: 2.44931in

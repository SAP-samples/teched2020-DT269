# Exercise 1 - Setup connection between ITCM and Kyma runtime

In this exercise, you will set up a connection between ITCM and Kyma runtime, register ITCM domain events on Kyma runtime.

## Step 1.1 - Create an ITCM application in Kyma runtime

1.Create an ITCM application from the Kyma cockpit.
![](/exercises/ex1/images/e1-create-app.png)

2.Bind ITCM application to a namespace.
![](/exercises/ex1/images/e1-create-app-binding.png)

## Step 1.2 - Register Kyma runtime in ITCM Extension Center

1.Register Kyma runtime in the ITCM Extension Center on the system tab.
![](/exercises/ex1/images/e1-register-kyma.png)

## Step 1.3 - Register ITCM exposed domain event APIs

Expose the domain event to Kyma runtime through a secure connection.

***To secure the connection, you need to generate a private key by the OpenSSL tool and request a certificate signed by Kyma runtime.***
***The credential is mandatory for the communication with Kyma runtime.***
</br>Detail steps:[here](https://kyma-project.io/docs/components/application-connector/#tutorials-get-the-client-certificate)

1.Choose claims from the categorized event on the Event Mesh tab.
<br>![](/exercises/ex1/images/e1-events-list.png)

2.Event reference for claims.
<br>![](/exercises/ex1/images/e1-events-detail.png)

3.Define a channel for claims event publishing.
<br>![](/exercises/ex1/images/e1-events-channel.png)

## Summary

Now the connection between ITCM & Kyma runtime is ready,</br>
Continue to - [Exercise 2 - Implement extensional functions in Kyma runtime](../ex2/README.md)
